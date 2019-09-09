<template>
    <div class="location-bar">
        <div class="location-text">
            <span class="anc-loc">
                                <img width="24" src="../assets/icons/location-pin.svg">
                <span class="ml-5">در محدوده</span>
                <strong class="loc-title">دزفول </strong>
            </span>
            <div id="location"></div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "LocationBar"
    }
</script>

<style scoped lang="scss">
    @import "../scss/variables";
    .location-bar {
        text-align: center;
        padding: 10px ;
        border-bottom: 1px solid #e5e5e5;
        -webkit-box-shadow: 0 4px 6px -5px #d2d2d2;
        -moz-box-shadow: 0 4px 6px -5px #d2d2d2;
        box-shadow: 0 4px 6px -5px #d2d2d2;
    }


    .loc-title {
        color: $global-primary-background;
        cursor: pointer;
        border-bottom: 1px dotted transparent;
        -webkit-transition: all .25s cubic-bezier(.19,1,.22,1);
        -moz-transition: all .25s cubic-bezier(.19,1,.22,1);
        -o-transition: all .25s cubic-bezier(.19,1,.22,1);
        transition: all .25s cubic-bezier(.19,1,.22,1);
        -webkit-touch-callout: none;
        font-weight: 700;
        -webkit-user-select: none;
        -khtml-user-select: none;
        -moz-user-select: none;
        -ms-user-select: none;
        user-select: none;
        vertical-align: middle;
        display: inline-block;
    }
    .loc-title:after {
        font-family: 'Material Icons';
        content: "expand_more";
        vertical-align: middle;
    }
</style>
