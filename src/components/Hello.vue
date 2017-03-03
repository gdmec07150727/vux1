<template>
   <div>
     <span class="title">
       欢迎登陆
     </span>
     <divider>Vue Vux</divider>
     <Group>
       <XInput title="账号" v-model='account' placeholder='账号' type='text'>
       </XInput>
     </Group>
     <x-input title="密码" v-model="password" placeholder="密码" type="password"/>
     <XButton type="primary" action-type="button">登录</XButton>
   </div>
</template>

<script>
  import { Divider, Group, XInput, XButton } from 'vux'
  export default {
    components: {
      Divider,
      Group,
      XInput,
      XButton
    },
    data () {
      return {
        account: '',
        password: '' 
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
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
