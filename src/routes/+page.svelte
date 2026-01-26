<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import WhyAttend from "$lib/components/WhyAttend.svelte";
  import Passes from "$lib/components/Passes.svelte";
  import Speakers from "$lib/components/Speakers.svelte";
  import Agenda from "$lib/components/Agenda.svelte";
  import Sponsors from "$lib/components/Sponsors.svelte";
  import FAQ from "$lib/components/FAQ.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<svelte:head>
  <title>ACEF - Fueling Africa's New Generation of Creators</title>
  <meta name="description" content="ACEF delivers upfront event capital via receivables-backed loans secured by MOOKH's automated ticket sales platform. World's first tokenized creative industry bond." />
</svelte:head>

<main class="bg-[#F7F7F8] min-h-screen font-sans text-[#110F28] selection:bg-[#110F28] selection:text-white">
  <Header />
  <Hero />
  <WhyAttend />
  <Agenda />
  <Passes />
  <Speakers />
  <Sponsors />
  <FAQ />
  <Footer />
</main>

