<template>
    <div>
        <nav class="small-screen-nav-container">
            <ul class="left-small-nav">
                <li class="logo">
                    <router-link to="#">
                        <img src="@/assets/images/logo.png" alt="logo_image">
                    </router-link>
                </li>
                <li class="dropdown">
                    <router-link to="#" class="dropdown-toggle" id="dropdownMenuButton1" data-bs-toggle="dropdown">
                        Kategoriler
                    </router-link>
                    <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
                        <li ><a class="dropdown-item text-black" href="#">Action</a></li>
                        <li ><a class="dropdown-item text-black" href="#">Another action</a></li>
                        <li ><a class="dropdown-item text-black" href="#">Something else here</a></li>
                    </ul>
                </li>
            </ul>
            <ul class="right-small-nav">
                <li>
                    <router-link to="#">
                        <i class="fa-solid fa-magnifying-glass"></i>
                    </router-link>
                </li>
                <li class="user-icon">
                    <router-link to="#" >
                        <i class="fa-solid fa-user"></i>
                    </router-link>
                </li>
                <li>
                    <router-link to="#" class="bar-icon">
                        <i class="fa-solid fa-bars"></i>
                    </router-link>
                </li>
            </ul>
        </nav>
    </div>
</template>

<script>
export default {

}
</script>

<style>

.small-screen-nav-container {
    background-color: var(--theme-color-black);
    display: flex;
    justify-content: space-between;
    padding: 20px;
}
.small-screen-nav-container ul{
    list-style: none;
}
.small-screen-nav-container ul li a{
    text-decoration: none;
    color: white;
}
.small-screen-nav-container ul li:not(.logo){
    padding-top: 10px;
}
.small-screen-nav-container .left-small-nav{
    display: flex;
    width: 40%;
    padding: 0;
    margin: 0;
    gap: 25px;
}
.small-screen-nav-container .right-small-nav{
    display: flex;
    justify-content: flex-end;
    width: 60%;
     padding: 0px 20px 0px 0px;
    margin: 0;
    gap: 20px;
}

.small-screen-nav-container .right-small-nav li .fa-user{
    background-color: var(--theme-color-blue);
    padding: 10px;
    border-radius:50%;
    width: 30px;
    height: 30px;
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>