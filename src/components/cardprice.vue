<template>
<el-row>
  <el-col :span="5" v-for="(o, index) in 4" :key="o" :offset="index > 0 ? 1: 0.8">
    <el-card :body-style="{ padding: '10px' }" shadow="hover">
        <img :src="cardsrcs[index].path" class="image">
    </el-card>
  </el-col>
</el-row>
</template>

<script>
export default{
  data() {
    return {
      cardsrcs:[
        {
          path: require('../assets/bods/1.png')
        },
        {
          path: require('../assets/bods/4.png')
        },
        {
          path: require('../assets/bods/1.png')
        },
        {
          path: require('../assets/bods/4.png')
        }
      ]
    }
  }
}
</script>

<style scoped>

  .image {
    width: 100%;
    display: block;
  }

  .clearfix:before,
  .clearfix:after {
      display: table;
      content: "";
  }
  
  .clearfix:after {
      clear: both
  }
</style>