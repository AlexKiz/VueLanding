<template>
<footer>
    <div class='wrapper row'>
        <div class='footer-content col-10 offset-1'>
            <div class='footer-text'>
                Data Protection / Imprint
            </div>
            <div class='footer-logo'>
                <div class='footer-logo__img'>

                </div>
                <div class='footer-logo__text'>
                    CLOCKWISE
                    <span>Software</span>
                </div>
            </div>
        </div>
    </div>
</footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped lang="scss">
footer {
    background-color: black;
    max-width: 1440px;
    margin: 0 auto;
    height: 104px;

    .wrapper {
        width: 1140px;
        margin: 0 auto;
    }

    .footer-content {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 40px 0 40px 0;
    }

    .footer-text {
        margin-left: 7.5px;
        width: 200px;
        font-family: 'Open Sans', sans-serif;
        font-size: 15px;
        font-weight: 600;
        letter-spacing: 0.12px;
        text-align: center;
        color: #fff;
    }

    .footer-logo {
        width: 118px;
        display: flex;
        justify-content: space-between;
        &__text {
            width: 88px;
            font-family: 'Catamaran', sans-serif;
            font-size: 10px;
            font-weight: 900;
            letter-spacing: 0.08px;
            line-height: 1;
            color: #fff;
            span {
                font-family: 'Open Sans', sans-serif;
                font-size: 8px;
                letter-spacing: 0.07px;
                color: #fff;
            }
        }
        &__img {
            background-image: url('../assets/img/footer/logo.png');
            background-size: cover;
            margin-left: -8px;
            width: 24px;
            height: 24px;
        }
    }
}

@media (max-width: 768px) {
    footer {
        .wrapper {
            max-width: 768px;
        }

        .footer-content {
            padding: 35px 0px 0px 20px;
        }

        .footer-logo{
            margin-top: 4px;
            margin-right: -28px;
            padding-top: 4px;
        }
    }
}

@media (max-width: 380px) {
    footer {
        height: 208px;
        width: 375px;
        .wrapper {
            max-width: 375px;
        }

        .footer-content {
            flex-wrap: wrap;
            padding: 65px 0px 0px 49px;
        }

        .footer-text {
            margin-bottom: 33px;
        }

        .footer-logo {
            margin-top: 0;
            padding-left: 15px;
        }
    }
}
</style>
