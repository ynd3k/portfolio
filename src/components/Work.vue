<template>
    <div>
        <section class="section" id="work">
            <h2 class="section__title">制作物</h2>
        </section>
        <section class="work-section">
            <div class="work">
                <img  class="work__img" src="../assets/forum.png" alt="">
                <div class="work__explain">
                    <dl class="list">
                        <dt>概要</dt>
                        <dd class="">
                            Webサービス部の復習として作った掲示板です。
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>機能</dt>
                        <dd class="">
                            ユーザ登録、ログイン、ログアウト、投稿、編集、検索、パスワード編集、プロフィール編集、ダイレクトメッセージ、お気に入り
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>URL</dt>
                        <dd class="">
                            https://forum0.herokuapp.com/
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>ソース</dt>
                        <dd class="">
                            https://github
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>言語</dt>
                        <dd class="">
                            HTML/CSS/JavaScript/jQuery/PHP+MySQL
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>公開</dt>
                        <dd class="">
                            Heroku
                        </dd>
                    </dl>
                </div>
            </div> 
        </section>
        <section class="work-section work-wp-theme">
            <div class="work">
                <img  class="work__img" src="../assets/tree.png" alt="">
                <div class="work__explain">
                    <dl class="list">
                        <dt>概要</dt>
                        <dd class="">
                            スクールの卒業課題で、美容院のWordPressテーマを作りました。
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>機能</dt>
                        <dd class="">
                            カスタムフィールド、ウィジェット等の基本的な機能を使いました。
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>URL</dt>
                        <dd class="">
                            http://wp-tree.herokuapp.com/
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>ソース</dt>
                        <dd class="">
                            https://github
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>言語</dt>
                        <dd class="">
                            HTML/CSS/JavaScript/jQuery/PHP
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>公開</dt>
                        <dd class="">
                            レンタルサーバー
                        </dd>
                    </dl>
                </div>
            </div> 
        </section>
        <section class="work-section work-this-site">
            <div class="work">
                <img  class="work__img" src="../assets/site.png" alt="">
                <div class="work__explain">
                    <dl class="list">
                        <dt>概要</dt>
                        <dd class="">
                            ポートフォリオサイト（このサイト）です。
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>機能</dt>
                        <dd class="">
                            Vue.jsで作りました。
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>URL</dt>
                        <dd class="">
                            https://nanshi99.firebaseapp.com/
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>ソース</dt>
                        <dd class="">
                            https://github
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>言語</dt>
                        <dd class="">
                            HTML/CSS/JavaScript/Vue.js
                        </dd>
                    </dl>
                    <dl class="list">
                        <dt>公開</dt>
                        <dd class="">
                            Firebase
                        </dd>
                    </dl>
                </div>
            </div> 
        </section>
    </div>
</template>

<style lang="scss" scoped>
@import '../scss/global.scss';

.section{
    width: 100%;
    box-sizing: border-box;
    background: $theme-color;
    padding: $space-l 0 120px;
    margin-bottom: 30px;
    color: #fff;
    text-align: center;
    margin: 0 auto 10px;
    &__title{
        text-align: center;
    }
}
.work-section{
    position: relative;
    top: -100px;
    margin: 0 auto;
    width: 88%;
}
.work{
    display: flex;
    justify-content: space-between;
    @include mq_l(){
        flex-direction: column;
        align-items: center;
    }
    &__img{
        border-radius: 12px;
        object-fit: cover;
        object-position: 0px 0px;
        box-shadow: 0px 3px 10px #ddd;
        width: 100%;
        max-width: 250px;
        max-height: 380px;
        margin-right: $space-xm;
        @include mq_l(){
            margin-bottom: $space-xm;
            width: unset;
            margin-right: 0;
        }
    }
    &__explain{
        width: 100%;
        box-sizing: border-box;
        word-break: break-word;
        background: #fff;
        color: $theme-color;
        border-radius: 12px;
        box-shadow: 0px 3px 10px #ddd;
        padding: $space-xm $space-m;
    }
}
.list{
    display: flex;
    & dt{
        width: 20%;
        margin-right: $space-s;
    }
    & dd{
        width: 80%;
        margin: 0;
    }
}
.work-wp-theme{
    top: -30px;
}
.work-this-site{
    top: 40px;
    margin-bottom: 100px;//修正
}
</style>
