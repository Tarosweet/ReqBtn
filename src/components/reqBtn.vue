<template>
  <div class="hello">
    <el-button style="width: 20%; margin-top: 40px" @click="Request" type="primary">Send Request</el-button>
  </div>
</template>

<script>
  import axios from 'axios';
export default {
  name: 'HelloWorld',
  data() {
    return {
      data: {}
    }
  },
  methods: {
    Request() {
      let url = 'http://localhost:8088/test';
      axios.post(url, this.data, {}).then(res => {
        if(res.status === 200)
          this.$message.success('Send request success!');
      }).catch(err => {
        console.log(err);
      });
    }
  }
}
</script>
