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

            <!-- List trending and new -->
            <div id="t-list-area">
                <base-trend 
                    class="t-right-24"
                    :arrInfo="topTrending"
                />
                <base-trend
                    :title="'New & Noteworthy'"
                    :paragraph="'See what’s up and coming this week.'"
                    :arrInfo="newNoteworthy"
                />
            </div>
            <!-- End list trending and new -->

            <!-- Ending soon -->
            <div id="t-ending-soon">
                <base-section 
                    :title="'Ending Soon'" 
                    :paragraph="'Check out featured NFT auctions that are ending soon.'"
                />
                <div class="t-ending-list">
                    <div v-for="(item, index) in arrEndings" :key="index">
                        <base-nft
                            :imgName="item.imgName"
                            :series="item.series"
                            :price="item.price"
                            :purpleMan="item.purpleMan"
                            :rank="item.rank"
                            :topBid="item.topBid"
                            :dayLeft="item.dayLeft"
                        />
                    </div>
                </div>
            </div>
            <!-- End Ending soon -->

        </div>
    </div>
</template>

<script>
import BaseCard from '../base/BaseCard.vue';
import BaseHero from '../base/BaseHero.vue';
import BaseNft from '../base/BaseNft.vue';
import BaseSection from '../base/BaseSection.vue';
import BaseTrend from '../base/BaseTrend.vue';

export default {
    name: 'the-content',
    components: {
        BaseHero,
        BaseCard,
        BaseSection,
        BaseTrend,
        BaseNft,
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
            topTrending: [
                {
                    name: '#1 - Roundiiies',
                    lowestPrice: '45.2',
                    mobilize: '+1,095.3%',
                    price: '87,490.32',
                    imgName: 'Ellipse7.png'
                },
                {
                    name: '#2 - Flewid',
                    lowestPrice: '2.5',
                    mobilize: '-5.3%',
                    price: '5,984.23',
                    imgName: '2.png'
                },
                {
                    name: '#3 - Angel of Moon',
                    lowestPrice: '19.4',
                    mobilize: '+19.6%',
                    price: '109,938.11',
                    imgName: '3.png'
                },
                {
                    name: '#4 - Goggle Eyes',
                    lowestPrice: '0.7',
                    mobilize: '-1.9%',
                    price: '65,382.17',
                    imgName: '4.png'
                },
                {
                    name: '#5 - Paradize',
                    lowestPrice: '82.3',
                    mobilize: '+214.8%',
                    price: '10,980.66',
                    imgName: '5.png'
                },
            ],
            newNoteworthy: [
                {
                    name: '#1 - Bored Something',
                    lowestPrice: '34.7',
                    mobilize: '+33,902.6%',
                    price: '11,192.84',
                    imgName: '6.png'
                },
                {
                    name: '#2 - LTD SOCKS',
                    lowestPrice: '1.8',
                    mobilize: '+11,231.33%',
                    price: '75,094.33',
                    imgName: '7.png'
                },
                {
                    name: '#3 - SpAcEwArP',
                    lowestPrice: '1.9',
                    mobilize: '+1,982.0%',
                    price: '4,908.39',
                    imgName: '8.png'
                },
                {
                    name: '#4 - BUILDblcks',
                    lowestPrice: '10.4',
                    mobilize: '+709.9%',
                    price: '1,093.84',
                    imgName: '9.png'
                },
                {
                    name: '#5 - Roman Empire',
                    lowestPrice: '11.4',
                    mobilize: '+580.3%',
                    price: '4,095.37',
                    imgName: '10.png'
                },
            ],
            arrEndings: [
                {
                    imgName: 'nft1.png',
                    series: 'Flowitars',
                    purpleMan: 'Floppy',
                    rank: '#12',
                    topBid: 'TOP BID',
                    price: '2.99ETH',
                    dayLeft: '1 day left',
                },
                {
                    imgName: 'nftt2.png',
                    series: 'Anna Kuife',
                    purpleMan: 'Merlge',
                    rank: '#8745',
                    topBid: 'TOP BID',
                    price: '1.23ETH',
                    dayLeft: '2 day left',
                },
                {
                    imgName: 'nftt3.png',
                    series: 'MUSIKC',
                    purpleMan: 'Starr Eyes',
                    rank: '#192',
                    topBid: 'TOP BID',
                    price: '0.71ETH',
                    dayLeft: '3 day left',
                },
                {
                    imgName: 'nft4.png',
                    series: 'BLOODFLOW',
                    purpleMan: 'H e l p',
                    rank: '#54',
                    topBid: 'TOP BID',
                    price: '5.90ETH',
                    dayLeft: '5 day left',
                },
                
            ],

        }
    },
}
</script>

<style scoped>
@import url('../../style/layout/content.css');
</style>