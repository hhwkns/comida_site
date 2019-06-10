<template>
  <div class="top">
    <b-navbar toggleable="lg" type="dark">
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <ul>
            <li><nuxt-link to="/">Home</nuxt-link></li>
            <li><nuxt-link to="/menu">Menu</nuxt-link></li>
            <li><nuxt-link to="/gallery">Gallery</nuxt-link></li>
            <li><nuxt-link to="/about">About</nuxt-link></li>
          </ul>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<style>
.nav-list {
     list-style: none;
     padding: 0;
     margin: 0;
 }
 .nav-item {
     margin: 0 10px;
 }
 li a {
     text-decoration: none;
     color: #212529;
     list-style-type: none;
     padding: 0;
 }
 li a:hover,
 li a:active {
     color: #b4b4b4;
    text-decoration: none;

 }
 @media (max-width: 767px) {
     .nav-list {
         display: block;
     }
     .nav-item{
         margin-top: 16px;
         margin-bottom: 16px;
     }
 }
 @media (min-width: 768px) {
     .nav-list {
         display: flex;
     }
 }

.top {
  background-color: #ACD143;
}

.links {
  list-style-type: none;
  padding: 1rem;
  text-decoration: none;
  color: black;
}
</style>
