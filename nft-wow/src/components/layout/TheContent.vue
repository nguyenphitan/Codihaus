<template>
    <div id="t-the-content">
        <div id="t-content-container">
            <!-- Hero -->
            <base-hero/>
            <!-- End hero -->

            <!-- Intro cards -->
            <div id="t-intro-cards">
                <base-card 
                    :showIcon="true" 
                    :imgName="imgName[1]"
                    :btnStyle="false"
                />
                <base-card 
                    :showIcon="true" 
                    :title="title[2]"
                    :text="text[2]"
                    :buttonName="buttonName[2]"
                    :imgName="imgName[2]"
                    :btnStyle="false"
                />
            </div>
            <!-- End intro cards -->

            <!-- Upcoming drops -->
            <div id="t-upcoming-drops">
                <base-section/>
                <div id="t-upcoming-cards">
                    <base-card
                        style="background-color: #FFD8E6;"
                        class="t-FF005C"
                        :title="title[3]"
                        :text="text[3]"
                        :buttonName="buttonName[3]"
                        :imgName="imgName[3]"
                    />
                    <base-card
                        style="background-color: #F2D8FF;"
                        class="t-AA00FF"
                        :title="title[4]"
                        :text="text[4]"
                        :buttonName="buttonName[4]"
                        :imgName="imgName[4]"
                    />                         
                </div>
            </div>
            <!-- End upcoming drops -->

        </div>
    </div>
</template>

<script>
import BaseCard from '../base/BaseCard.vue';
import BaseHero from '../base/BaseHero.vue';
import BaseSection from '../base/BaseSection.vue';

export default {
    name: 'the-content',
    components: {
        BaseHero,
        BaseCard,
        BaseSection,
    },
    data() {
        return {
            title: [
                '', '',
                'Finance with 0% APR',
                'CHARBlobs',
                'Jeanie Tyu',

            ],
            text: [
                '', '',
                'We have partnered with Zlamra to allow you to finance your NFT investments with zero fees.',
                'This new collection by Muxhy recreates some of his most famous characters in 3D.',
                'Artist Jeanie Tyu’s new exhibition in Tokyo consists of ten artworks which will be available for sale on NFTwow.',

            ],
            buttonName: [
                '', '',
                'Learn More',
                '00:01:09:34',
                '02:03:32:17',


            ],
            imgName: [
                '',
                'Rectangle9.png',
                'Rectangle91.png',
                '92.png',
                '93.png',


            ],
        }
    },
}
</script>

<style scoped>
#t-the-content {
    margin-top: 80px;
}

/* intro cards */
#t-the-content #t-intro-cards, 
#t-upcoming-drops #t-upcoming-cards {
    display: flex;
    justify-content: space-between;
}

/* Upcomine drops */
#t-upcoming-drops {
    margin-top: 56px;
}

#t-upcoming-drops #t-upcoming-cards {
    margin-top: 32px;
}

</style>