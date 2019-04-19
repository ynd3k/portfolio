<template>
    <section class="skill-section" id="skill">
        <div class="skill">
            <div class="skill__title">
                <i class="fab fa-html5 skill__title__icon icon-html5"></i>
                <h3>HTML5</h3>
            </div>
            <p class="skill__body">
                基礎的なコーディングができます。
            </p>
        </div>
        <div class="skill">
            <div class="skill__title">
                <i class="fab fa-css3-alt skill__title__icon icon-css3"></i>
                <h3>CSS3</h3>
            </div>
            <p class="skill__body">
                基礎的なコーディングができます。
            </p>
        </div>
        <div class="skill">
            <div class="skill__title">
                <i class="fab fa-js-square skill__title__icon icon-js"></i>
                <h3>JavaScript</h3>
            </div>
            <p class="skill__body">
                基礎的なコーディングができます。
            </p>
        </div>
        <div class="skill">
            <div class="skill__title">
                <img src="../assets/jquery.png" alt="" class="skill__title__icon icon-jquery">
                <h3>jQuery</h3>
            </div>
            <p class="skill__body">
                基礎的なコーディングができます。
            </p>
        </div>
        <div class="skill">
            <div class="skill__title">
                <img src="../assets/logo.png" alt="" class="skill__title__icon icon-vue">
                <h3>Vue.js</h3>
            </div>
            <p class="skill__body">
                チュートリアルをやりました。
            </p>
        </div>
        <div class="skill">
            <div class="skill__title">
                <i class="fab fa-php skill__title__icon icon-php"></i>
                <h3>PHP</h3>
            </div>
            <p class="skill__body">
                Webサービスに必要な基本的な機能を実装できます。
            </p>
        </div>
        <div class="skill">
            <div class="skill__title">
                <img src="../assets/fuelphp.png" alt="" class="skill__title__icon icon-fuel">
                <h3>FuelPHP</h3>
            </div>
            <p class="skill__body">
                チュートリアルをやりました。
            </p>
        </div>
        <div class="skill">
            <div class="skill__title">
                <img src="../assets/mysql.png" alt="" class="skill__title__icon icon-mysql">
                <h3>MySQL</h3>
            </div>
            <p class="skill__body">
                基本的なSQL文でデータベース操作ができます。
            </p>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@import '../scss/global.scss';
.skill{
    background: #fff;
    border-radius: 12px;
    text-align: center;
    padding: $space-xm;
    box-shadow: 0px 3px 10px #ddd;;
    &__title{
        display: flex;
        align-items: center;
        justify-content: center;
        &__icon{
            font-size: 2em;
            margin-right: $space-s;
        }
    }
}
.skill-section{
    display: grid;
    justify-content: center;
    grid-template-columns: 20% 20% 20% 20% 20%;
    grid-column-gap: $space-xm;
    grid-row-gap: $space-xm;
    position: relative;
    top: -100px;
    margin: 0 auto;
    width: 88%;
    @include mq_xs(){
        grid-template-columns: 100%;
    }
    @include mq_sm(){
        grid-template-columns: 50% 50%;
    }
    @include mq_md(){
        grid-template-columns: 33% 33% 33%;
    }
    @include mq_lg(){
        grid-template-columns: 25% 25% 25% 25%;
    }
}
.icon-html5{
    color: #fd5600;
}
.icon-css3{
    color: #00a5da;
}
.icon-js{
    color: #ffd800;
}
.icon-jquery{
    color: #2a689a;
    width: 24px;
}
.icon-vue{
    width: 24px;
}
.icon-php{
    color: #7377b2;
}
.icon-fuel{
    width: 19px;
}
.icon-mysql{
}
</style>
