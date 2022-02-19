<template>
    <div id="t-base-item">
        <div id="t-item-container">
            <!-- Left -->
            <div id="t-item-left">
                <div class="t-item-img">
                    <img src="../../assets/imgs/Ellipse7.png">
                </div>
                <div class="t-item-info">
                    <div class="t-item-name">#1 - Roundiiies</div>
                    <div class="t-lowest-price">Lowest Price: <span class="t-price"></span> 45.2</div>
                </div>
            </div>

            <!-- Right -->
            <div id="t-item-right">
                <div class="t-item-mobilize">+1,095.3%</div>
                <div class="t-item-price"> <span class="t-price"></span> 87,490.32</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'base-item',
    // props: {
    //     url: {
    //         type: String,
    //         default:'../../assets/imgs/hero-image.png'
    //     }
    // },
    data() {
        return {
            
        }
    },
    // methods: {
    //     resolve_img_url: function (path) {
    //         let images = require.context('../../assets/', false, /\.png$|\.jpg$/)
    //         return images("./"+path)
    //     }
    // }
}
</script>

<style scoped>
@import url('../../style/base/item.css');
</style>