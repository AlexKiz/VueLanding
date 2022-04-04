<template>
<header class='header'>
    <div class='header__container'>
        <div class='header__logo'>
        </div>
        <nav class='header__menu menu'>
            <li class='menu__item'>Benefits</li>
            <li class='menu__item'>Advantages</li>
            <li class='menu__item'>Achievements</li>
        </nav>
        <div class='header__language language'>
            <li class='language__item language__item_opacity'>DE</li>
            <li class='language__item'>EN</li>
        </div>
        <div class='header__menu-mobile' @click="isOpen()">
            <img v-if="menuMobileOpen" src='../assets/img/header/menu-close.png' alt='menu'/>
            <img v-else src='../assets/img/header/menuMobile.png' alt='menu'/>
        </div>
    </div>
    <div v-if="menuMobileOpen" class='menu-mobile'>
        <div class='menu-mobile__item'>
            Benefits
        </div>
        <div class='menu-mobile__item'>
            Advantages
        </div>
        <div class='menu-mobile__item'>
            Achievements
        </div>
        <div class='menu-mobile__item'>
            Imprint and Data protection
        </div>
        <div class='menu-mobile__language language-mobile'>
            <div class='language-mobile__text'>Language</div>
            <div class='language-mobile__lang'>
                <div class='language-mobile__lang_item language-mobile_opacity'>DE</div>
                <div class='language-mobile__lang_item'>EN</div>
            </div>
        </div>
        <div  class='menu-mobile__button'>
            <button @click="handleModalOpen()">Request&nbsp;&nbsp;a free consultation</button>
        </div>
    </div>
</header>
</template>

<script>
export default {
  name: 'HeaderTest',
  data () {
    return {
      menuMobileOpen: false
    }
  },
  methods: {
    isOpen () {
      if (this.menuMobileOpen) {
        this.menuMobileOpen = false
        document.body.style.overflow = ''
      } else {
        this.menuMobileOpen = true
        document.body.style.overflow = 'hidden'
      }
    },
    handleModalOpen () {
      this.$emit('open')
      document.body.style.overflow = 'hidden'
    }
  }
}
</script>

<style scoped lang="scss">
.header {
    font-family: 'Open Sans', sans-serif;
    font-size: 17px;
    font-weight: 600;
    letter-spacing: 0.13px;
    font-stretch: normal;

    max-width: 1440px;
    margin: 0 auto;
    padding: 40px 0px 40px 53px;
    box-sizing: border-box;
    margin-bottom: 115px;

    &__container {
        box-sizing: border-box;
        max-width: 1166px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    &__logo {
        width: 204px;
        height: 64px;
        background-image: url('../assets/img/logo/group-2.png');
        background-size: cover;
        margin-right: 75px;
        cursor: pointer;
    }

    &__menu-mobile {
        display: none;
        width: 24px;
        height: 24px;
        cursor: pointer;
    }
}

.menu {
    display: flex;
    align-items: center;
    justify-content: center;
    &__item {
        width: 144px;
        text-align: center;
        cursor: pointer;
        &:nth-child(2) {
            margin-right: 20px;
        }
    }
}

.language {
    display: flex;
    justify-content: start;
    align-items: center;
    &__item {
        width: 56px;
        display: flex;
        justify-content: center;
        cursor: pointer;
        &_opacity {
            opacity: 0.4;
        }
    }
}

@media (max-width: 912px) {
    .header {
        padding: 40px 0px 40px 0px;
        &__logo {
            margin-right: 0;
        }
    }
}

@media (max-width: 768px) {

    .header {
        min-width: 768px;
        padding: 40px 0px 40px 53px;
        margin-bottom: 123px;
        &__container {
            max-width: 694px;
        }
        &__logo {
            height: 64px;
            width: 64px;
            background-image: url('../assets/img/logo/group-2Tablet.png');
            margin-right: 15px;
        }
    }

    .menu {
        &__item {
            max-width: 120px;
        }
    }
}

@media (max-width: 391px) {
        .header {
            min-width: 375px;
            padding: 40px 0px 40px 37px;
            margin: 0 auto;
            margin-bottom: 101px;
            &__container {
                max-width: 293px;
            }
            &__logo {
                width: 204px;
                height: 64px;
                background-image: url('../assets/img/logo/group-2.png');
                margin-right: 15px;
            }
            &__menu-mobile {
                display: block;
                width: 24px;
                height: 24px;
            }
    }

    .menu {
        display: none;
    }

    .menu-mobile {
        width: 375px;
        height: 613px;
        padding-top: 233px;

        &__item {
            height: 56px;
            padding: 11px 40px 11px 2px;
            box-sizing: border-box;
            &:nth-child(4) {
                margin-bottom: 50px;
            }

            font-family: 'Catamaran', sans-serif;
            font-size: 21px;
            font-weight: bold;
            letter-spacing: -0.53px;
        }

        &__language {
            display: flex;
            align-items: center;
            box-sizing: border-box;
            justify-content: space-between;
            width: 343px;
            height: 56px;
            padding: 11px 40px 11px 3px;
            margin-bottom: 50px;

            font-family: 'Catamaran', sans-serif;
            font-size: 21px;
            font-weight: bold;
            letter-spacing: -0.53px;
        }

        &__button {
            display: flex;
            align-items: center;
            margin-left: -21px;

            button {
                font-family: 'Catamaran', sans-serif;
                font-size: 21px;
                font-weight: 900;
                letter-spacing: -0.53px;
                text-align: center;
                color: #fff;

                width: 345px;
                height: 44px;
                border-radius: 72px;
                background: rgba(8, 61, 119);
                border: none;
            }
        }
    }

    .language {
        display: none;
    }

    .language-mobile {
        &__lang {
            display: flex;

            font-family: 'Open Sans', sans-serif;
            font-size: 17px;
            font-weight: 600;
            letter-spacing: 0.13px;
            text-align: center;

            &_item {
                width: 56px;
            }
        }
        &_opacity {
            opacity: 0.4;
        }
    }

}
</style>
