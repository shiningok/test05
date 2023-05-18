<script>
import TheWelcome from '../components/TheWelcome.vue'

export default {
    name: 'HelloWorld',
    data() {
        return {
            id: "",

        }
    },
    mounted() {
        var elmList = document.querySelectorAll("#test ul li")
        console.log(elmList)
        for (var i = 0; i < elmList.length; i++) {
            var elm = elmList[i]

            elm.addEventListener("click", function () {
                elmList.forEach(function (item) {
                    item.classList.remove("active");
                })

                this.classList.add("active")
            })
        }
    },

}
</script>

<template>
    <main>


        <video autoplay src="../assets/sample.mp4" style=""></video>

        <div class="layer">
            <div>
                <span class="bordered">전체</span>
                <span class="bordered">FHD</span>
            </div>
            <div style="float: right;">
                <img :src='`https://blog.kakaocdn.net/dn/evVAm5/btq7p9Wt4Qi/LWkvYk4QkBq6PSv1oTMAN1/img.gif`' alt=""/>
            </div>
            <div class="tag-wrapper">
                2023 · 인터랙티브	· 청춘드라마	· 로맨스	· 코미디
            </div>
            <div style="margin-top:10px;">
                <a style="display: inline-block" href="#">
                    이어서 재생
                </a>
            </div>
            <div style="margin-top:10px;">
                <a style="display: inline-block">
                    처음부터 다시
                </a>
            </div>
            <div style="margin-top:10px;" >
                <b style="display: inline-block">
                    전체 로드맵 보기
                </b>
            </div>

            <div id="test">
                <span>선택할수 있는 장면 </span>
                <ul>
                    <li>
                        <span> 1 </span>
                        <img :src='`https://blog.kakaocdn.net/dn/evVAm5/btq7p9Wt4Qi/LWkvYk4QkBq6PSv1oTMAN1/img.gif`'
                             alt=""/>
                        <div style="display: inline-block">
                            <p>alskdjf</p>
                            <p>영화보러가요 </p>
                        </div>
                    </li>
                    <li>
                        <span>2</span>
                        <img :src='`https://blog.kakaocdn.net/dn/evVAm5/btq7p9Wt4Qi/LWkvYk4QkBq6PSv1oTMAN1/img.gif`'
                             alt=""/>
                        <div style="display: inline-block">
                            <p>alskdjf</p>
                            <p>영화보러가요 </p>
                        </div>
                    </li>
                    <li>
                        <span>3</span>
                        <img :src='`https://blog.kakaocdn.net/dn/evVAm5/btq7p9Wt4Qi/LWkvYk4QkBq6PSv1oTMAN1/img.gif`'
                             alt=""/>
                        <div style="display: inline-block">
                            <p>alskdjf</p>
                            <p>영화보러가요 </p>
                        </div>
                    </li>
                    <li>
                        <span>4</span>
                        <img :src='`https://blog.kakaocdn.net/dn/evVAm5/btq7p9Wt4Qi/LWkvYk4QkBq6PSv1oTMAN1/img.gif`'
                             alt=""/>
                        <div style="display: inline-block">
                            <p>alskdjf</p>
                            <p>영화보러가요 </p>
                        </div>
                    </li>
                    <li>
                        <span>1</span>
                        <img :src='`https://blog.kakaocdn.net/dn/evVAm5/btq7p9Wt4Qi/LWkvYk4QkBq6PSv1oTMAN1/img.gif`'
                             alt=""/>
                        <div style="display: inline-block">
                            <p>alskdjf</p>
                            <p>영화보러가요 </p>
                        </div>
                    </li>
                    <li>
                        <span>1</span>
                        <img :src='`https://blog.kakaocdn.net/dn/evVAm5/btq7p9Wt4Qi/LWkvYk4QkBq6PSv1oTMAN1/img.gif`'
                             alt=""/>
                        <div style="display: inline-block">
                            <p>alskdjf</p>
                            <p>영화보러가요 </p>
                        </div>
                    </li>

                </ul>
            </div>

        </div>
    </main>
</template>


<style scoped>


main {
    position: relative;
    height: 100%;
    width: 100%;
}


#test {
    background-color: #18181888;
    position: absolute;
    right: 0;
    bottom: 0;
    width: 50%;
    height: 50%;


}

#test ul {
    list-style: none;
    overflow-y: auto;
    height: 100%;
}

#test ul li {
    padding: 20px;
    color: white;
}

#test ul li.active {
    border: 1px solid #ffffff;

}


video {
    height: 100%;
    width: 100%;
}

.layer {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    background: #333333;
    display: block;
    padding: 50px;
}

.layer .bordered {
    margin-right: 5px;
    padding: 5px;
    border: 1px solid #ffffff;
    color: #ffffff;
    border-radius: 5px;

}


img {
    margin-top: 30px;
    width: 100px;
    height: 100px;
}

.tag-wrapper {
    margin-top: 40px;
}

.tag-wrapper span {
    color: white;
    border: none;
}


a {
    padding: 10px 30px 10px 30px;
    background: #f8f8f8;
    display: inline-block;
    margin-right: 10px;
    border-radius: 10px;

}

b {
    padding: 10px 30px 70px 60px;
    background: #f8f8f8;
    display: inline-block;
    margin: 10px;
    border-radius: 5px;

}


</style>
