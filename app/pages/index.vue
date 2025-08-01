<!-- <template>
  <div>
    <HeroSection />
    <FeatureSlider />

    <FeaturedProducts />
  </div>
</template>

<script setup>
import HeroSection from "@/components/HeroSection.vue";
import FeatureSlider from "@/components/FeaturedSlider.vue";
import FeaturedProducts from "./FeaturedProducts.vue";
</script> -->


<template>
  <div>
    <HeroSection />
    <FeaturedCategories />
    <LookbookSection />
    <BrandIntro />
    <PromoPopup />
    <ServicesSection />
  </div>
</template>

<script setup>
import HeroSection from "@/components/HeroSection.vue";
import FeaturedCategories from "./FeaturedCategories.vue";
import LookbookSection from "./LookbookSection.vue";
import BrandIntro from "./BrandIntro.vue";
import PromoPopup from "./PromoPopup.vue";
import ServicesSection from "./ServicesSection.vue";
</script>
