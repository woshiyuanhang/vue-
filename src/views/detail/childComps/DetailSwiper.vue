<template>

  <Swiper class="detail-swiper">
    <SwiperItem v-for="item in topImages">
      <img :src="item " alt="">
    </SwiperItem>
  </Swiper>

</template>

<script>
import {Swiper,SwiperItem} from '../../../components/commom/swiper'
export default {
  name: "DetailSwiper",
  components:{
    Swiper,
    SwiperItem
  },
  props:{
    topImages:{
      type:Array,
      default(){
        return[]
      }
    }
  }
}
</script>

<style scoped>
.detail-swiper{
  height: 300px;
  overflow: hidden;
}
</style>
