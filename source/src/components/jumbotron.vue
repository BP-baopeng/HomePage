<template>
    <div class="jumbotron">
        <div class="container">
            <h1>爱编程，爱生活</h1>
            <p>欢迎访问我的个人主页！</p>
            <a-button type="primary" size="large">Hello Word!</a-button>
        </div>
    </div>
</template>
<script>
export default {

}
</script>
<style lang="scss">
    .jumbotron{
        background: url("https://source.unsplash.com/random/1600x900") no-repeat;
        background-size: 100%;
        text-align: center;
        display: block;
        width: 100%;
        max-height: 420px;
        overflow: hidden;
        .container{
            margin: 80px 0 ;
            height: 80%;
            h1{
                color: #fff;
                font-size: 4.8em;
                font-weight: 700;
                margin: 0;
            }
            p{  
                margin: 30px 0;
                font-size: 1.5em;
                color: #fff;
            }
        }
    }
    @media screen and (max-width: 768px){
        .jumbotron{
            .container{
                margin: 35px 0;
                height: 80%;
                h1{
                    color: #fff;
                    font-size: 4em;
                    font-weight: 600;
                }
                p{
                    margin: 20px 0;
                    font-size: 1.3em;
                }
            }
        }
    }
    

    
</style>