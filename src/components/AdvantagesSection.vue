<template>
<section>
    <div class='wrapper row'>
        <div class='advantages col-6 offset-1'>
            <div class='advantages__title'>
                OUR ADVANTAGES
            </div>
            <div class='advantages__list-item'>
                <div class='item'>
                    <div class='item__dot'>
                        <img src='../assets/img/advantages/red-dot.png' alt='dot'/>
                    </div>
                    <div class='item__info info'>
                        <div class='info__title'>
                            System Integration
                        </div>
                        <div class='info__text'>
                            We help you with educating employees and
                            integrating software in your running processes
                        </div>
                    </div>
                </div>
                <div class='item'>
                    <div class='item__dot'>
                        <img src='../assets/img/advantages/red-dot.png' alt='dot'/>
                    </div>
                    <div class='item__info info'>
                        <div class='info__title'>
                            Technical support
                        </div>
                        <div class='info__text'>
                            We guarantee support and product maintenance
                            after release and keep improving the system in
                            cooperation with your team
                        </div>
                    </div>
                </div>
                <div class='item'>
                    <div class='item__dot'>
                        <img src='../assets/img/advantages/red-dot.png' alt='dot'/>
                    </div>
                    <div class='item__info info'>
                        <div class='info__title'>
                            Data security
                        </div>
                        <div class='info__text'>
                            Your data is stored on secure servers based in
                            Germany (or any other country on your request)
                        </div>
                    </div>
                </div>
                <div class='item'>
                    <div class='item__dot'>
                        <img src='../assets/img/advantages/red-dot.png' alt='dot'/>
                    </div>
                    <div class='item__info info'>
                        <div class='info__title'>
                            We speak your language
                        </div>
                        <div class='info__text'>
                            Our managers are German- and English-speaking,
                            so the business communication is clear and easy
                        </div>
                    </div>
                </div>
                <div class='item'>
                    <div class='item__dot'>
                        <img src='../assets/img/advantages/red-dot.png' alt='dot'/>
                    </div>
                    <div class='item__info info'>
                        <div class='info__title'>
                            Representative in Germany
                        </div>
                        <div class='info__text'>
                            Our business analyst is based in Frankfurt am Main.
                            Discussing all the business issues in person is much
                            more efficient
                        </div>
                    </div>
                </div>
                <div class='item'>
                    <div class='item__dot'>
                        <img src='../assets/img/advantages/red-dot.png' alt='dot'/>
                    </div>
                    <div class='item__info info'>
                        <div class='info__title'>
                            5 years experience in logistics
                        </div>
                        <div class='info__text'>
                            We’ve successfully implemented custom logistics/
                            transportation/stock and order management
                            systems
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class='advantages-mobile'>
            <div class='advantages-mobile__title'>
                OUR ADVANTAGES
            </div>
            <div class='advantages-mobile__list-item'>
                <div class='item-mobile'>
                    <div class='item-mobile__info-mobile info-mobile'>
                        <div class='info-mobile__title'>
                            System Integration
                        </div>
                    </div>
                    <div class='item-mobile__arrow'></div>
                </div>
                <div class='item-mobile'>
                    <div class='item__info-mobile info-mobile'>
                        <div class='info-mobile__title'>
                            Technical support
                        </div>
                    </div>
                    <div class='item-mobile__arrow'></div>
                </div>
                <div class='item-mobile'>
                    <div class='item-mobile__info info-mobile'>
                        <div class='info-mobile__title'>
                            Data security
                        </div>
                    </div>
                    <div class='item-mobile__arrow'></div>
                </div>
                <div class='item-mobile'>
                    <div class='item-mobile__info info-mobile'>
                        <div class='info-mobile__title'>
                            We speak your language
                        </div>
                    </div>
                    <div class='item-mobile__arrow'></div>
                </div>
                <div class='item-mobile'>
                    <div class='item-mobile__info info-mobile'>
                        <div class='info-mobile__title'>
                            Representative in Germany
                        </div>
                    </div>
                    <div class='item-mobile__arrow'></div>
                </div>
                <div class='item-mobile'>
                    <div class='item-mobile__info info-mobile'>
                        <div class='info-mobile__title'>
                            5 years experience in logistics
                        </div>
                    </div>
                    <div class='item-mobile__arrow'></div>
                </div>
            </div>
        </div>
        <div class='quotes col-5'>
            <div class='quotes__list'>
                <div class='quote'>
                    <div class='quote__text'>
                        Flawless communication with the Clockwise
                        Software team resulted in a fleet management
                        system that exactly met the needs of the municipal
                        waste transportation company. The software runs on
                        Android smartphones, so there was no need for
                        expensive equipment, and the learning curve was
                        low. We’ve implemented multi-tenancy to use this
                        software in other projects connected with logistics.
                    </div>
                    <div class='quote__person person'>
                        <div class='person__post'>
                            <span>Dan Weber</span><br>
                            CEO/CTO at Marketsoup
                        </div>
                        <div class='person__photo'>
                            <img src='../assets/img/advantages/person1.png' alt='person1'/>
                        </div>
                    </div>
                </div>
                <div class='quote'>
                    <div class='quote__text'>
                        With the automatic load scheduling and proper route
                        planning, we are finally able to use 100% of our truck
                        load capacity. Also, order management and delivery
                        have become much more efficient due to custom
                        modules. In the first year, we have covered our
                        investment in custom ERP system development
                    </div>
                    <div class='quote__person person'>
                        <div class='person__post'>
                            <span>Vadim Chabanenko</span><br>
                            Director at UDK Gazbeton
                        </div>
                        <div class='person__photo'>
                            <img src='../assets/img/advantages/person2.png' alt='person2'/>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
</template>

<script>
export default {
  name: 'AdvantagesSection'
}
</script>

<style scoped lang="scss">
section {
    max-width: 1440px;
    margin: 0 auto;
    margin-bottom: 248px;

    .wrapper {
        max-width: 1140px;
        margin: 0 auto;
        flex-wrap: nowrap;
    }

    .advantages {
        padding-left: 30px;
        &__title {
            display: flex;
            align-items: center;
            margin-bottom: 50px;
            height: 44px;

            font-family: 'Catamaran', sans-serif;
            font-size: 35px;
            font-weight: 900;
            line-height: 1;
            letter-spacing: -0.88px;
        }
    }

    .advantages-mobile {
        display: none;
    }

    .item {
        display: flex;
        margin-bottom: 26px;
        &:last-child {
            margin-bottom: 0px;
        }

        &__dot {
            width: 34px;
            height: 34px;
            margin-right: 43px;
        }
    }

    .info {

        &__title {
            font-family: 'Catamaran', sans-serif;
            font-size: 21px;
            font-weight: 900;
            letter-spacing: -0.53px;
        }

        &__text {
            padding-right: 113px;
            margin-top: -2px;

            opacity: 0.75;
            font-family: 'Open Sans', sans-serif;
            font-size: 15px;
            letter-spacing: -0.38px;
        }
    }

    .quotes {
        box-shadow: 0 10px 30px 0 rgba(0, 0, 0, 0.1);
        background-image: linear-gradient(140deg, #fff, #efefef);
        width: 633px;

        &__list {
            padding: 94px 158px 61px 24px;
        }
    }

    .quote {
        margin-bottom: 71px;
            &:last-child {
                .quote__text {
                    margin-bottom: 33px;
                }
                .person {
                    &__photo {
                        margin-right: 2px;
                    }
                }
            }

        &__text {
            font-family: 'Open Sans', sans-serif;
            font-size: 17px;
            font-weight: 600;
            letter-spacing: -0.43px;

            margin-bottom: 14px;
            padding-right: 22px;
        }

        &__person {
            display: flex;
            justify-content: end;
            align-items: center;
            text-align: right;
            padding-right: 22px;
        }
    }

    .person {
        &__post {
            margin-right: 15px;
            font-family: 'Open Sans', sans-serif;
            font-size: 15px;
            letter-spacing: -0.43px;

            span {
                font-size: 17px;
                font-weight: bold;
            }
        }

        &__photo {
            width: 44px;
            height: 44px;
        }
    }
}

@media (max-width: 768px) {
    section {
        margin-bottom: 117px;
        .wrapper {
            min-width: 768px;
            flex-wrap: wrap;
        }

        .advantages {
            padding-left: 15px;
            margin-bottom: 96px;

            &__title {
                margin-bottom: 47px;

                font-size: 25px;
                letter-spacing: -0.63px;
            }
        }

        .info {

            &__text {
                padding-right: 0;
                margin-right: -47px;
            }
        }

        .quotes {
            display: flex;
            justify-content: center;
            margin-left: 68px;

            &__list {
                padding: 91px 81px 0px 101px;
            }
        }
    }
}

@media (max-width: 375px) {
    section {
        margin-bottom: 93px;
        .wrapper {
            min-width: 375px;
        }

        .advantages {
            display: none;
        }

        .advantages-mobile {
            display: block;
            width: 345px;
            display: flex;
            align-items: center;
            flex-direction: column;
            margin: 0 auto;
            padding: 0;

            &__title {
                margin-bottom: 70px;
                width: 345px;

                font-family: 'Catamaran', sans-serif;
                font-size: 25px;
                font-weight: 900;
                line-height: 1;
                letter-spacing: -0.63px;
            }

            &__list-item {
                width: 375px;
                margin-bottom: 86px;
            }
        }

        .item-mobile {
            display: flex;
            justify-content: space-between;
            padding-right: 40px;
            padding-left: 15px;

            &__arrow {
                width: 24px;
                height: 24px;
                background-image: url('../assets/img/advantages/pin-left.png');
                background-position: center;
                background-size: auto auto;
                background-repeat: no-repeat;
                padding-bottom: 5px;
            }
        }

        .info-mobile {
            &__title {
                font-family: 'Catamaran', sans-serif;
                font-size: 21px;
                font-weight: 900;
                letter-spacing: -0.53px;

                margin-bottom: 22px;
            }
        }

        .quotes {
            width: 345px;
            margin: 0px 0px 0px 15px;

            &__list {
                width: 295px;
                padding: 26px 0px 0px 0px;
            }
        }

        .quote {
            margin-bottom: 50px;

            &:last-child {
                margin-bottom: 25px;
                .quote__text {
                    margin-bottom: 43px;
                }
                .person {
                    &__photo {
                        margin-right: 0px;
                    }
                }
            }

            &__text {
                font-size: 15px;
                font-weight: 600;
                letter-spacing: -0.38px;
                padding-right: 0;
            }

            &__person {
                padding-right: 0px;
            }
        }
    }
}

</style>
