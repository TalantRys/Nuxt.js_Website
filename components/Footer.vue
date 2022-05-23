<template>
  <footer>
    <div class="footer__container container">
      <div class="footer__left">
        <nuxt-link to="/" exact class="footer__logo">Scake</nuxt-link>
        <div class="footer__list">
            <nuxt-link class="footer__link" to="#"><h3 class="footer__title">Главная</h3></nuxt-link>
          <div class="footer__links">
          <ul>
            <li><nuxt-link class="footer__link" to="#">Торты</nuxt-link></li>
            <li><nuxt-link class="footer__link" to="#">О нас</nuxt-link></li>
          </ul>
          <ul>
            <li><nuxt-link class="footer__link" to="#">Доставка</nuxt-link></li>
            <li>
              <nuxt-link class="footer__link" to="#"
                >Связаться с нами</nuxt-link
              >
            </li>
          </ul>
          </div>
        </div>
        <ul class="footer__list">
          <h3 class="footer__title">Контакты</h3>
          <li>
            <a href="tel:+73812999999" class="footer__link">+7-3812-99-99-99</a>
          </li>
          <li><a href="mailto:scake@mail.ru" class="footer__link">scake@mail.ru</a></li>
        </ul>
      </div>
      <div class="footer__right">
        <div class="footer__block">
          <div class="footer__social">
            <p class="social__title">Мы в соц. сетях:</p>
            <div class="social__block">
              <img src="~assets/images/icons/Social/vk.svg" alt="vk" />
              <img
                src="~assets/images/icons/Social/instagram.svg"
                alt="instagram"
              />
            </div>
          </div>
          <div class="footer__pay">
            <p class="pay__title">Платёжные системы:</p>
            <div class="pay__block">
              <img src="~assets/images/icons/Pay/visa.svg" alt="visa" />
              <img
                src="~assets/images/icons/Pay/mastercard.svg"
                alt="mastercard"
              />
              <img src="~assets/images/icons/Pay/maestro.svg" alt="maestro" />
              <img
                src="~assets/images/icons/Pay/apple-pay.svg"
                alt="apple-pay"
              />
              <img
                src="~assets/images/icons/Pay/google-pay.svg"
                alt="google-pay"
              />
            </div>
          </div>
        </div>
        <p class="footer__address">
          Адрес: г. Омск, ул. просп. Карла Маркса, 10
        </p>
      </div>
    </div>
    <div class="footer__bottom">
      <div class="footer__bottom_container container">
        <hr />
        <p class="footer__copyright">@2022 ИСП306 Рыскулов Талант</p>
      </div>
    </div>
  </footer>
</template>
<style>
footer {
  background-color: #6d6875;
  color: #fff;
}
footer p,
footer a {
  font-size: 14px;
  line-height: 17px;
  letter-spacing: 0.045em;
}
.footer__container {
  display: flex;
  justify-content: space-between;
  padding: 30px 0;
}
.footer__left,
.footer__right {
  display: flex;
  align-items: center;
}
.footer__left {
}
.footer__right {
  flex-direction: column;
  align-items: flex-start;
  justify-content: space-between;
}

.footer__bottom {
  text-align: center;
}
.footer__bottom_container {
  box-sizing: border-box;
  padding: 0 20px;
}
.footer__logo,
.footer__link {
  color: #fff;
}
.footer__logo {
  font-family: "SeoulHangang CBL", serif;
  text-decoration: none;
  font-size: 36px;
  text-shadow: 0px 7px 20px rgba(0, 0, 0, 0.45);
  line-height: 36px;
  letter-spacing: 0.105em;
  margin-right: 80px;
}

.footer__copyright {
  padding: 15px 0;
}
.footer__title{
  margin-bottom: 17px;
  font-weight: 600;
  font-size: 16px;
  line-height: 20px;
}
.footer__list {
  list-style: none;
}
.footer__list:not(:last-child){
  margin: 0 105px 0 0;
}
.footer__list li:not(:last-child) {
  margin-bottom: 20px;
}
.footer__links{
  display: flex;
}
.footer__links ul{
  list-style: none;
  margin-right: 30px;
}
.footer__link {
  text-decoration: none;
  line-height: 17px;
  letter-spacing: 0.045em;
}
.footer__block {
  display: flex;
}
.footer__social {
  margin-right: 58px;
}
.social__title {
  margin-bottom: 6px;
}
.pay__title {
  margin-bottom: 10px;
}
.footer__address{
  margin-top: 11px;
}
.social__block,
.pay__block {
  display: flex;
  align-items: center;
}
.social__block img:not(:last-child),
.pay__block img:not(:last-child) {
  margin-right: 10px;
}
</style>