<template>
    <div class="profile" id="profile">
        <h2 class="profile__title">自己紹介</h2>
        <p class="profile__body">
            はじめまして。[名前]と申します。平成6年生まれの24歳です。高校中退後、職歴はありません。Webエンジニアになりたいと思い、2018年11月にプログラミングを始めました。アニメーションに興味があります。
        </p>
    </div>
</template>

<style lang="scss" scoped>
@import '../scss/global.scss';

.profile{
    width: 100%;
    box-sizing: border-box;
    background: $theme-color;
    padding: $space-l 0 120px;
    margin-bottom: 30px;
    color: #fff;
    text-align: center;
    &__body{
        width: 60%;
        margin: 0 auto;
    }
}
</style>
