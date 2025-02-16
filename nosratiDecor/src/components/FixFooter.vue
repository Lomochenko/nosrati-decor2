<script setup>
// import { RouterLink } from 'vue-router';

</script>

<template>
  <!-- footer -->
  <footer class="footer" dir="rtl">
    <div class="container">
      <div class="footer-links p-relative">
        <div class="row">
          <div class="col-md-3 dsn-col-footer">
            <div class="footer-block">
              <div class="footer-logo">
                <a href=""><img src="assets/img/logo.png" alt=""></a>
              </div>

              <div class="footer-social">

                <ul>
                  <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
                  <li><a href="#"><i class="fab fa-behance"></i></a></li>
                  <li><a href="#"><i class="fab fa-instagram"></i></a></li>
                  <li><a href="#"><i class="fab fa-twitter"></i></a></li>

                </ul>

              </div>
            </div>
          </div>

          <div class="col-md-3 dsn-col-footer">
            <div class="footer-block col-menu">
              <h4 class="footer-title">Navigation</h4>
              <nav>
                <ul>
                  <li><a href="#">Portfolio</a>
                  </li>
                  <li><a href="#">About</a></li>
                  <li><a href="#">News</a></li>
                  <li><a href="#">Contact</a>
                  </li>
                </ul>
              </nav>
            </div>
          </div>

          <div class="col-md-3 dsn-col-footer" dir="rtl">
            <div class="footer-block col-contact">
              <h4 class="footer-title">Contact</h4>
              <ul>
                <li class="d-flex flex-md-column align-items-md-start align-items-center justify-content-between">
                  <span>Phone</span>
                  <a href="#">+1 (800) 990 8877</a>
                </li>
                <li
                  class="d-flex flex-md-column align-items-md-start justify-content-md-end align-items-center justify-content-between">
                  <span>Instagram</span>
                  <a href="#">NosratiDecor</a>
                </li>
              </ul>
            </div>
          </div>

          <div class="col-md-3 dsn-col-footer">
            <div class="col-address">
              <h4 class="footer-title">Address</h4>

              <p>El-Mahalla El-Kubra 37<br>
                1776 Damietta<br>
                Egypt</p>
            </div>
          </div>
        </div>
      </div>
      <!-- credit -->
      <div class="copyright" dir="ltr">
        <div class="text-center">
          <p>© 2025 Pesteh Tech Digital Agency</p>
          <div class="copright-text over-hidden">Designed by <a class="link-hover" data-hover-text="DSN Grid" href="#"
              target="_blank">Pesteh Tech</a>
          </div>
        </div>
      </div>
      <!-- end credit -->
    </div>
  </footer>
  <!-- end footer -->
</template>

<style scoped>
/** === Footer menu === */
.footer-navigation {
  display: inline;
}

.footer-navigation>div {
  display: inline;
}

.footer-navigation .footer-menu {
  display: inline;
  padding-left: 0;
}

.footer-navigation .footer-menu li {
  display: inline;
  margin-right: 1rem;
}

/* -------------------------------------------------------
                   Footer
-------------------------------------------------------- */
footer {
  position: relative;
  z-index: 3;
  padding: 0 50px 30px;
}

@media only screen and (max-width: 767px) {
  footer {
    margin-left: 0;
    padding: 0 30px 30px 30px;
  }
}

@media only screen and (max-width: 575px) {
  footer {
    padding-left: 15px;
  }
}

footer a,
footer p {
  color: rgba(194, 194, 194, 0.6);
  margin-bottom: 0;
  font-size: 1rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 4px;
  line-height: 1.6;
  font-variant-numeric: proportional-nums;
  font-family: "Montserrat", sans-serif;
}

footer span {
  font-size: 1rem;
  font-weight: 700;
  text-transform: uppercase;
  font-family: "Montserrat", sans-serif;
  line-height: 1.6;
  margin-bottom: .2rem;
}

.v-light footer a,
.v-light footer p {
  color: #0009;
}

@media only screen and (max-width: 767px) {

  footer a,
  footer p {
    letter-spacing: 0;
  }
}

footer .contact-footer {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  -webkit-box-pack: start;
  -ms-flex-pack: start;
  justify-content: flex-start;
  margin-bottom: 10px;
}

footer .contact-footer .phone {
  margin-right: 30px;
}

footer .copyright-social {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
  -ms-flex-direction: row;
  flex-direction: row;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
}

@media only screen and (max-width: 767px) {
  footer .copyright-social {
    -webkit-box-align: start;
    -ms-flex-align: start;
    align-items: start;
    -webkit-box-orient: inherit;
    -webkit-box-direction: inherit;
    -ms-flex-direction: inherit;
    flex-direction: inherit;
  }
}

@media only screen and (max-width: 575px) {
  footer .copyright-social {
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
  }
}

@media only screen and (max-width: 767px) {
  footer .copyright-social p {
    -webkit-box-ordinal-group: 3;
    -ms-flex-order: 2;
    order: 2;
  }
}

footer .copyright-social ul {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

@media only screen and (max-width: 767px) {
  footer .copyright-social ul {
    margin-top: 0;
    margin-bottom: 10px;
  }
}

footer .copyright-social ul li {
  display: list-item;
  margin-right: 20px;
  list-style: none;
}

footer .copyright-social ul li:last-child {
  margin-right: 0;
}

.footer {
  background-color: #090909;
}

.v-light .footer {
  background-color: #e6e6e6;
}

.footer .footer-links {
  padding-top: 80px;
  padding-bottom: 80px;
}

@media only screen and (max-width: 767px) {
  .footer .footer-links .dsn-col-footer:nth-of-type(n+2) {
    margin-top: 30px;
  }
}

.footer .footer-links .footer-title {
  position: relative;
  color: #fff;
  text-transform: uppercase;
  font-weight: 700;
  /* font-size: 1rem; */
  padding-bottom: 10px;
  margin-bottom: 25px;
  letter-spacing: 2px;
}

.v-light .footer .footer-links .footer-title {
  color: #000;
}

.footer .footer-links .footer-title::after {
  content: "";
  position: absolute;
  right: 0;
  bottom: 0;
  width: 15px;
  height: 2px;
  background-color: #fff;
}

.v-light .footer .footer-links .footer-title::after {
  background-color: #000;
}

.footer .footer-links .footer-block.col-menu ul li {
  font-size: 14px;
  font-weight: 600;
  margin-bottom: 10px;
  overflow: hidden;
}

.footer .footer-links .footer-block.col-menu ul li:last-of-type {
  margin-bottom: 0;
}

.footer .footer-links .footer-block.col-menu ul li a {
  font-weight: 600;
}

.footer .footer-links .footer-block.col-contact p {
  /* font-size: 12px; */
  font-weight: 600;
  margin-bottom: 10px;
}

.footer .footer-links .footer-block.col-contact p strong {
  color: #fff;
}

.v-light .footer .footer-links .footer-block.col-contact p strong {
  color: #000;
}

.footer .footer-links .footer-block.col-contact p span {
  margin-right: 5px;
  margin-left: 5px;
}

.footer .footer-links .footer-block .footer-logo {
  width: 90px;
}

.footer .footer-links .footer-block .footer-social {
  margin-top: 20px;
}

.footer .footer-links .footer-block .footer-social ul li {
  display: inline-block;
  list-style: none;
  margin-right: 5px;
}

.footer .footer-links .footer-block .footer-social ul li:last-child {
  margin-right: 0;
}

.footer .footer-links .footer-block .footer-social ul li a {
  position: relative;
  color: #fff;
  border-radius: 50%;
  letter-spacing: 0;
  border: 1px solid rgba(255, 255, 255, 0.5);
  height: 35px;
  width: 35px;
  line-height: 35px;
  text-align: center;
  -webkit-transition: -webkit-transform 0.2s ease-in-out;
  transition: -webkit-transform 0.2s ease-in-out;
  -o-transition: transform 0.2s ease-in-out;
  transition: transform 0.2s ease-in-out;
  transition: transform 0.2s ease-in-out, -webkit-transform 0.2s ease-in-out;
}

.v-light .footer .footer-links .footer-block .footer-social ul li a {
  color: #000;
  border: 1px solid #bebebe;
}

.footer .footer-links .footer-block .footer-social ul li a i {
  position: relative;
  z-index: 2;
  -webkit-transition: -webkit-transform 0.2s ease-in-out;
  transition: -webkit-transform 0.2s ease-in-out;
  -o-transition: transform 0.2s ease-in-out;
  transition: transform 0.2s ease-in-out;
  transition: transform 0.2s ease-in-out, -webkit-transform 0.2s ease-in-out;
}

.footer .footer-links .footer-block .footer-social ul li a:before {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  opacity: 0;
  border-radius: 50%;
  -webkit-transform: scale(0);
  -ms-transform: scale(0);
  transform: scale(0);
  background-color: #fff;
  -webkit-transform-origin: center center;
  -ms-transform-origin: center center;
  transform-origin: center center;
  -webkit-transition: opacity 0.3s cubic-bezier(0.215, 0.61, 0.355, 1), -webkit-transform 0.3s cubic-bezier(0.215, 0.61, 0.355, 1);
  transition: opacity 0.3s cubic-bezier(0.215, 0.61, 0.355, 1), -webkit-transform 0.3s cubic-bezier(0.215, 0.61, 0.355, 1);
  -o-transition: transform 0.3s cubic-bezier(0.215, 0.61, 0.355, 1), opacity 0.3s cubic-bezier(0.215, 0.61, 0.355, 1);
  transition: transform 0.3s cubic-bezier(0.215, 0.61, 0.355, 1), opacity 0.3s cubic-bezier(0.215, 0.61, 0.355, 1);
  transition: transform 0.3s cubic-bezier(0.215, 0.61, 0.355, 1), opacity 0.3s cubic-bezier(0.215, 0.61, 0.355, 1), -webkit-transform 0.3s cubic-bezier(0.215, 0.61, 0.355, 1);
}

.v-light .footer .footer-links .footer-block .footer-social ul li a:before {
  background-color: #000;
}

.footer .footer-links .footer-block .footer-social ul li a:hover i {
  color: #000;
  -webkit-transform: rotate(360deg);
  -ms-transform: rotate(360deg);
  transform: rotate(360deg);
}

.v-light .footer .footer-links .footer-block .footer-social ul li a:hover i {
  color: #fff;
}

.footer .footer-links .footer-block .footer-social ul li a:hover:before {
  opacity: 1;
  -webkit-transform: scale(1);
  -ms-transform: scale(1);
  transform: scale(1);
  -webkit-transition: opacity 0.5s cubic-bezier(0.215, 0.61, 0.355, 1) 0.2s, -webkit-transform 0.5s cubic-bezier(0.23, 1, 0.32, 1) 0.2s;
  transition: opacity 0.5s cubic-bezier(0.215, 0.61, 0.355, 1) 0.2s, -webkit-transform 0.5s cubic-bezier(0.23, 1, 0.32, 1) 0.2s;
  -o-transition: transform 0.5s cubic-bezier(0.23, 1, 0.32, 1) 0.2s, opacity 0.5s cubic-bezier(0.215, 0.61, 0.355, 1) 0.2s;
  transition: transform 0.5s cubic-bezier(0.23, 1, 0.32, 1) 0.2s, opacity 0.5s cubic-bezier(0.215, 0.61, 0.355, 1) 0.2s;
  transition: transform 0.5s cubic-bezier(0.23, 1, 0.32, 1) 0.2s, opacity 0.5s cubic-bezier(0.215, 0.61, 0.355, 1) 0.2s, -webkit-transform 0.5s cubic-bezier(0.23, 1, 0.32, 1) 0.2s;
}

/* .footer .footer-links .footer-block .footer-social ul li a i {
  font-size: 12px;
} */

.footer .copyright {
  padding-top: 30px;
  font-size: 14px;
  letter-spacing: 2.67px;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
}

.v-light .footer .copyright {
  border-top: 1px solid #bebebe;
}

.footer .copyright p {
  text-transform: uppercase;
}

.footer .copyright .copright-text {
  color: #a7a7a7;
  margin-top: 5px;
  font-weight: 500;
}

.footer .copyright .copright-text a {
  color: #fff;
}

.v-light .footer .copyright .copright-text a {
  color: #000;
}

.cap {
  position: absolute;
  bottom: 30px;
  left: 0;
  background-image: -webkit-gradient(linear, left top, right top, from(#0e0e0e5c), to(#1b1515));
  background-image: -webkit-linear-gradient(left, #0e0e0e5c 0%, #1b1515 100%);
  background-image: -o-linear-gradient(left, #0e0e0e5c 0%, #1b1515 100%);
  background-image: linear-gradient(to right, #0e0e0e5c 0%, #1b1515 100%);
  padding: 4px 15px;
  color: #fff;
  z-index: 10;
}

.cap span {
  font-size: 12px;
  text-transform: uppercase;
  letter-spacing: 2px;
}

.caption {
  left: -20px;
  bottom: 0px;
  -webkit-transform: rotate(-90deg);
  -ms-transform: rotate(-90deg);
  transform: rotate(-90deg);
  -webkit-transform-origin: left center;
  -ms-transform-origin: left center;
  transform-origin: left center;
  color: #fff;
  letter-spacing: 2px;
  font-size: 12px;
  font-weight: 600;
  position: absolute;
}

.v-light .caption {
  color: #000;
}
</style>