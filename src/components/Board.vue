<template>
  <div>
    <b-table
      striped
      hover
      :items="items"      
      :fields="fields"
      @row-clicked="rowClick"
    ></b-table>
     <button class="bbtn" @click="writeContent">글쓰기</button>
     
  </div>
</template>

<script>
import data from "@/data";
 
   let items = data.Content.sort((a, b) => {
      return b.content_id - a.content_id;
    }); // 내림차순
    const user_name='운영자'
  
export default {
  name: "Board",
  data() {
   
     return {
    
      // bootstrap 'b-table' 필드 설정
      fields: [
        {
          key: "content_id",
          label: "번호"
        },
        {
          key: "title",
          label: "제목"
        },
        {
          key: "user_name",
          label: "글쓴이"
        },
        {
          key: "created_at",
          label: "작성일"
        }
      ],
      items: items
    };
  },
  methods: {
  
    rowClick(items) {
      this.$router.push({
        path: `/detail/${items.content_id}`
      });
      
    },
   
    writeContent() {
      this.$router.push({
        path: `/create`
      });
      
    }
  },
  computed: {
    rows() {
        return this.items;
    }
  },
   
}
</script>
<style>
 .bbtn {background: #ff4a7b;border:none;color:white;width:100px;height:40px;border-radius:8px}
 .bbtn:hover {background:#ffa0bb}
</style>