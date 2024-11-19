<script lang="ts">
  import "../app.css";
  import Footer from "../components/Footer.svelte";
  import Header from "../components/Header.svelte";

  import { injectSpeedInsights } from "@vercel/speed-insights/sveltekit";
  import { inject } from "@vercel/analytics";

  injectSpeedInsights();
</script>

<div class="flex flex-col w-full h-screen bg-slate-300">
  <Header />
  <slot />
  <Footer />
</div>
