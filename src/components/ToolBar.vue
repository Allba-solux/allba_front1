<template>
    <div id="bo">
    <div class ="wrap">
    <link href="custom.css" rel="stylesheet">
    <header>
    <router-link to="/main" class="logo">Allba<span id="clock"><i class="fa-solid fa-clock-rotate-left"></i></span></router-link>
    <nav>
        <ul class="gnb">
            <li><a><router-link to="/finding">지점찾기</router-link></a></li>
            <li><a><router-link to="/schedule">스케쥴링</router-link></a></li>
            <li><a><router-link to="/login">로그인</router-link></a></li>
            <li><a><router-link to="/login"><span id="bell"><i class="fa-regular fa-bell"></i></span></router-link></a></li>
            
        </ul>
    </nav>
    </header>
    </div>
    </div>
</template>
<script>

export default {
    
}
</script>

<style scoped>
#bo header {
    background-color:rgba(255, 253, 242, 0.968);
    width: 100%;
    height: 120px;
    line-height: 120px;
    padding: 0 60px;
    box-sizing: border-box;
    box-shadow: 0 3px 7px rgba(0, 0, 0, 0.1);
    top: 0;
    z-index: 100;
    /* background: #fff; */
}

#bo header .logo {
    display: block;
    font-size: 41px;
    font-weight: 800;
    letter-spacing: -5px;
    color: rgba(41, 22, 0, 0.99);
    float: left;
}

#bo header nav {
    float: right;
}

#bo header nav .gnb li {
    display: inline-block;
    margin-left: 60px;
    color: rgba(41, 22, 0, 0.99);
}

#bo header nav .gnb li a {
    display: block;
    font-size: 18px;
    text-transform: uppercase;
    position: relative;
}

#clock{
    font-size:41.5px;
}

#bo header nav .gnb li a:after {
    content: '';
    width: 0%;
    height: 1px;
    position: absolute;
    background: #888;
    bottom: 47px;
    left: 50%;
    transform: translateX(-50%);
    transition: all 0.5s;
}

#bo header nav .gnb li a:hover:after,
#bo header nav .gnb li a:focus:after {
    width: 100%;
}

#bell{
    font-size:20px;
}
#bo i {
     font-style: normal;
 }
</style>