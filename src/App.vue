<template>
  <div class="" style="overflow: hidden">
    <div class="" style="height: 300px"></div>
    <div class="" style="height: 200px"></div>

    <div class="flex-wrapper">
      <div class="box-1" v-scroll-ease="{ rotate: 360 }">
        360 rotate
      </div>
    </div>
    <div class="" style="height: 300px"></div>

    <div class="flex-wrapper">
      <div class="box-2" v-scroll-ease="{ from: 500, direction: 'right' }">
        right 500
      </div>
    </div>
    <div class="" style="height: 300px"></div>
    <div class="flex-wrapper" style="justify-content: flex-end">
      <div class="box-2" v-scroll-ease="{ from: 500, direction: 'left' }">
        left 500
      </div>
    </div>
    <div class="" style="height: 300px"></div>
    <div class="flex-wrapper">
      <div class="box-3" v-scroll-ease="{ from: 500, direction: 'right', rotate: 30 }">
        right 500 rotate 30
      </div>
    </div>

    <div class="flex-wrapper" style="justify-content: flex-end">
      <div class="box-4" v-scroll-ease="{ from: 500, direction: 'left', rotate: -180, delay: 300 }">
        left 500 rotate -180 delay 300
      </div>
    </div>
    <div class="" style="height: 300px"></div>
  </div>
</template>


<style scoped lang="scss">
.flex-wrapper {
  display: flex;
  flex-wrap: wrap;
  gap: 20px; /* Space between items */
  margin: 20px;
  .box-1 {
    width: 300px;
    height: 300px;
    background: black;
  }

  .box-2 {
    width: 300px;
    height: 300px;
    background: red;
  }

  .box-3 {
    width: 300px;
    height: 300px;
    background: red;
  }
  .box-4 {
    width: 300px;
    height: 300px;
    background: red;
  }
}
</style>