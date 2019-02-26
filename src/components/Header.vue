<template>
    <div class = "header">
        <div >
            <a href="/" class="main-header__brand">Test for you</a>
        </div>
        <nav class="main-nav">
            <!-- <router-link tag="li" to="/students">Students</router-link> -->
            <ul class="main-nav__items">
                <!-- <li class="main-nav__item">
                    <a href="/students">Users</a>    
                </li>
                <li class="main-nav__item">
                    <a href="/">Courses</a>    
                </li> -->
                <router-link tag="li" exact to="/students" class="main-nav__item" active-class="active">
                    <a>Students</a>
                </router-link>
                <router-link tag="li" to="/" class="main-nav__item" active-class="active">
                    <a>Courses</a>
                </router-link>
            </ul>
        </nav>
    </div>
</template>
<script>
export default {
    data: function () {
    return {
  
    }
  },    
}
</script>

<style>
    @import url('https://fonts.googleapis.com/css?family=Montserrat" rel="stylesheet');

    .header {
        background: grey;
        width: 100%;
        padding: 8px 16px;
    }

    .header > div {
        display: inline-block;
        vertical-align: middle;
    }

    .main-header__brand {
        color:honeydew;
        text-decoration: none;
        font-weight: bold;
        font-size: 22px;
        font-family: 'Montserrat';
      
    }

    .main-nav {
        display: inline-block;
        text-align: right;
        width: calc(100% - 115px);
        vertical-align: middle;
    }

    .main-nav__items {
        margin: 0;
        padding: 0;
        list-style: none;
    }

    .main-nav__item {
        display: inline-block;
        margin: 0 16px;
        text-decoration: none;
    }

    .main-nav__item a {
        text-decoration: none;
        color: honeydew;
        font-weight: bold;
        padding: 3px;
        
    }

    .main-nav__item a:hover,
    .main-nav__item a:active
    {
        color: blue;
        border-bottom: 5px solid blue;
    }
    .active {
        color: brown;
    }



</style>


