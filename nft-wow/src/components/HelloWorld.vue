<template>
    <div class="hello">
        
        <!-- Base header -->
        <h1>Base Header</h1>
        <br>
        <base-header/>
        <br><br><br><br><br>
        <!-- End base header -->

        <!-- Base hero -->
        <h1>Base hero</h1>
        <br>
        <base-hero/>
        <br><br><br><br><br>
        <!-- End base hero -->

        <!-- Base card -->
        <h1>Base card</h1>
        <br>
        <base-card/>
        <br><br><br><br><br>
        <!-- End base card -->


    </div>
</template>

<script>
import BaseHeader from '../components/base/BaseHeader.vue';
import BaseHero from '../components/base/BaseHero.vue';
import BaseCard from '../components/base/BaseCard.vue';
export default {
    components: {
        BaseHeader,
        BaseHero,
        BaseCard,
    },
    data() {
        return {
            
        }
    },
}
</script>

<style scoped>

</style>