<template>
  <nav class="navbar navbar-light nav__bar">
    <a class="nav__logo" href="#"><span class="head_span">theFortunate</span>Developer.</a>
    <div class="humburger">
      <img src="../static/menu.png" alt="" width="30">
    </div>
    <ul class="nav nav-bar">
      <li class="nav-item">
        <a href="#" class="nav-link active">Home</a>
      </li>
      <li class="nav-item">
        <a href="#about" class="nav-link">About</a>
      </li>
      <li class="nav-item">
        <a href="#skills" class="nav-link">Skills</a>
      </li>
      <li class="nav-item">
        <a href="#contact" class="nav-link">Contact</a>
      </li>
      <li class="nav-item">
        <a href="#" class="nav-link">Blog</a>
      </li>
      <li class="nav-item">
        <a href="#" class="nav-link"><i class="uil uil-moon"></i></a>
      </li>
    </ul>
    <!--<div class="page_progress" id="scroll_progress"></div>-->
  </nav>
</template>

<script>
export default {
  name: 'SiteNavbar'

}
</script>