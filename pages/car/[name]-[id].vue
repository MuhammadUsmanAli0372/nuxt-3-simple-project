<template>
    <div>
        <!-- CAR DETAIL PAGE -->
        <!-- <div class="mx-auto mt-4 max-w-7xl space-y-4 px-4 xs:px-8 sm:px-10 lg:px-16 pb-16 w-3/5"> -->
            
            <!-- CAR HERO -->
            <CarDetailHero />
            <!-- CAR HERO -->

            <!-- CAR ATTRIBUTES -->
            <CarDetailAttributes />
            <!-- CAR ATTRIBUTES -->

            <!-- CAR DESCRISPTION -->
            <CarDetailDescription />
            <!-- CAR DESCRISPTION -->

            <!-- CAR CONTACT -->
            <CarDetailContact />
            <!-- CAR CONTACT -->
        <!-- </div> -->
        <!-- CAR DETAIL PAGE   -->
    </div>
</template>

<script setup>
const route = useRoute();
const { toTitleCase } = useUtilities();

useHead({
    title: toTitleCase(route.params.name)
});

definePageMeta({
  layout: 'custom',
});
</script>