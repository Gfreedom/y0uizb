<template>
  <el-row>
  <el-col :span="6" v-for="(o, index) in 6" :key="o" :offset="(index % 3) > 0 ? 2 : 1">
    <el-card :body-style="{ padding: '10px' }" shadow="hover" class="box-card">
        <a>
          <img :src="cardsrcs[index].path" class="image">
        </a>
        <div >{{ cardsrcs[index].name }}</div>
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
          name: '1 Rolled Spline Dimensions LC1500A',
          path: require('../assets/bodright/1.jpg')
        },
        {
          name: '2 Horizontal Oil Pressure Rock Rolling Machine LC100',
          path: require('../assets/bodright/2.jpg')
        },
        {
          name: '3 Cage Window Milling Machine QXG125',
          path: require('../assets/bodright/3.jpg')
        },
        {
          name: '4 Spline Rolling Machine',
          path: require('../assets/bodright/4.jpg')
        },
        {
          name: '5 Spline',
          path: require('../assets/bodright/5.jpg')
        },
        {
          name: '6 Blank Die',
          path: require('../assets/bodright/6.jpg')
        }
      ]
    }
  }
}
</script>

<style>
  <style scoped>

  .image {
    width: 180px;
    height: 180px;
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
  .box-card{

    width: 250px;
    height: 280px;
  }

</style>