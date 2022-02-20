<template>
    <div class="hello">
        
        <!-- Base header -->
        <h1>Base Header</h1>
        <br>
        <base-header/>
        <br><br><br><br><br>
        <!-- End base header -->

        <!-- Base intro -->
        <h1>Base intro</h1>
        <br>
        <base-intro/>
        <br><br><br><br><br>
        <!-- End base intro -->

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

        <!-- Base nft -->
        <h1>Base nft</h1>
        <br>
        <base-nft/>
        <br><br><br><br><br>
        <!-- End base nft -->

        <!-- Base learn -->
        <h1>Base learn</h1>
        <br>
        <base-learn/>
        <br><br><br><br><br>
        <!-- End base learn -->

        <!-- Base upsell -->
        <h1>Base upsell</h1>
        <br>
        <base-upsell/>
        <br><br><br><br><br>
        <!-- End base upsell -->
        
        <!-- Base press -->
        <h1>Base press</h1>
        <br>
        <base-press/>
        <br><br><br><br><br>
        <!-- End base press -->

        <!-- Base footer -->
        <h1>Base footer</h1>
        <br>
        <base-footer/>
        <br><br><br><br><br>
        <!-- End base footer -->

    </div>
</template>

<script>
import BaseHeader from '../components/base/BaseHeader.vue';
import BaseIntro from '../components/base/BaseIntro.vue';
import BaseHero from '../components/base/BaseHero.vue';
import BaseCard from '../components/base/BaseCard.vue';
import BaseSection from '../components/base/BaseSection.vue';
import BaseItem from '../components/base/BaseItem.vue';
import BaseTrend from '../components/base/BaseTrend.vue';
import BaseNft from '../components/base/BaseNft.vue';
import BaseLearn from '../components/base/BaseLearn.vue';
import BaseUpsell from '../components/base/BaseUpsell.vue';
import BasePress from '../components/base/BasePress.vue';
import BaseFooter from '../components/base/BaseFooter.vue';

export default {
    components: {
        BaseHeader,
        BaseIntro,
        BaseHero,
        BaseCard,
        BaseSection,
        BaseTrend,
        BaseItem,
        BaseNft,
        BaseLearn,
        BaseUpsell,
        BasePress,
        BaseFooter,
        
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