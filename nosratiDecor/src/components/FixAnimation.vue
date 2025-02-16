<template>
    <!-- hover animation -->
    <section class="contact-up section-margin section-padding">
        <div class="container">
            <div class="c-wapp">

                <span class="hiring">
                    Nosrati Decor
                </span>
                <span class="career">
                    Make your ideal design for your place!
                </span>

            </div>
        </div>
    </section>
    <!-- end hover animation -->
</template>

<style scoped>
.contact-up {
  position: relative;
  background-color: #090909;
  overflow: hidden;
}

.v-light .contact-up {
  background-color: #e6e6e6;
}

.contact-up::before {
  width: 0%;
  height: 100%;
  left: 0;
  top: 0;
  position: absolute;
  background-color: #000;
  content: "";
  -webkit-transition: width 0.5s cubic-bezier(0.77, 0, 0.175, 1);
  -o-transition: width 0.5s cubic-bezier(0.77, 0, 0.175, 1);
  transition: width 0.5s cubic-bezier(0.77, 0, 0.175, 1);
}

.v-light .contact-up::before {
  background-color: #f9f9f9;
}

.contact-up .c-wapp {
  width: 100%;
  display: table;
}

.contact-up .c-wapp {
  width: 100%;
  height: 100%;
  position: relative;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
  -ms-flex-flow: row;
  flex-flow: row;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  overflow: hidden;
}

@media only screen and (max-width: 767px) {
  .contact-up .c-wapp {
    -ms-flex-flow: wrap;
    flex-flow: wrap;
  }
}

.contact-up .c-wapp .hiring {
  width: 50%;
  position: relative;
  display: block;
  text-align: left;
  font-size: 42px;
  font-weight: 800;
  line-height: 1.2;
  letter-spacing: 0.01em;
  color: transparent;
  -webkit-text-stroke: 1px #fff;
  text-transform: uppercase;
  -webkit-transition: color 0.5s cubic-bezier(0.77, 0, 0.175, 1);
  -o-transition: color 0.5s cubic-bezier(0.77, 0, 0.175, 1);
  transition: color 0.5s cubic-bezier(0.77, 0, 0.175, 1);
}

.v-light .contact-up .c-wapp .hiring {
  -webkit-text-stroke: 1px #000;
}

@media only screen and (max-width: 767px) {
  .contact-up .c-wapp .hiring {
    display: block;
    text-align: center;
    width: 100%;
    -webkit-box-ordinal-group: 3;
    -ms-flex-order: 2;
    order: 2;
  }
}

@media only screen and (max-width: 400px) {
  .contact-up .c-wapp .hiring {
    font-size: 28px;
  }
}

.contact-up .c-wapp .career {
  color: #fff;
  width: 50%;
  position: relative;
  display: block;
  text-align: right;
  font-size: 1rem;
  font-weight: 600;
  margin-top: 10px;
}

.v-light .contact-up .c-wapp .career {
  color: #000;
}

@media only screen and (max-width: 767px) {
  .contact-up .c-wapp .career {
    display: block;
    text-align: center;
    width: 100%;
    margin-top: 0;
    margin-bottom: 15px;
  }
}

.contact-up:hover::before {
  width: 100%;
}

.contact-up:hover .hiring {
  color: #fff;
}

.v-light .contact-up:hover .hiring {
  color: #000;
}
</style>