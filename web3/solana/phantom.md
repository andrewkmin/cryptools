# Tinkering with Solana via Phantom
Phantom docs: https://docs.phantom.app/ 

At this point in time, Phantom has established itself as the leading wallet of the Solana ecosystem. Other prominent wallets include Solflare, which also has gained significant traction.

Assuming the client side is using React, getting setup is relatively simple:

```javascript
// Import bare React necessities
import React, { useEffect } from 'react';
...

// Check for the presence of an injection of a Solana instance, and in particular a Phantom wallet
const checkWallet = async () => {
  try { 
    const { solana } = window;

    if (solana && solana.isPhantom) {
      // Attempt to connect to Phantom. The `onlyIfTrusted` flag is used to ensure that the wallet only connects if
      // the dapp has been authorized.
      const response = await solana.connect({ onlyIfTrusted: true });

      // You can access your public key as follows:
      console.log(`public key: ${response.publicKey.toString()}`);
    } else {
      console.log(`y'all need phantom`);
    }
  } catch (error) {
    console.error(error);
  }
}

// Attempt to connect Phantom wallet
const connectWallet = async () => {
  const { solana } = window;

  if (solana) {
    // note: we must omit the `onlyIfTrusted` flag here since the first time around, we need to *establish* trust 
    const response = await solana.connect();
    console.log(`connected with public key: ${response.publicKey.toString()}`);
    setWalletAddress(response.publicKey.toString());
  }
};

// Use some React magic to checkWallet() upon component mount
useEffect(() => {
  const onLoad = async () => {
    await checkWallet();
  };

  // We only want to check once the page is fully loaded
  window.addEventListener('load', onLoad);
  return () => window.removeEventListener('load', onLoad);
}, []);

// Monitor state of walletAddress
useEffect(() => {
    if (walletAddress) {
      console.log(`wallet address: ${walletAddress}`);

      // do anything
    }
  }, [walletAddress]);
```

H/t to Buildspace for the baseline of this content.
