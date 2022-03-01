<template>
<section>
    <div class='wrapper row'>

        <div class='transport__title'>
            WHAT OUR PARTNERS HAVE ACHIEVED
            WITH CUSTOM TRANSPORT MANAGEMENT
            SOFTWARE
        </div>

        <div class='transport'>
            <div class='transport__carousel carousel'>
                <div class='carousel__action action'>
                    <div class='action__prev-arrow'>
                        <img src='../assets/img/transport/prev-button.png' alt='prev'/>
                    </div>
                    <div class='action__dots'>
                        <div class='dot dot_active'>
                            <img  src='../assets/img/transport/active-selector-dot.png' alt='dot'/>
                        </div>
                        <div class='dot dot_disabled'>
                            <img  src='../assets/img/transport/selector-dot.png' alt='dot'/>
                        </div>
                        <div class='dot dot_disabled'>
                            <img  src='../assets/img/transport/selector-dot.png' alt='dot'/>
                        </div>
                    </div>
                    <div class='action__next-arrow'>
                        <img src='../assets/img/transport/next-button.png' alt='next'/>
                    </div>
                </div>
                <div class='carousel__content'>
                    <div class='content'>
                        <div class='content__image'></div>
                        <div class='content__title'>
                            double truck day load capacity increase
                        </div>
                    </div>
                </div>
            </div>

            <div class='transport__info'>
                <div class='info-wrapper info'>
                    <div class='info__title'>
                        ERP system for construction
                        materials factory
                    </div>
                    <div class='info__text'>
                        Custom logistics software includes several
                        modules that enabled to fully digitalize a
                        factory<br>
                        – Order and stock management optimization<br>
                        – Automatic invoicing and accounting<br>
                        – Delivery scheduling and route planning<br>
                        – Automatic contractors selection<br><br>
                        Eliminating manual work enabled the factory
                        to double truck day load capacity (an increase
                        from 45 to 92 trucks per day) and save over
                        60.000 EUR in the first year.
                    </div>
                </div>
            </div>
        </div>

        <div class='discuss col-6 offset-3'>
            <div class='discuss__title'>
                Discuss your project with the professionals
            </div>
            <div class='discuss__button'>
                <button>
                    Let's discuss
                </button>
            </div>
            <div class='discuss__button-mobile'>
                <button>
                    Request&nbsp;&nbsp;a free consultation
                </button>
            </div>
        </div>
    </div>
</section>
</template>

<script>
export default {
  name: 'TransportManagementSection'
}
</script>

<style scoped lang="scss">
section {
    max-width: 1440px;
    margin: 0 auto;
    margin-bottom: 229px;

    .wrapper {
        max-width: 1140px;
        margin: 0 auto;
    }

    .transport__title {
        font-family: 'Catamaran', sans-serif;
        font-size: 35px;
        font-weight: 900;
        line-height: 1;
        letter-spacing: -0.88px;
        text-align: right;

        padding-left: 315px;
        padding-right: 105px;
        margin-bottom: 102px;
    }

    .transport {
        display: flex;
        padding-left: 140px;
        margin-bottom: 173px;

        &__carousel {
            width: 531px;
        }

        &__info {
            padding: 152px 20px 3px 18px;
        }
    }

    .carousel {
        &__action {
            display: flex;
            justify-content: end;
        }
    }

    .action {
        &__dots {
            display: flex;
            align-items: center;
            justify-content: space-between;
            width: 81px;
            margin-left: 58px;
        }

        &__next-arrow {
            margin-left: 60px;
            margin-right: 15px;
        }
    }

    .content {

        &__image {
            width: 483px;
            height: 498px;
            background-image: url('../assets/img/transport/carousel-image1.png');
            margin-top: -2px;
            margin-left: -28px;
            margin-bottom: 5px;

            padding-right: 10px;
        }

        &__title {
            width: 345px;
            padding-left: 46px;

            font-family: 'Open Sans', sans-serif;
            font-size: 15px;
            font-weight: bold;
            letter-spacing: -0.38px;
            text-align: center;
            text-transform: uppercase;
        }
    }

    .info {
        width: 345px;
        margin-bottom: 10px;

        &__title {
            font-family: 'Catamaran', sans-serif;
            font-size: 25px;
            font-weight: 900;
            line-height: 1.2;
            letter-spacing: -0.63px;

            margin-bottom: 10px;
        }

        &__text {
            font-family: 'Open Sans', sans-serif;
            font-size: 17px;
            letter-spacing: -0.43px;
        }
    }

    .discuss {
        &__title {
            font-family: 'Catamaran', sans-serif;
            font-size: 17px;
            font-weight: 900;
            line-height: 1.24;
            letter-spacing: -0.43px;
            text-align: center;
            text-transform: uppercase;

            margin-bottom: 44px;
            width: 345px;
            padding-left: 105px;
        }

        &__button {
            display: flex;
            justify-content: center;

            button {
                font-family: 'Catamaran', sans-serif;
                font-size: 21px;
                font-weight: 900;
                letter-spacing: -0.53px;
                text-align: center;
                color: #fff;
                border-radius: 72px;

                width: 345px;
                height: 72px;
                border-radius: 72px;
                cursor: pointer;
                background: rgba(8, 61, 119);
                border: none;
            }
        }

        &__button-mobile {
            display: none;
        }
    }
}

@media (max-width: 768px) {
    section {
        margin-bottom: 102px;
        .wrapper {
            min-width: 768px;
        }

        .transport {
            padding-left: 70px;
            margin-bottom: 255px;

            &__carousel {
                width: 345px;
            }

            &__info {
                padding: 117px 0px 0px 9px;
            }
        }

        .transport__title {
            font-family: 'Catamaran', sans-serif;
            font-size: 25px;
            font-weight: 900;
            line-height: 1;
            letter-spacing: -0.63px;
            text-align: right;

            padding-left: 145px;
            padding-right: 91px;
            margin-bottom: 95px;
        }

        .carousel {
            &__action {
                justify-content: start;
            }
        }

        .action {
            margin-left: -11px;
        }

        .content {
            &__image {
                width: 345px;
                height: 366px;
                background-image: url('../assets/img/transport/carousel-image1Tablet.png');
                background-repeat: no-repeat;
            }

            &__title {
                margin-left: -90px;
                padding-left: 72px;
            }
        }

        .info {
            &__title {
                font-size: 21px;
                line-height: 1;
                letter-spacing: -0.53px;

                margin-bottom: 23px;
            }

            &__text {
                font-size: 15px;
                letter-spacing: -0.38px;
                padding-right: 16px;
            }
        }

        .discuss {
            &__title {
                padding-left: 15px;
            }
        }
    }
}

@media (max-width: 375px) {
    section {
        margin-bottom: 77px;
        .wrapper {
            min-width: 375px;
        }

        .transport {
            flex-direction: column-reverse;
            padding-left: 15px;
            margin-bottom: 290px;

            &__info {
                padding: 40px 0px 0px 9px;
                margin-bottom: 36px;
            }
        }

        .transport__title {
            padding-left: 0;
            padding-right: 15px;
            margin-bottom: 10px;
        }

        .action {
            margin-left: -2px;

            &__dots {
                margin-left: 64px;
                margin-right: 60px;
            }

            &__next-arrow {
                margin-right: 0px;
                padding-left: 0px;
                margin-left: 1px;
            }
        }

        .content {
            &__image {
                padding-right: 0;
                margin-left: -13px;
            }

            &__title {
                margin-left: -74px;
            }
        }

        .discuss {
            &__title {
                margin-left: -101px;
            }

            &__button {
                display: none;
            }

            &__button-mobile {
                display: flex;
                justify-content: center;

                margin-right: -85px;
                margin-left: -85px;
                button {
                    font-family: 'Catamaran', sans-serif;
                    font-size: 21px;
                    font-weight: 900;
                    letter-spacing: -0.53px;
                    text-align: center;
                    color: #fff;
                    border-radius: 72px;

                    width: 345px;
                    height: 56px;
                    border-radius: 72px;
                    cursor: pointer;
                    background: rgba(8, 61, 119);
                    border: none;
                }
            }
        }
    }
}
</style>
