<script lang="ts">
  import { MetaTags } from "svelte-meta-tags";
  import socialImage from "$lib/assets/polkadot.png";
</script>

<MetaTags
  title="Enjin Canary Faucet"
  description="A fast and reliable Enjin testnet faucet for blockchain developers."
  openGraph={{
    images: [{ url: socialImage }],
  }}
  twitter={{
    title: "Enjin Canary Faucet",
    description: "A fast and reliable Enjin testnet faucet for blockchain developers.",
    image: socialImage,
    imageAlt: "Enjin Canary Faucet Website",
  }}
/>
