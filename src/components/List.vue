<template>
<div class="text-center container">
  <b-button variant="primary" md="6">
    Items Count <b-badge variant="light">{{count}}</b-badge>
  </b-button>
  <b-form @submit.prevent="">
  <b-form-group
      id="fieldset-horizontal"
      label="List"
      label-for="input-horizontal"
    >
      <b-form-input id="input-horizontal" 
      type="text" v-model="name" placeholder="Enter Item Name" 
      required @keyup.enter="name == '' ? '' : add()"></b-form-input>
    </b-form-group>
      <b-button variant="info" :disabled="check" @click="add()" md="4">Add+</b-button><br><br>

  </b-form>
  <b-list-group>
    <b-list-group-item v-for="(item,index) in items" v-bind:key="index">
       {{ item }}
</b-list-group-item>
  </b-list-group>
</div>


</template>
<script>
export default {
  name: "List",
  data(){
    return{
      name: '',
      items: []
    }
  },
  computed:{
    check(){
      if(this.name == ''){
        return true
      }
      else{
        return false
      }
      },
        count(){
    return this.items.length
    }
  },

  methods:{
    add(){
      this.items.push(this.name)
      this.name= ''
    }
  }

};

</script>
<style scoped>

</style>