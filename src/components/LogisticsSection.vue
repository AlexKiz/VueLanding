<template>
    <section class='section'>
            <div class='section__content content'>
                <div class='content__scroll'>
                    <a href='#benefit'>
                        <img  src='../assets/img/logistics/scroll-down-arrow.png' alt='arrow'/>
                        <div class='content__scroll_text'>
                            Scroll for more information
                        </div>
                    </a>
                </div>
                <div class='content__info'>
                    <div class='content__title'>
                        LOGISTICS MANAGEMENT
                        SOFTWARE DEVELOPMENT
                    </div>
                    <div class='content__text'>
                        We solve transportation and stock management problems
                        for Factories, Manufacturers, Carriers, Resellers, E-commerce
                        and even more.<span> Any issue can be solved with smart
                        digitalization.</span>
                    </div>
                    <div class='content__button'>
                        <button @click="handleModalOpen()">
                            <span>Request&nbsp;&nbsp;a free consultation</span>
                        </button>
                    </div>
                </div>
                <div class='content__img'>
                </div>
            </div>
    </section>
</template>

<script>
export default {
  name: 'LogisticsSectionTest',
  methods: {
    handleModalOpen () {
      this.$emit('open')
      document.body.style.overflow = 'hidden'
    }
  }
}
</script>

<style scoped lang="scss">
.section {
    max-width: 1440px;
    margin: 0 auto;

    margin-bottom: 168px;
}

.content {
    display: flex;
    justify-content: space-between;
    align-items: center;

    &__info {
        width: 710px;
        margin-top: -8px;
    }

    &__scroll{
        display: flex;
        justify-content: space-between;
        align-items: center;
        min-width: 207px;
        transform: rotate(-90deg);
        margin: 39px -20px 0 -40px;
        cursor: pointer;
        a {
            display: flex;
            justify-content: space-between;
            align-items: center;
            min-width: 207px;
        }

        &_text {
            opacity: 0.5;
            font-family: 'Open Sans', sans-serif;
            font-size: 13px;
            font-weight: 300;
            letter-spacing: 0.16px;
            text-align: center;

        }

        img {
            object-fit: contain;
            transform: rotate(90deg);
        }
    }

    &__title {
        font-family: 'Catamaran', sans-serif;
        font-size: 55px;
        font-weight: 900;
        line-height: 1;
        letter-spacing: -1.38px;

        margin-bottom: 49px;
    }

    &__text {
        width: 568px;
        text-align: start;
        margin-bottom: 62px;

        font-family: 'Open Sans', sans-serif;
        font-size: 21px;
        letter-spacing: -0.53px;
        color: #1a1d1a;
    }

    &__button {
        display: flex;
        justify-content: end;
        align-items: center;
        padding-right: 70px;

        button {
            font-family: 'Catamaran', sans-serif;
            font-size: 21px;
            font-weight: 900;
            letter-spacing: -0.53px;
            text-align: center;
            color: #fff;

            width: 345px;
            height: 72px;
            border-radius: 72px;
            cursor: pointer;
            background: rgba(8, 61, 119);
            border: none;
        }
    }

    &__img {
        width: 415px;
        height: 522px;
        background-image: url('../assets/img/logistics/decorative-routes-thing.png');
        background-size: cover;
    }
}

@media (max-width: 912px) {

    .content {
        &__scroll {
            margin: 100px -50px 0 -50px;
        }
    }
}

@media (max-width: 768px) {
    .section {
        min-width: 768px;
        margin-bottom: 74px;
    }

    .content {

        &__info {
            width: 452px;
        }

        &__scroll {
            margin: 23px -7px 0 -70px;
        }

        &__title {
            font-size: 35px;
            letter-spacing: -0.88px;

            margin-bottom: 68px;
        }

        &__text {
            font-size: 17px;
            letter-spacing: -0.43px;

            width: 452px;
            margin-bottom: 87px;
        }

        &__button {
            padding-right: 25px;
        }

        &__img {
            min-width: 195px;
            min-height: 522px;
            background-image: url('../assets/img/logistics/decorative-routes-thingTablet.png');
            background-size: cover;
            position: relative;
            top: -78px;
            left: -17px;
        }
    }
}

@media (max-width: 380px) {
    .section {
        min-width: 375px;
        margin-bottom: -190px;
    }

        .content {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;

        &__info {
            width: 325px;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }

        &__scroll {
            display: none;
        }

        &__title {
            font-size: 30px;
            letter-spacing: -0.75px;

            margin-bottom: 50px;
        }

        &__text {
            width: 325px;
            margin-bottom: 50px;

            span {
                display: block;
            }
        }

        &__button {
            padding-right: 0;
            z-index: 2;

            button {
                width: 345px;
                height: 57px;
            }
        }

        &__img {
            width: 178px;
            max-height: 363px;
            background-image: url('../assets/img/logistics/decorative-routes-thingMobile.png');
            background-repeat: no-repeat;
            background-size: auto;
            top: -66px;
            left: 99px;
        }
    }
}
</style>
