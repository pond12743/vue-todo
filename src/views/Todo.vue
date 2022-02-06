<template>
    <v-container >
    <h1>การบ้าน/งานที่ได้รับมอบหมาย</h1>
    <Input @Addata="addTodo"></Input>
  <Data :additems="additems"></Data>
  </v-container>


</template>

<script>
import Input from '../components/Addwork.vue';
import Data from '../components/Data.vue';
export default { 
  data: () =>  ({
      additems: [],
    }),
  additems:"Addata",
  methods:{
    addTodo(subject,work,Time) {
      this.additems.push({
        text1 : subject + " | " + work+ " | "+Time,
      });
    },
  },
 components: { Data,Input },
};
</script>

<style></style>
