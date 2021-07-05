<template>
  <div>
    <header class="main-header header-2 header-absolute">
    <nav class="navbar">
      <div class="container">
        <!-- Logo -->
        <a class="navbar-brand" href="index.html"> <img src="~/assets/img/logo-lg-light.png" alt="logo"> </a>
        <!-- Menu -->
        <ul class="navbar-nav">
          <li class="menu-item menu-item-has-children">
            <a href="#">Home Pages</a>
            <ul class="submenu">
              <li class="menu-item"> <a href="index.html">Home v1</a> </li>
              <li class="menu-item"> <a href="home-v2.html">Home v2</a> </li>
            </ul>
          </li>
          <li class="menu-item menu-item-has-children">
            <a href="#">Blog</a>
            <ul class="submenu">
              <li class="menu-item menu-item-has-children">
                <a href="blog-grid.html">Blog Archive</a>
                <ul class="submenu">
                  <li class="menu-item"> <a href="blog-grid.html">Grid View</a> </li>
                  <li class="menu-item"> <a href="blog-list.html">List View</a> </li>
                  <li class="menu-item"> <a href="blog-masonry.html">Masonry</a> </li>
                </ul>
              </li>
              <li class="menu-item menu-item-has-children">
                <a href="blog-single-v1.html">Blog Single</a>
                <ul class="submenu">
                  <li class="menu-item"> <a href="blog-single-v1.html">Blog Single v1</a> </li>
                  <li class="menu-item"> <a href="blog-single-v2.html">Blog Single v2</a> </li>
                  <li class="menu-item"> <a href="blog-single-v3.html">Blog single v3</a> </li>
                </ul>
              </li>
            </ul>
          </li>
          <li class="menu-item menu-item-has-children">
            <a href="#">Pages</a>
            <ul class="submenu">
              <li class="menu-item"> <a href="about-us.html">About Us</a> </li>
              <li class="menu-item"> <a href="login.html">Login</a> </li>
              <li class="menu-item"> <a href="register.html">Sign Up</a> </li>
              <li class="menu-item"> <a href="checkout.html">Checkout</a> </li>
              <li class="menu-item"> <a href="cart.html">Cart</a> </li>
              <li class="menu-item"> <a href="product-details.html">Product Details</a> </li>
            </ul>
          </li>
          <li class="menu-item menu-item-has-children">
            <a href="#">Courses</a>
            <ul class="submenu">
              <li class="menu-item"> <a href="courses.html">Teaching Archive</a> </li>
              <li class="menu-item"> <a href="course-details.html">Course Details</a> </li>
            </ul>
          </li>
          <li class="menu-item">
            <a href="books.html">Books</a>
          </li>
          <li class="menu-item">
            <a href="contact-us.html">Contact Us</a>
          </li>
        </ul>

        <!-- Toggler -->
        <div class="aside-toggler aside-trigger">
          <span></span>
          <span></span>
          <span></span>
        </div>

      </div>
    </nav>
  </header>
  </div>
</template>

<style>
  .navbar-nav {
      flex-direction: row;
  }
</style>
