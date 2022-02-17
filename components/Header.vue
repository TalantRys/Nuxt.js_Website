<template>
    <header>
        <div class="header__container container">
            <nuxt-link to="/" exact class="header__logo">Scake</nuxt-link>
            <ul class="header__list">
                <li><nuxt-link active-class="active-link" exact no-prefetch to="/" class="header__link">Торты</nuxt-link></li>
                <li><nuxt-link active-class="active-link" to="/about" class="header__link">Доставка</nuxt-link></li>
                <li><nuxt-link active-class="active-link" to="/Delivery" class="header__link">О нас</nuxt-link></li>
            </ul>
            <ul class="header__buttons">
                <li><nuxt-link active-class="active-link" exact no-prefetch to="#" class="header__button">Свяжитесь с нами</nuxt-link></li>
                <li><span active-class="active-link" to="#" class="header__button header__button_cart"><img src="~assets/images/icons/shopping-cart.svg" alt="shopping cart"> Корзина</span></li>
            </ul>
        </div>
    </header>
</template>
<style>
    header{
        background: #B5838D99;
        width: 100%;
        position: fixed;
        top: 0;
        left: 0;
    }
    .header__logo, .header__link{
        color: #fff;
    }
    .header__container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100px;
        margin: 0 auto;
    }
    .header__logo {
        font-family: "SeoulHangang CBL",  serif;
        text-decoration: none;
        font-size: 36px;
        text-shadow: 0px 7px 20px rgba(0, 0, 0, 0.45);
        line-height: 36px;
        letter-spacing: 0.105em;
    }
    .header__list {
        display: flex;
        list-style: none;
        transform: translateX(30%);
    }
    .header__list li:not(:last-child){
        margin-right: 30px;
    }
    .header__link {
        text-decoration: none;
        line-height: 22px;
        letter-spacing: 0.1em;
    }
    /* .active-link{
        color:#000000;
    } */
    .header__buttons {
        display: flex;
        align-items: center;
        list-style: none;
    }
    .header__buttons li{
        margin-left: 10px;
    }
    .header__button {
        padding: 9px 13px;
        border-radius: 100px;
        background: #FFB4A2;
        text-decoration: none;
        color: #4b4949;
        box-shadow: 0px 7px 20px 0px #FFB4A280;
        line-height: 22px;
        letter-spacing: 0.045em;
    }
    .header__button_cart{
        display: flex;
        align-items: center;
    }
    .header__button_cart img{
        margin-right: 10px;
        width: 24px;
        height: 24px;
    }
</style>