<template>
<section>
    <div class='content__scroll'>
        <a href='#advantages'>
            <img  src='../assets/img/logistics/scroll-down-arrow.png' alt='arrow'/>
            <span>Scroll to see our advantages</span>
        </a>
    </div>
    <div class='wrapper row'>
        <div class='benefit'>
            <img class='benefit__background' src='../assets/img/benefit/group.png' alt='background'/>
            <div class='benefit__title'>
                HOW CAN YOU BENEFIT FROM
                CUSTOM LOGISTICS SOFTWARE?
            </div>
            <div class='benefit__title_mobile'>
                LOGISTICS MANAGEMENT
                SOFTWARE DEVELOPMENT
            </div>
            <div class='benefit__list-item'>
                <div class='item'>
                    <div class='item__image'>
                        <img src='../assets/img/benefit/circle1.png' alt='circle1'/>
                    </div>
                    <div class='item__info info'>
                        <div class='info__title'>
                            Customized to your needs
                        </div>
                        <div class='info__text'>
                            A software is developed exclusively with your
                            needs and plans in mind. This enables to
                            solve unique problems efficiently
                        </div>
                    </div>
                </div>
                <div class='item'>
                    <div class='item__image'>
                        <img src='../assets/img/benefit/circle2.png' alt='circle2'/>
                    </div>
                    <div class='item__info info'>
                        <div class='info__title'>
                            Short-term ROI
                        </div>
                        <div class='info__text'>
                            You will experience the first returns right in
                            the first month after integrating the system in
                            your current processes
                        </div>
                    </div>
                </div>
                <div class='item'>
                    <div class='item__image'>
                        <img src='../assets/img/benefit/circle3.png' alt='circle3'/>
                    </div>
                    <div class='item__info info'>
                        <div class='info__title'>
                            Predictable scalability
                        </div>
                        <div class='info__text'>
                            A custom system grows along with your
                            business since your company goals are taken
                            into account in the development process
                        </div>
                    </div>
                </div>
                <div class='item'>
                    <div class='item__image'>
                        <img src='../assets/img/benefit/circle4.png' alt='circle4'/>
                    </div>
                    <div class='item__info info'>
                        <div class='info__title'>
                            Improve, not rebuild
                        </div>
                        <div class='info__text'>
                            Custom software supports and improves your
                            running processes step-by-step. Your current
                            system keeps working
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class='discuss col-12'>
            <div class='discuss__title'>
                YOUR BUSINESS CASE<br>
                IS COMPLETELY DIFFERENT?
                <span class='discuss__title_watermelon'>
                    LET’S DISCUSS
                </span>
            </div>
        </div>
        <div class='discuss col-12'>
            <div class='discuss__button'>
                <button @click="handleModalOpen()">
                    Fill in the contact form
                </button>
            </div>
        </div>
    </div>
</section>
</template>

<script>
export default {
  name: 'BenefitSection',
  methods: {
    handleModalOpen () {
      this.$emit('open')
      document.body.style.overflow = 'hidden'
    }
  }
}
</script>

<style scoped lang="scss">
section {
    max-width: 1440px;
    margin: 0 auto;
    margin-bottom: 175px;

    .content__scroll {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 207px;
        height: 36px;
        position: relative;
        top: 290px;
        left: -24px ;
        transform: rotate(-90deg);

        opacity: 0.5;
        font-family: 'Open Sans', sans-serif;
        font-size: 13px;
        font-weight: 300;
        letter-spacing: 0.16px;
        text-align: center;

        img {
            width: 20px;
            height: 20px;
            object-fit: contain;
            transform: rotate(90deg);
            position: relative;
            right: 22px;
        }

        a {
            display: flex;
            justify-content: space-between;
            align-items: center;
            min-width: 207px;
        }

    }

    .wrapper {
        max-width: 1140px;
        margin: 0 auto;
    }

    .benefit {
        height: 608px;
        padding: 44px 0 60px 88px;
        margin-bottom: 58px;
        margin-left: 7.5px;
        position: relative;

        &__background {
            position: absolute;
            z-index: -1;
            top: -2px;
            left: 0px;
        }

        &__title {
            font-family: 'Catamaran', sans-serif;
            font-size: 35px;
            font-weight: 900;
            line-height: 1;
            letter-spacing: -0.88px;

            padding-right: 400px;
            margin-bottom: 127px;
        }

        &__title_mobile {
            display: none;
        }

        &__list-item {
            display: flex;
            flex-wrap: wrap;
        }
    }

    .item {
        display: flex;
        width: 460px;
        height: 130px;
        margin-right: 68px;
        margin-bottom: 47px;
        &:nth-child(2n) {
            margin-right: 0px;
            width: 465px;
                }
        &:nth-child(3) {
            .item__info {
                .info__title {
                    margin-left: -7px;
                }
            }
        }

        &__image {
            width: 80px;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-right: 35px;
        }
    }

    .info {
        display: flex;
        flex-wrap: wrap;

        &__title {
            margin-bottom: 20px;

            font-family: 'Catamaran', sans-serif;
            font-size: 25px;
            font-weight: 900;
            letter-spacing: -0.63px;
            text-align: center;
        }

        &__text {
            opacity: 0.75;
            font-family: 'Open Sans', sans-serif;
            font-size: 17px;
            font-weight: 400;
            letter-spacing: -0.43px;
        }
    }

    .discuss {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        &__title {
            text-align: center;
            margin-bottom: 30px;
            width: 345px;

            font-family: 'Catamaran', sans-serif;
            font-size: 25px;
            font-weight: 900;
            line-height: 1.2;
            letter-spacing: -0.63px;

            &_watermelon {
                color: #ea5256;
            }
        }

        &__button {
            display: flex;
            justify-content: center;
            align-items: center;

            button {
                font-family: 'Catamaran', sans-serif;
                font-size: 21px;
                font-weight: 900;
                letter-spacing: -0.53px;
                text-align: center;
                color: #fff;
                object-fit: contain;

                width: 345px;
                height: 72px;
                border-radius: 72px;
                cursor: pointer;
                background: rgba(8, 61, 119);
                border: none;
            }
        }
    }
}

@media (max-width: 1340px) {
    section {
        .content__scroll {
            display: none;
        }

        .benefit {
            &__background {
                transform: rotate(-270deg);
                left: 1px;
                top: 1px;
            }
        }
    }
}

@media (max-width: 768px) {
    section {
        .wrapper {
            min-width: 768px;
        }

        .benefit {
            height: 955px;
            padding: 31px 0px 60px 50px;
            margin-bottom: 55px;

            &__background {
                top: 305px;
                left: -214px;
            }

            &__title {
                width: 585px;
                font-size: 25px;
                letter-spacing: -0.63px;
                padding-right: 132px;
                padding-left: 34px;
                box-sizing: border-box;
                margin-bottom: 116px;
            }
        }

        .item {
            margin-bottom: 46px;
        }

        .info {
            &__title {
                font-size: 21px;
                letter-spacing: -0.53px;

                padding-top: 7px;
                margin-bottom: -3px;
            }
        }

    }
}

@media (max-width: 391px) {
    section {
        margin-bottom: 170px;

        .wrapper {
            min-width: 375px;
        }

        .title_mobile {
            display: block;
        }

        .benefit {
            height: 955px;
            padding: 31px 0px 60px 50px;
            margin-bottom: 147px;

            &__background {
                top: 141px;
                left: -610px;
            }

            &__title {
                display: none;
            }

            &__title_mobile {
                font-family: 'Catamaran', sans-serif;
                font-weight: 900;
                line-height: 1;
                font-size: 25px;
                letter-spacing: -0.63px;

                width: 345px;
                padding-right: 0px;
                padding-left: 0px;
                margin-left: -42px;
                box-sizing: border-box;
                margin-bottom: 158px;
            }

            &__list-item {
                margin-left: -43px;
            }
        }

        .item {
            margin-bottom: 46px;
            &__image {
                margin-right: 31px;
            }
            &:nth-child(3) {
                .item__info {
                    .info__title {
                        margin-left: 0px;
                        margin-top: -20px;
                    }
                }
            }
        }

        .info {
            flex-wrap: wrap;
            padding-top: 34px;
            margin-bottom: 25px;
            &__title {
                font-size: 21px;
                letter-spacing: -0.53px;
                text-transform: uppercase;
                line-height: 1;

                width: 220px;
                text-align: left;
                margin-bottom: 10px;
            }

            &__text {
                width: 220px;
                font-size: 15px;
                letter-spacing: -0.38px;
            }
        }

        .discuss {
            &__title {
                font-size: 21px;
                line-height: 1.19;
                letter-spacing: -0.53px;
                width: 345px;
                padding: 0 20px;
                margin-bottom: 40px;
            }

            &__button {
                button {
                    height: 56px;
                    border-radius: 72px;
                }
            }
        }
    }
}
</style>
