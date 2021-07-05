<template>
  <div class="container">
    <p class="demo" :class="objClass"> Hello World {{ name }} </p>
    <button @click="changeStateActive">Active</button>
    <p> Count: {{ count }} </p>
    <button @click="increase">Increase</button>
    <button @click="decrease">Decrease</button>
    <form action="" @submit.prevent="addStudent(name,age)">
      Name: <input type="text" v-model="name1" name='name1'>
      Age: <input type="text" v-model="age" name='age'>
      <button type="submit" >add student</button>
    </form>
    <button @click="getStudent">get student</button>

  </div>
</template>
<script lang='ts'>
  import Vue from 'vue'

  class Student{
    age!: number;
    name!: string;


    constructor(name: string, age: number){
      this.age = age;
      this.name = name;
    }
  }
  const studentList: Array<Student> = [];
  export default Vue.extend({
    components:{

    },
    data(){
      return {
        count: 0,
        name: 'Truong Uchiha',
        name1:'',
        age:0,
        studentList,
        isActive:true,
        isError:false,
      }
    },
    computed: {
      objClass(): Object {
        return {
          active:this.isActive,
          error:this.isError
        }
      },
    },
    methods: {
      increase(e: Event){
        console.log(e);
        this.count+=1;
      },
      decrease(e: Event){
        console.log(e);
        this.count-=1;
      },
      addStudent(){
        console.log(this.name1 + this.age);
        this.studentList.push(new Student(this.name1,this.age));
      },
      getStudent(e: Event){
        console.log(e);

        console.log(this.studentList);
      },
      changeStateActive(){
        // eslint-disable-next-line no-return-assign
        return this.isActive = !this.isActive
      }
    },
  })
</script>
<style>
  div.container{
    background-color: wheat;
  }
  p{
    color:white;
    font-size: 20px;
    font-family: sans-serif;
  }
  .active{
    color: green;
  }
</style>
