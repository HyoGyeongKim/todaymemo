<template>
  <div role="tablist">
    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-1 variant="danger">오늘의 메모를 이용해주셔서 감사합니다</b-button>
      </b-card-header>
      <b-collapse id="accordion-1" visible accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>
            <img src='../static/thanks.png' alt='thanks'/> 
          <!-- <b-img :src="require('../static/pic.jpg')" alt='pic1'></b-img> -->
          </b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-2 variant="danger">공지사항</b-button>
      </b-card-header>
      <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>
           <img src='../static/pic1.jpg' alt='pic1'/>
          </b-card-text>
           <b-card-text>
          {{ text }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-3 variant="danger">자료실</b-button>
      </b-card-header>
      <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>
           <img src='../static/pic2.jpg' alt='pic2'/>
          </b-card-text>
           <b-card-text>
          {{ text2 }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        text: `
          공지사항입니다. 새로운 소식은 공지사항을 참조하세요.
        `,
        text2: `
          메인의 작성하기 버튼을 통해 간단한 메모를 남겨보세요. 
        `
      }
    }
  }
</script>