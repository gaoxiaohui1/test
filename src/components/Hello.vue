<template>
  <div class="hello">
    <h1>hello:{{ msg }}</h1>
    <button @click="doSend" :disabled="isVCSend">{{msg}}</button>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: '获取手机动态码',
      isVCSend: false,
      sec: 10,
      clock: ''
    }
  },
  methods: {
    doSend () {
      this.isVCSend = true
      this.msg = this.sec + '秒后可重新获取'
      this.clock = setInterval(this.countDown, 1000)
    },
    countDown () {
      this.sec--
      if (this.sec > 0) {
        this.msg = this.sec + '秒后可重新获取'
      } else {
        clearInterval(this.clock)
        this.isVCSend = false
        this.msg = '获取手机动态码'
        this.sec = 10
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
