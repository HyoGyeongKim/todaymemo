<template>
  <div>
    <b-navbar toggleable="lg" type="dark" style="background:#ffd9e4">
      <b-navbar-brand to="/"><img src='../assets/images/logo.png' alt="logo"></b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"><img src='../assets/images/mbtn.jpg' alt="logo"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item to="/"><p class="blue">오늘의메모</p></b-nav-item>
          <b-nav-item to="/gallery"><p class="blue">갤러리</p></b-nav-item>
          <b-nav-item to="/boardlist"><p class="blue">공지사항</p></b-nav-item>
          <b-nav-item to="/Photo"><p class="blue">사진기록장</p></b-nav-item>
          <b-nav-item to="/Calendar"><p class="blue">달력</p></b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  nama: "Header",
  data() {
    return {

    }
  }
};
</script>
<style>
 .blue {color:#ff4a7b}
</style>