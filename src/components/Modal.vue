<template>
<div class="modal-background">
    <div class="modal-body">
        <div class='modal'>
            <div @click="handleModalClose" class="modal__cross">
                <img src='../assets/img/modal/close-form-button.png' alt='cross'/>
            </div>
            <div class="modal-content">
                <div class="modal-content__title">
                    LET’S DISCUSS<br/>
                    YOUR BUSINESS CASE!
                </div>
                <div class="modal-content__text">
                    Everything is possible! We will analyze your existing situation, discover the
                    bottlenecks and offer a solution that exactly matches your business case!
                </div>
                <div class="modal-content-mobile__text">
                    Everything is possible!
                </div>
                <div class="modal-content__action modal-action">
                    <div class="modal-action__inputs inputs">
                        <div class="inputs__first-name">
                            <label>First Name</label>
                            <input
                                type='text'
                                placeholder="Klaus"
                            />
                        </div>
                        <div class="inputs__last-name">
                            <label>Last Name</label>
                            <input
                                type='text'
                                placeholder="Voorman"
                            />
                        </div>
                        <div class="inputs__email">
                            <label>E-Mail</label>
                            <input
                                type='text'
                                placeholder="klaus.voormann@email.de"
                            />
                        </div>
                        <div class="inputs__text-area">
                            <label>Some brief description or comments</label>
                            <textarea
                                placeholder="My business case is completely different, so I want to discuss it with you."
                            />
                        </div>
                    </div>

                    <div class="modal-action__request-info">
                        By pressing the “request a consultation” button you
                        agree with <span>data protection</span> policy
                    </div>
                    <div class="modal-action__button">
                        <button>Request a Consultation</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
  name: 'Modal',
  methods: {
    handleModalClose () {
      this.$emit('close')
      document.body.style.overflow = ''
    }
  }
}
</script>

<style scoped lang="scss">
.modal-background {
    z-index: 3;
    position: fixed;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    backdrop-filter: blur(10px);
}

.modal-body {
    min-height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
}

.modal {
    width: 633px;
    margin: 0 auto;
    padding: 52px 52px 33px 52px;
    box-sizing: border-box;
    position: relative;

    box-shadow: 0 10px 30px 0 rgba(30, 30, 30, 0.25);
    background-image: linear-gradient(140deg, #fff, #efefef 100%);

    &__cross {
        position: absolute;
        top: 0;
        right: 0;
        width: 44px;
        height: 44px;
        cursor: pointer;
    }
}

.modal-content {
    width: 529px;

    &__title {
        width: 345px;
        margin-bottom: 20px;

        font-family: 'Catamaran', sans-serif;
        font-size: 25px;
        font-weight: 900;
        line-height: 1.2;
        letter-spacing: -0.63px;
    }

    &__text {
        font-family: 'Open Sans', sans-serif;
        font-size: 15px;
        line-height: normal;
        letter-spacing: -0.38px;

        margin-bottom: 50px;
    }

    &__action {
        padding-left: 12px;
        padding-right: 12px;
    }
}

.modal-action {
    &__request-info {
        width: 345px;
        font-family: 'Open Sans', sans-serif;
        font-size: 15px;
        letter-spacing: -0.38px;
        span {
            text-decoration: underline;
            font-weight: 600;
            cursor: pointer;
        }

        margin-bottom: 25px;
    }

    &__button {
        display: flex;
        justify-content: end;
        button {
            width: 240px;
            height: 44px;
            border-radius: 22px;
            border: none;
            cursor: pointer;
            background: rgba(8, 61, 119);

            font-family: 'Open Sans', sans-serif;
            font-size: 17px;
            font-weight: bold;
            letter-spacing: -0.43px;
            text-align: center;
            color: #fff;
        }
    }
}

.inputs {
    display: flex;
    flex-wrap: wrap;
        label {
            display: block;
            font-family: 'Open Sans', sans-serif;
            font-size: 13px;
            line-height: normal;
            letter-spacing: -0.33px;
            padding-left: 24px;
            height: 24px;
        }

        input {
            opacity: 0.25;
            font-family: 'Open Sans', sans-serif;
            font-size: 17px;
            letter-spacing: -0.43px;

            border-radius: 72px;
            border: 1px solid black;
            box-sizing: border-box;
            object-fit: contain;
            padding-left: 24px;
        }

    &__first-name {
        flex-wrap: wrap;
        width: 240px;
        margin-right: 24px;
        margin-bottom: 25px;
        input {
            width: 240px;
            height: 44px;
        }
    }

    &__last-name {
        flex-wrap: wrap;
        width: 240px;
        margin-bottom: 25px;
        input {
            width: 240px;
            height: 44px;
        }
    }

    &__email {
        flex-wrap: wrap;
        margin-bottom: 25px;
        width: 100%;
        input {
            width: 504px;
            height: 44px;
        }
    }

    &__text-area {
        flex-wrap: wrap;
        width: 100%;
        margin-bottom: 25px;
        textarea {
            opacity: 0.25;
            font-family: 'Open Sans', sans-serif;
            letter-spacing: -0.43px;
            font-size: 17px;

            border: 1px solid black;
            padding: 13px 24px;
            width: 504px;
            height: 132px;
            border-radius: 22px;
            box-sizing: border-box;
        }
    }
}

.modal-content-mobile__text {
    display: none;
}

@media (max-width: 380px) {
    .modal {
        width: 345px;
        padding: 44px 25px 38px 25px;
    }

    .modal-content {

        &__title {
            width: 295px;
            margin-bottom: 14px;

            font-size: 21px;
            font-weight: 900;
            line-height: 1;
            letter-spacing: -0.63px;
        }

        &__text {
            display: none;
        }

        &__action {
            padding-left: 0;
            padding-right: 0;
        }
    }

    .modal-content-mobile__text {
        display: block;
        margin-bottom: 20px;

        opacity: 0.75;
        font-family: 'Open Sans', sans-serif;
        font-size: 13px;
        line-height: normal;
        letter-spacing: -0.33px;
    }

    .modal-action {
        &__request-info {
            width: 295px;
            margin-bottom: 25px;
        }

        &__button{
            width: 295px;
            justify-content: center;
        }
    }

    .inputs {
        &__first-name {
            width: 295px;
            margin-bottom: 22px;
            input {
                width: 100%;
            }
        }

        &__last-name {
            width: 295px;
            margin-bottom: 22px;
            input {
                width: 100%;
            }
        }

        &__email {
            width: 295px;
            margin-bottom: 22px;
            input {
                width: 100%;
            }
        }

        &__text-area {
            width: 295px;
            textarea {
                width: 100%;
            }
        }
    }
}
</style>
