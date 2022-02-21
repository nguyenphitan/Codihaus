<template>
    <div id="t-base-item">
        <div id="t-item-container">
            <!-- Left -->
            <div id="t-item-left">
                <div class="t-item-img">
                    <!-- <img src="@/assets/imgs/Ellipse7.png"> -->
                    <img :src="require(`@/assets/imgs/${imgName}`)"/>
                </div>
                <div class="t-item-info">
                    <div class="t-item-name">{{name}}</div>
                    <div class="t-lowest-price">Lowest Price: <span class="t-price"></span> {{lowestPrice}}</div>
                </div>
            </div>

            <!-- Right -->
            <div id="t-item-right">
                <div 
                    class="t-item-mobilize"
                    :class="{'t-red' : !mobilize.indexOf('-')}"
                >{{mobilize}}</div>
                
                <div class="t-item-price"> <span class="t-price"></span> {{price}}</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'base-item',
    props: {
        imgName: {
            type: String,
            default: 'Ellipse7.png'
        },
        name: {
            type: String,
            default: ''
        },
        lowestPrice: {
            type: String,
            default: ''
        },
        mobilize: {
            type: String,
            default: ''
        },
        price: {
            type: String,
            default: ''
        },
    },
    data() {
        return {
        }
    },
}
</script>

<style scoped>
@import url('../../style/base/item.css');
</style>