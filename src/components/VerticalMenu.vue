<template>
    <nav>
        <div class="vertical-nav">
            <div class="vertical-nav__header"></div>
            <div class="vertical-nav__search">
                <i class="icon-search"></i>
            </div>
            <ul class="vertical-nav__list">
                <li class="vertical-nav__list__item">
                    <a href="#">
                        <i class="icon"></i>
                        <span class="vertical-nav__list__item__value active">Главная</span>
                    </a>
                </li>
                <li class="vertical-nav__list__item">
                    <a href="#">
                        <i class="icon"></i>
                        <span class="vertical-nav__list__item__value">Клиенты</span>
                    </a>
                </li>
            </ul>
            <div class="vertical-nav__footer">
                <div class="user">
                    <div class="user-icon"></div>
                    <div class="user-name"></div>
                </div>
            </div>
        </div>
    </nav>
</template>

<style lang="scss">
nav {
    position: fixed;
    overflow: hidden;
    top: 0;
    left: 0;
    min-height: 100vh;
    width: 64px;
    background: #e8ecf3;
    .vertical-nav {
        display: flex;
        flex-direction: column;
        color: #c0c4d1;
        a {
            color: inherit;

        }
        &__header {
            height: 64px;
            background: #ffffff url(../assets/hamburger-butt.svg) no-repeat center;
            box-shadow: 0 0 16px 0 rgba(0, 0, 0, 0.18);
        }
        &__search {
            height: 64px;
            background: url(../assets/search.svg) no-repeat center;
            background: url(../assets/search.svg) no-repeat center;
            line-height: 64px;
            text-align: center;
            // .icon-search {
            //     height: 15px;
            //     width: 15px;
            // }
        }
        &__list {
            border-top: 1px solid #dce0e8;
            border-bottom: 1px solid #dce0e8;
            list-style-type: none;
            margin: 0;
            padding: 0;
            height: auto;
            &__item {
                background: url(../assets/home-icon.svg) no-repeat center;
                height: 64px;
                line-height: 64px;
                text-align: center;
                &__value {
                    display: none;
                }
            }
        }
        &__footer {
            height: 64px;
            bottom: 0;
            height: 64px;
        }
        .active {
            width: auto;
        }
    }
}
</style>