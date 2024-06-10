<script setup>
import { ref } from "vue";


</script>



<style scoped>
.nav-content-main-ctn{
    width:100%;
    height:30%;
}
.nav-content-ctn, .nav-content-ctn-mobile{
    margin:0 3vw 5px;
    display:flex;
    justify-content: space-between;
}
.nav-content-ctn-mobile{
    width:100%;
    height:30%;
    display:none;
}
.search-box-ctn, .search-box-ctn-mobile{
    display:flex;
}
.search-box-ctn i{
    font-size:22px;
}
.search-box-ctn input{
    width:100%;
    padding:2px 1vw;
    background-color: rgba(79, 105, 121, 0.479);
    color:white;
    border:0;
}
.search-box-ctn input::placeholder{
    color: rgba(255, 255, 255, 0.596);
}
.nav-list-ctn ul{
    display:flex;
    gap:20px;
}
.nav-list{
    color: white;
}
.menu-bar-ctn i{
    font-size:22px;
    display:none;
}


@media screen and (max-width:950px){
    .nav-content-ctn{
        display:none;
    }
    .nav-content-ctn-mobile{
        display:flex;
    }
    .nav-list-ctn-mobile{
        background-color: rgb(27, 40, 48);
        display:flex;
        position:absolute;
        right:20px;
        top:7vh;
        width:80%;
        min-width:60%;
        height:auto;
        place-items:center;
        justify-content:center;
    }
    .nav-list-ctn-mobile ul .nav-list{
        width:100%;

        margin:40px 0;
        font-size: 20px;
        text-align:center;
    }
    .search-box-ctn-mobile input{
        display:none;
    }

}
</style>

<template>
    <div class="nav-content-main-ctn">
        <div class="nav-content-ctn">

            <!-- search box -->
            <div class="search-box-ctn">
                <!-- logo -->
                <i class='bx bx-search'></i>
                <!-- input box -->
                <input type="text" placeholder="Search...">
            </div>

            <!-- Nav list container -->
            <div class="nav-list-ctn">
                <ul>
                    <li class="nav-list">Home</li>
                    <li class="nav-list">Blog</li>
                    <li class="nav-list">About</li>
                    <li class="nav-list">Initiatives</li>
                    <li class="nav-list">Books</li>
                    <li class="nav-list">Media</li>
                    <li class="nav-list">Diving</li>
                    <li class="nav-list">Contact</li>
                    
                </ul>
            </div>

            <!-- menu bar -->
        </div>

        <!-- MOBILE VIEW -->
        <div class="nav-content-ctn-mobile">

            <!-- search box -->
            <div class="search-box-ctn-mobile">
                <!-- logo -->
                <i class='bx bx-search'></i>
                <!-- input box -->
                <input type="text" placeholder="Search...">
            </div>

            <!-- Nav list container -->
            <div class="nav-list-ctn-mobile">
                <ul>
                    <li class="nav-list">Home</li>
                    <li class="nav-list">Blog</li>
                    <li class="nav-list">About</li>
                    <li class="nav-list">Initiatives</li>
                    <li class="nav-list">Books</li>
                    <li class="nav-list">Media</li>
                    <li class="nav-list">Diving</li>
                    <li class="nav-list">Contact</li>
                    
                </ul>
            </div>

            <!-- menu bar -->
        </div>
    </div>
</template>