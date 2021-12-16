<template>
  <div>
    <Navbar />
    <main>
      <Hero />
    </main>
    <Features />
    <UniqApp />
    <SiteFooter />
  </div>
</template>

<script>
import Hero from "./components/sections/Hero";
import Features from "./components/sections/Features";
import UniqApp from "./components/sections/UniqApp";
import Navbar from "./components/layouts/Navbar";
import SiteFooter from "./components/layouts/SiteFooter";
export default {
  name: "App",
  components: {
    Navbar,
    Features,
    UniqApp,
    Hero,
    SiteFooter,
  },
};
</script>
