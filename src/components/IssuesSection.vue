<template>
<section class='section'>
    <div class='content wrapper row'>
        <div class='content__title col-10 offset-1'>
            Have you experienced any of these issues?
        </div>

        <div class='content__cards offset-1'>
            <Carousel
                :breakpoints="breakpoints"
                :snapAlign = 'center-1-2'
                :items-to-show="2.5"
                :transition = "300"
                :wrapAround = "true"
            >
                <Slide v-for="slide in slides" :key="slide">
                    <div class='card'>
                        <div class='card__title'>
                            {{slide.title}}
                            <br>
                            {{slide.subTitle}}
                        </div>
                        <div class='card__text'>
                            {{slide.text}}
                        </div>
                    </div>
                </Slide>
                <template #addons>
                    <Pagination />
                    <Navigation />
                </template>
            </Carousel>
        </div>

    </div>
    <div class='wrapper row'>
        <div class='percent col-10 offset-1'>
            <div class='percent__text'>
                Expenses reduction after
                implementing logistics
                management software!
            </div>
            <div class='percent__img'>
            </div>
        </div>
    </div>
</section>
</template>

<script>
import { Carousel, Slide, Navigation, Pagination } from 'vue3-carousel'
import 'vue3-carousel/dist/carousel.css'
export default {
  name: 'IssuesSection',
  data: function () {
    return {
      slides: [
        {
          title: 'Overwhelming and',
          subTitle: 'inaccurate paperwork',
          text: `Most documents, such as orders, invoices,
                            contracts, etc. are stored in folders on endless
                            shelves. They are never easy to find.
                            Moreover, due to human factor, crucial
                            mistakes take place that cost your company
                            much time to solve, but also drain your
                            budget.`,
          key: 1
        },
        {
          title: 'Manual order management',
          subTitle: 'based on phone calls and emails',
          text: `Do your clients call you just to find out that
                            the necessary product is currently out of
                            stock? You waste resources by not providing
                            them with actual information about your
                            available inventory online`,
          key: 2
        },
        {
          title: 'Inefficient truck load',
          subTitle: '',
          text: `Without dynamic truck load
                            scheduling, your company misses up
                            to 50% of the potential loading
                            capability`,
          key: 3
        },
        {
          title: 'Overwhelming and',
          subTitle: 'inaccurate paperwork',
          text: `Most documents, such as orders, invoices,
                            contracts, etc. are stored in folders on endless
                            shelves. They are never easy to find.
                            Moreover, due to human factor, crucial
                            mistakes take place that cost your company
                            much time to solve, but also drain your
                            budget.`,
          key: 4
        },
        {
          title: 'Manual order management',
          subTitle: 'based on phone calls and emails',
          text: `Do your clients call you just to find out that
                            the necessary product is currently out of
                            stock? You waste resources by not providing
                            them with actual information about your
                            available inventory online`,
          key: 5
        },
        {
          title: 'Inefficient truck load',
          subTitle: '',
          text: `Without dynamic truck load
                            scheduling, your company misses up
                            to 50% of the potential loading
                            capability`,
          key: 6
        }
      ],
      breakpoints: {
        769: {
          itemsToShow: '2.5'
        },
        376: {
          itemsToShow: '1.95'
        },
        0: {
          itemsToShow: '1.001'
        }
      }
    }
  },
  components: {
    Carousel,
    Slide,
    Navigation,
    Pagination
  }
}
</script>

<style scoped lang="scss">

.section {
    max-width: 1440px;
    margin: 0 auto;
    padding: 52px 0 0 0;
    overflow: hidden;
    margin-bottom: 235px;

    .wrapper {
        max-width: 1140px;
        margin: 0 auto;
    }
    .content {
        &__title {
            display: flex;
            align-items: center;
            justify-content: right;
            margin-bottom: 168px;

            font-family: 'Catamaran', sans-serif;
            font-size: 35px;
            font-weight: 900;
            line-height: 1;
            letter-spacing: -0.88px;
            text-transform: uppercase;
        }

        &__cards {
            overflow: hidden;
            display: flex;
            flex-direction: row;
        }
    }
    .carousel__slide {
        min-width: 0;
    }
    .carousel {
        min-width: 0;
    }

    .prev {
        transform: scaleX(-1);
    }
    .card {
        height: 368px;
        min-width: 435px;
        max-width: 435px;
        padding: 67px 37px 68px 38px;
        background-color: #083d77;
        margin-right: 15px;
        box-sizing: border-box;
        text-align: start;
        &__title {
            height: 50px;
            font-family: 'Open Sans', sans-serif;
            font-size: 21px;
            font-weight: bold;
            line-height: 1.19;
            letter-spacing: -0.53px;
            color: #fff;
            margin-bottom: 22px;
        }
        &__text {
            font-family: 'Open Sans', sans-serif;
            font-size: 17px;
            letter-spacing: -0.43px;
            color: #fff;
            overflow: hidden;
        }
    }

    .action {
        display: flex;
        flex-direction: row;
        margin-bottom: 178px;

        &__arrows {
            display: flex;
            margin-right: 291px;
            img {
                height: 70px;
                width: 70px;
            }
        }

        &__dots {
            display: flex;
            align-items: center;
            justify-content: end;
            height: 70px;
            padding-right: 38px;
        }
    }

    .dot {
        width: 15px;
        height: 14px;
        margin-right: 16px;
        background-image: url('../assets/img/issue/selector-dot-2.png');

        &__active {
            background-image: url('../assets/img/issue/active-selector-dot.png');
        }

        &__adaptive {
            display: none;
        }
    }

    .percent {
        display: flex;
        justify-content: center;
        &__text {
            width: 345px;
            opacity: 0.75;
            font-family: 'Open Sans', sans-serif;
            font-size: 25px;
            line-height: 1.2;
            letter-spacing: -0.63px;
        }

        &__img {
            height: 100px;
            width: 346px;
            background-image: url('../assets/img/issue/49.png');
            background-size: cover;
            position: relative;
            top: -10px;
        }
    }
}

@media (max-width: 768px) {
    .section {
        min-width: 768px;
        margin-bottom: 130px;

        .wrapper {
            min-width: 768px;
        }

        .content {
            &__title {
                font-size: 25px;
                letter-spacing: -0.63px;

                justify-content: center;
                margin-bottom: 165px;
            }
        }

        .card {
            min-width: 375px;
            max-width: 375px;
            padding: 87px 15px;
            &__title {
                width: 345px;
            }
            &__text {
                font-size: 15px;
                letter-spacing: -0.38px;
            }
        }

        .action {
            margin-bottom: 164px;

            &__arrows {
                margin-right: 57px;
            }
        }

        .dot {
            &__adaptive {
                display: block;
            }
        }

        .percent {
            &__text {
                width: 258.6px;
                font-size: 18.8px;
                line-height: 1.2;
                letter-spacing: -0.47px;
            }

            &__img {
                height: 75.2px;
                width: 259.4px;
            }
        }
    }
}

@media (max-width: 380px) {
    .section {
        min-width: 375px;
        margin-bottom: 164.8px;

        .wrapper {
            min-width: 375px;
        }

        .content {
            &__title {
                justify-content: center;
                margin-bottom: 50px;
                text-align: right;
                width: 345px;
            }

            &__cards {
                justify-content: start;
                margin-left: 0;
                padding-left: 0;
                padding-right: 0;
            }
        }

        .card {
            height: 375px;
            min-width: 376px;
            max-width: 376px;
            padding: 92px 30px;

            &__title {
                line-height: 1;
                margin-bottom: 25px;
                width: 315px;
            }
        }

        .action {
            flex-direction: row-reverse;
            width: 345px;

            &__arrows {
                padding-left: 0;
                margin-right: -6px;
            }

            &__dots {
                &:last-child {
                    padding-right: 0;
                }
            }
        }

        .dot {
            &:last-child {
                margin-right: 39px;
            }
        }

        .percent {
            flex-wrap: wrap;

            &__text {
                font-size: 18.8px;
                letter-spacing: -0.47px;
                padding-bottom: 29.8px;
            }

            &__img {
                top: 0;
            }
        }
    }
}
</style>
