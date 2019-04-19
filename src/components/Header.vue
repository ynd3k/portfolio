<template>
    <div>
        <div class="header">
            <h1 class="header__logo"><a href="">ポートフォリオ</a></h1>
            <ul class="menu">
                <li class="menu__item">自己紹介</li>
                <li class="menu__item">スキル</li>
                <li class="menu__item">制作物</li>
                <li class="menu__item">連絡先</li>
            </ul>
            <div class="menu-sp"
                 @click="isOpen = !isOpen"
                 v-bind:class="{'menu-sp__line--active': isOpen}">
                <span class="menu-sp__line"></span>
                <span class="menu-sp__line"></span>
                <span class="menu-sp__line"></span>
            </div>
            <div v-if="isOpen" class="menu-open">
                <ul class="sp-menu" @click="isOpen = !isOpen">
                    <a class="sp-menu__item" href="#profile">自己紹介</a>
                    <a class="sp-menu__item" href="#skill">スキル</a>
                    <a class="sp-menu__item" href="#work">制作物</a>
                    <a class="sp-menu__item" href="#footer">連絡先</a>
                </ul>
            </div>
        </div>

        <div class="header-top">
            <h2 class="header-top__title">なんしのポートフォリオ</h2>
            <img src="../assets/top-icon.png" alt="">
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            isOpen: false
        }
    },
    methods:{
        clickMenuSp: function(){
            this.isOpen = !this.isOpen;
            console.log(isOpen);
        }
    }
}
</script>


<style lang="scss" scoped>
@import '../scss/global.scss';

.header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: $theme-color;
    border-bottom: $border;
    margin-bottom: $space-3l;
    &__logo{
        margin-left: $space-xm;
        font-weight: unset;
        font-size: 1.4em;
    }
}
.menu{
    list-style: none;
    display: flex;
    &__item{
        margin-right: $space-xm;
    }
    @include mq_xl(){
        display: none;
    }
}
.header-top{
    margin: 0 auto;
    width: 60%;
    text-align: center;
    &__title{
        font-weight: unset;
    }
}
.menu-sp{
    @include mq_xl(){
        display: block;
    }
    display: none;
    margin-right: 15px;
    width: 28px;
    height: 28px;
    position: relative;
    cursor: pointer;
    // border: $border;
    &__line{
        width: 100%;
        background: $theme-color;
        height: 2px;
        position: absolute;
        display: block;
        width: 100%;
        transition: all .5s;
        &--active &:nth-child(1){
            transform: translateY(8px) rotate(-45deg);
        }
        &--active &:nth-child(2){
            opacity: 0;
        }
        &--active &:nth-child(3){
            transform: translateY(-8px) rotate(45deg);
        }
        &:nth-child(1){
            top: 5px;
        }
        &:nth-child(2){
            top: 13px;
        }
        &:nth-child(3){
            bottom: 5px;
        }
    }
}
.menu-open{
    position: absolute;
    right: 0px;
    top: 70px;
    width: 150px;
    height: auto;
    background: #fcfcfc;
}
.sp-menu{
    list-style: none;
    transition: all .5s;
    padding-left: 0;
    &__item{
        display: block;
        padding: $space-xs $space-xm;
        &:hover{
            background: beige;
        }
    }
}
</style>




