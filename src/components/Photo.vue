<template>
    <div>
  <b-card no-body>
    <b-tabs card>
      <b-tab no-body title="고양이 기록1">
        <b-card-img bottom fluid :src="require('../static/c1.jpg')" alt="Image 1"></b-card-img>
        <b-card-footer>집 앞 고양이들</b-card-footer>
      </b-tab>

      <b-tab no-body title="고양이 기록2">
       <b-card-img bottom fluid :src="require('../static/c2.jpg')" alt="Image 1"></b-card-img>
        <b-card-footer>고양이 카페 방문 1</b-card-footer>
      </b-tab>

      <b-tab no-body title="고양이 기록3">
        <b-card-img bottom fluid :src="require('../static/c3.jpg')" alt="Image 1"></b-card-img>
        <b-card-footer>고양이 카페 방문2</b-card-footer>
      </b-tab>
    </b-tabs>
  </b-card>
</div>
</template>
<script>
export default {
    
}
</script>