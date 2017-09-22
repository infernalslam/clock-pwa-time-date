<template>
  <div>
    <div class="centered1">
      10
    </div>
    <div class="centered2">
      17
    </div>
    <div class="centered3"> {{ date }} </div>
  </div>
</template>

<script>
import moment from 'moment'
export default {
  name: 'hello',
  data () {
    return {
      date: moment().format('LLLL')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
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

</style>
