<template>
    <div class="footer" id="footer">
        <h2>連絡先</h2>
        <ul class="contact">
            <li>
                <i class="fab fa-twitter icon"></i>
                <a href="">@nanshi099</a>
            </li>
            <li>
                <i class="far fa-envelope icon"></i>
                <a href="">net@gmail.cpm</a>
            </li>
            <li>
                <i class="fab fa-github icon"></i>
                <a href="">github.com</a>
            </li>
            <li>
                <span class="icon">Qiita</span>
                <a href="">github.com</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    data: function(){
        return{
            show: true
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../scss/global.scss';

.footer{
    box-sizing: border-box;
    background: $theme-color;
    color: $bg-color;
    text-align: center;
    padding: $space-m;
    width: 100%;
    margin-top: auto;
}
.contact{
    list-style: none;
    // margin: 0 auto;
    // width: 60%;
    padding-left: 0;
    & a{
        color: #fff;
        text-decoration-line: underline;
    }
    & li{
        display: flex;
        align-items: center;
        justify-content: space-between;
        // text-align: left;
        margin: 0 auto;
        width: 180px;
        margin-bottom: $space-s;
    }
}
.icon{
    font-size: 1.3em;
    margin-right: $space-xm;
    width: 50px;
}
.icon-q{
    width: 30px;
    background: #55c500;
}
</style>

