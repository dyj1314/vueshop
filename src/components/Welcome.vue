<template>
    <div>
      <!-- 轮播图 -->
      <div class="block">
        <el-carousel height="90vh">
          <el-carousel-item v-for="item in swiperList" :key="item.id">
            <img class="swiper-img" :src="item.img">
          </el-carousel-item>
        </el-carousel>
      </div>
    </div>
</template>
<script>
export default {
  data () {
    return {
      swiperList: [
        { id: '001', 
          img: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1599291267952&di=0a616b03dc088f9006f08940c8308b67&imgtype=0&src=http%3A%2F%2Fd.hiphotos.baidu.com%2Fzhidao%2Fpic%2Fitem%2Ff31fbe096b63f624b8c765b08c44ebf81b4ca3ef.jpg' },
        { id: '002', 
          img: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1599291319958&di=27586d5f30106bc0928933d3f0ad0459&imgtype=0&src=http%3A%2F%2Fimage11.m1905.com%2Fuploadfile%2Fs2010%2F0419%2F20100419085618596.jpg' }
      ]
    }
  }
}
</script>
<style lang="less" scoped>
  .swiper-img {
    width: 100%;
    height: 100%;
  }
</style>
