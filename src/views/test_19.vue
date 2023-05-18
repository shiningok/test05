<script setup>


</script>

<template>
    <main>

        <div class="img">
            <div>
                <a href="#"> ← 설정</a>
            </div>
            <div>
                <div class="b">제어 방법</div>
            </div>
            <div>
                <div class="c">설정</div>
            </div>

            <div>
                <img :src="`https://slp-statics.astockcdn.net/static_assets/staging/23spring/kr/home/curated-collections/card-6.jpg?width=580&format=webp`"
                     alt=""/>
            </div>

            <div id="box">
                <span style="color: white">설정</span>
                <hr>
                <ul>
                    <li>음량
                        <line>
                            <input type="checkbox">
                            <span style="font-size: 15px"> 음소거</span>
                        </line>
                        <div style="font-size: 15px; margin-left: 80px">0
                            <input type="range" min="1" max="10"/>
                        </div>
                    </li>
                    <hr>
                    <li>자막
                        <line>
                            <label class="switch-button">
                                <input type="checkbox"/>
                                <span class="onoff-switch"></span>
                            </label>
                        </line>
                    </li>
                    <hr>
                    <li>언어
                        <line>
                            <button class="back">❮</button>
                            <span style="margin-left: 40px">English</span>
                            <button class="next">❯</button>

                        </line>
                    </li>
                    <hr>
                    <li>해상도
                        <line>
                            <input type="checkbox">
                            <span style="font-size: 20px; " > 창모드</span>
                            <button class="back2;">❮</button>
                            <span style="font-size: 20px ">2560*1440 (UHD)</span>
                            <button class="next2">❯</button>
                        </line>
                    </li>
                </ul>

            </div>


        </div>

    </main>

</template>

<style scoped>

img {
    position: static;
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}

a {
    position: absolute;
    margin: 30px 30px 30px 30px;
    font-size: 30px;
    padding: 10px;
    color: #ffffff;
    background-color: transparent;
}

.img .b {
    position: absolute;
    padding: 10px 50px 10px 50px;
    background: lightgray;
    color: white;
    display: inline-block;
    margin-left: 40px;
    margin-top: 100px;


}

.img .c {
    position: absolute;
    padding: 10px 70px 10px 58px;
    background: lightgray;
    color: white;
    display: inline-block;
    margin-left: 40px;
    margin-top: 150px;
    border: 2px solid #ffffff;
}

#box {
    background-color: #18181888;
    position: absolute;
    right: 0;
    bottom: 0;
    margin-right: 40px;
    margin-bottom: 400px;
    width: 35%;
    height: 35%;
    font-size: 25px;
}

#box ul li {
    list-style-type: none;
    padding: 20px;
    color: white;
    margin-left: 20px;
    margin-right: 30px;
}

line {
    position: relative;
    margin-left: 30px;
}

.switch-button {
    position: relative;
    display: inline-block;
    width: 200px;
    height: 30px;
}

.switch-button input {
    opacity: 0;
    width: 200px;
    height: 30px;
}

.onoff-switch {
    position: absolute;
    cursor: pointer;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    border-radius: 20px;
    background-color: #ccc;
    box-shadow: inset 1px 5px 1px #999;
    -webkit-transition: .4s;
    transition: .4s;
}

.onoff-switch:before {
    position: absolute;
    content: "";
    height: 29px;
    width: 100px;
    left: 0px;
    bottom: 0px;
    background-color: #fff;
    -webkit-transition: .5s;
    transition: .4s;
    border-radius: 20px;
}

.switch-button input:checked + .onoff-switch {
    background-color: #F2D522;
    box-shadow: inset 1px 5px 1px #E3AE56;
}

.switch-button input:checked + .onoff-switch:before {
    -webkit-transform: translateX(50px);
    -ms-transform: translateX(50px);
    transform: translateX(100px);
}


.back {
    position: relative;
    bottom: 0px;
    right: 10px;

}

.next {
    position: relative;
    margin-left: 50px;
}
.back2{

    position: relative;
    bottom: 0px;
    left: -10px;
}
.next2{
    position: relative;
    bottom: 0px;
    right: -10px;

}

button {
    width: 20px;
    height: 20px;
    color: white;
    background: transparent;
}

button:active {
    background: #3e3e3e;
}

button:disabled {
    background: #cbcaca;
}

</style>