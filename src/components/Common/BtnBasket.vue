<template>
    <div class="basket">
        <button class="btn-inner btn-bg">

            <i class="material-icons-outlined  mr-5 icon">shopping_cart</i>
            <div class="badge pl-5">3</div>
        </button>
    </div>
</template>

<script>
    export default {
        name: "BtnBasket"
    }
</script>

<style scoped lang="scss">
    @import "../../scss/variables";
    .btn-inner{
        height: 42px;
    }

    .btn-bg{
        cursor: pointer;
        position: relative;
        direction: ltr;
        min-width: 60px;
        height: 43px;
        padding: 0 10px;
        display: inline-block;
        background: $global-primary-background;
        background: -moz-linear-gradient(-60deg,$global-primary-background 0,$global-accent-background 100%);
        background: -webkit-gradient(linear,left bottom,right top,color-stop(0,$global-primary-background),color-stop(100%,$global-accent-background));
        background: -webkit-linear-gradient(-60deg,$global-primary-background,$global-accent-background);
        background: -o-linear-gradient(-60deg,$global-primary-background 0,$global-accent-background 100%);
        background: -ms-linear-gradient(-60deg,$global-primary-background 0,$global-accent-background 100%);
        background: linear-gradient(-60deg,$global-primary-background,$global-accent-background);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="$color1",endColorstr="$color2",GradientType=1);
        color: #fff;
        -webkit-transition: all .25s cubic-bezier(.19,1,.22,1);
        -moz-transition: all .25s cubic-bezier(.19,1,.22,1);
        -o-transition: all .25s cubic-bezier(.19,1,.22,1);
        transition: all .25s cubic-bezier(.19,1,.22,1);
        -webkit-border-radius: 5px;
        -moz-border-radius: 5px;
        border-radius: 5px;
        margin-right: 10px;
        border: 0;
    }

    .btn-bg:active{
        border : 1px solid darken($global-primary-background, 15%);
    }
    .badge{
        display: inline-block;
        font-size: 20px;
        vertical-align: bottom;
    }
</style>
