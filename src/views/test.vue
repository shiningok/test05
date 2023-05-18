<script setup>

</script>

<template>


    <main>
        <div class="top">
            <span class="text"> 질문 내용 질문 내용 질문 내용</span>
            <img :src="`https://slp-statics.astockcdn.net/static_assets/staging/22spring/kr/video/curated-collections/card-5.jpg?width=580&format=webp`"
                 alt=""/>
        </div>
        <div id="test"></div>
        <div class="b">
            <a href="#">
                선택 A
            </a>
            <a href="#">
                선택 B
            </a>
            <a href="#">
                선택 C
            </a>
        </div>
    </main>

</template>

<style scoped>
.top {
    height: 10px;
    margin-bottom: 100px;
}

.top .text {
    position: absolute;
    color: white;
    font-weight: 10;
    font-size: 20px;
    padding: 50px;
    margin-left: 500px;

}

img {
    position: static;
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}

a {
    position: relative;
    font-size: 20px;
    background: gray;
    margin-right: 5px;
    margin-left: 5px;
    padding-left: 30px;
    padding-right: 30px;
    color: white;
}

.b {
    position: absolute;
    bottom: 0px;
    margin-right: 50px;
    margin-left: 50px;
    margin-bottom: 30px;
    left: 30%;
}

#test {
    background-color: #18181888;
    position: absolute;
    right: 0;
    bottom: 0;
    width: 100%;
    height: 10%;


}


</style>