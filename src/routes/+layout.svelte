<script lang="ts">
  import "../app.css";
  import Footer from "../components/Footer.svelte";
  import Header from "../components/Header.svelte";
  import { injectSpeedInsights } from "@vercel/speed-insights/sveltekit";

  injectSpeedInsights();
</script>

<div class="flex flex-col">
  <Header />
  <slot />
  <Footer />
</div>
