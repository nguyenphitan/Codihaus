<template>
    <div id="t-base-nft">
        <div id="t-nft-container">
            <!-- Background image -->
            <div class="t-nft-background">
                <img :src="require(`@/assets/imgs/${imgName}`)" />
            </div>

            <!-- content -->
            <div id="t-nft-content">
                <!-- Left -->
                <div class="t-nft-left">
                    <div class="t-nft-series">{{series}}</div>
                    <div 
                        class="t-purple-man"
                        :class="{'t-color-white' : !imgName.indexOf('nftt')}"
                    >{{purpleMan}}</div>

                    <div 
                        class="t-nft-rank"
                        :class="{'t-color-cccccc' : !imgName.indexOf('nftt')}"
                    >{{rank}}</div>
                </div>

                <!-- Right -->
                <div class="t-nft-right">
                    <div 
                        class="t-top-bid" 
                        :class="{'t-color-white' : !imgName.indexOf('nftt')}"
                    >{{topBid}}</div>

                    <div 
                        class="t-nft-price"
                        :class="{'t-color-white' : !imgName.indexOf('nftt')}"
                    > <span class="t-price"></span> {{price}}</div>
                    
                    <div 
                        class="t-day-left"
                        :class="{'t-color-cccccc' : !imgName.indexOf('nftt')}"
                    >{{dayLeft}}</div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        series: {
            type: String,
            default: ''
        },
        purpleMan: {
            type: String,
            default: ''
        },
        rank: {
            type: String,
            default: '#12'
        },
        topBid: {
            type: String,
            default: 'TOP BID'
        },
        price: {
            type: String,
            default: '2.99 ETH'
        },
        dayLeft: {
            type: String,
            default: '1 day left'
        },
        imgName: {
            type: String,
            default: 'nft1.png'
        }
    }
}
</script>

<style scoped>
@import url('../../style/base/nft.css');
</style>