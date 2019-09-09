<template>
<div class="navbar">
    <nav class="uk-navbar-container bg-white pr-20 pl-20 pt-20 pb-20" uk-navbar>
        <div class="uk-navbar-right">
            <button  class="uk-button btn-outlined btn-h uk-visible@s">ورود | ثبت نام</button>
            <button  class="uk-button btn-outlined btn-h uk-hidden@s">ورود</button>
        </div>
        <div class="uk-navbar-center">
            <a class="uk-navbar-item uk-logo" href="#">
                <img width="100" src="../assets/images/logo.svg" onerror="this.src='yours.png'">.
            </a>
        </div>
        <div class="uk-navbar-left">
            <BtnBasket/>
        </div>
    </nav>
    <hr class="uk-divider-icon m-0">
    <LocationBar/>
</div>
</template>
<script>
    import BtnBasket from "./Common/BtnBasket";
    import LocationBar from "./LocationBar";
    export default {
        name: "Navbar",
        components: {LocationBar, BtnBasket}
    }
</script>

<style scoped>
    .btn-h{
        height: 43px;
    }
</style>
