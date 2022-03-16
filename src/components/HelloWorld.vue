<template>
  <div class="hello">
    <el-form :label-position="labelPosition" label-width="100px" :model="car">
      <el-form-item label="Automarke">
        <el-input v-model="car.make"></el-input>
      </el-form-item>
      <el-form-item label="Activity zone">
        <el-input v-model="car.model"></el-input>
      </el-form-item>
      <el-form-item label="Activity form">
        <el-input v-model="car.km"></el-input>
      </el-form-item>
    </el-form>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      car: {
        make: '',
        modek: '',
        km: '',
      }
    }
  },
  methods: {
    onSubmit() {
      console.log('submit!');
    }
  }
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
