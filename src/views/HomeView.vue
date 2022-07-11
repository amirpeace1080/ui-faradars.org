<template>
  <div>
    <v-img width="100%" height="400" src="https://faradars.org/next/imgs/banner.jpg" />

    <CategoryLearn />

    <span class="subtitle-1 font-weight-bold mt-8" style="margin-right: 150px">آموزش‌های پرمخاطب</span>
    <LearnFullUser />

    <span class="subtitle-1 font-weight-bold mt-8" style="margin-right: 150px">جدیدترین آموزش‌ها</span>
    <LearnFullUser />

    <span class="subtitle-1 font-weight-bold mt-8" style="margin-right: 150px">آموزش‌های پرمخاطب رایگان</span>
    <LearnFullUser />

    <span class="subtitle-1 font-weight-bold mt-8" style="margin-right: 150px">وبینارها</span>
    <LearnFullUser />

    <span class="subtitle-1 font-weight-bold mt-8" style="margin-right: 150px">جدیدترین آموزش‌های رایگان</span>
    <LearnFullUser />

    <span class="subtitle-1 font-weight-bold mt-8" style="margin-right: 150px">آموزش‌های در دست انتشار</span>
    <LearnFullUser />

    <span class="subtitle-1 font-weight-bold mt-8" style="margin-right: 150px">آخرین بازدیدهای شما</span>
    <LearnFullUser />

    <RouteLearn />
  </div>
</template>

<script>
import CategoryLearn from '../components/CategoryLearn.vue'
import LearnFullUser from '../components/LearnFullUser.vue'
import RouteLearn from '../components/RouteLearn.vue'

export default {
  name: "Home",
  components:{
    CategoryLearn,
    LearnFullUser,
    RouteLearn,
  }
};
</script>
