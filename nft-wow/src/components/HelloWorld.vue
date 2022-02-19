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

        <!-- Base section -->
        <h1>Base section</h1>
        <br>
        <base-section/>
        <br><br><br><br><br>
        <!-- End base section -->

        <!-- Base item -->
        <h1>Base item</h1>
        <br>
        <base-item/>
        <br><br><br><br><br>
        <!-- End base item -->

        <!-- Base trend -->
        <h1>Base trend</h1>
        <br>
        <base-trend/>
        <br><br><br><br><br>
        <!-- End base trend -->

        


    </div>
</template>

<script>
import BaseHeader from '../components/base/BaseHeader.vue';
import BaseHero from '../components/base/BaseHero.vue';
import BaseCard from '../components/base/BaseCard.vue';
import BaseSection from '../components/base/BaseSection.vue';
import BaseItem from '../components/base/BaseItem.vue';
import BaseTrend from '../components/base/BaseTrend.vue';

export default {
    components: {
        BaseHeader,
        BaseHero,
        BaseCard,
        BaseSection,
        BaseTrend,
        BaseItem,

    },
    data() {
        return {
            
        }
    },
}
</script>

<style scoped>
.hello {
    margin: 0 64px;
    overflow: hidden;
}
</style>