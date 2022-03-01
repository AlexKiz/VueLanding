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
            <li class='language__item'>DE</li>
            <li class='language__item'>EN</li>
        </div>
        <div class='header__menu-mobile'>
            <img src='../assets/img/header/menuMobile.png' alt='menu'/>
        </div>
    </div>
</header>
</template>

<script>
export default {
  name: 'HeaderTest'
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

@media (max-width: 375px) {
        .header {
            min-width: 375px;
            padding: 40px 0px 40px 37px;
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
            }
    }

    .menu {
        display: none;
    }

    .language {
        display: none;
    }
}
</style>
