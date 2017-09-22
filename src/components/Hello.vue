<template>
  <div>
    <div class='centered1'> {{ updatedTime1 }} </div>
    <div class='centered2'> {{ updatedTime2 }} </div>
    <div class='centered3'> {{ updateDate }} </div>
    <!-- <div class="battery"> {{ updatedBattery }} % </div> -->
  </div>
</template>

<script>
import moment from 'moment'
export default {
  name: 'hello',
  data () {
    return {
    }
  },
  computed: {
    updatedTime1 () {
      return moment().format('H')
    },
    updatedTime2 () {
      return moment().format('mm')
    },
    updateDate () {
      return moment().format('dddd, Do MMMM YYYY')
    }
  }
}
</script>

<!-- Add 'scoped' attribute to limit CSS to this component only -->
<style scoped>

.centered1 {
  position: fixed;
  top: 45%;
  left: 50%;
  /* bring your own prefixes */
  transform: translate(-50%, -50%);
  color: #fff;
  font-size: 50px;
  padding-left: 0px;
}

.centered2 {
  position: fixed;
  top: 52%;
  left: 50%;
  /* bring your own prefixes */
  transform: translate(-50%, -50%);
  color: #fff;
  font-size: 50px;
  padding-left: 0px;
}
.centered3 {
  position: fixed;
  top: 60%;
  left: 50%;
  /* bring your own prefixes */
  transform: translate(-50%, -50%);
  color: #fff;
  font-size: 12px;
  padding-left: 0px;
}

.battery {
  position: fixed;
  top: 63%;
  left: 50%;
  /* bring your own prefixes */
  transform: translate(-50%, -50%);
  color: #fff;
  font-size: 12px;
  padding-left: 0px;
}

</style>
