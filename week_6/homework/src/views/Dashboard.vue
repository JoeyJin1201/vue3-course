<template>
  <div>
    <h1>你現在在後台頁面</h1>
    <div id="nav">
      <router-link to="/">回到前台</router-link> |
      <router-link to="/admin/products">後台產品列表</router-link> |
      <a href="#" @click.prevent="signout">登出</a>
    </div>
    <router-view v-if="checkSuccess"></router-view>
  </div>
</template>

<script>
export default {
  name: 'Dashboard',
  data() {
    return {
      checkSuccess: false,
    };
  },
  created() {
    this.checkLogin();
  },
  methods: {
    checkLogin() {
      const token = document.cookie.replace(/(?:(?:^|.*;\s*)hexToken\s*=\s*([^;]*).*$)|^.*$/, '$1');
      if (token) {
        // Axios 預設值
        this.$http.defaults.headers.common.Authorization = `${token}`;
        const api = `${process.env.VUE_APP_API}api/user/check`;
        this.$http.post(api, { api_token: this.token }).then((res) => {
          if (res.data.success) {
            this.checkSuccess = true;
          } else {
            alert(res.data.message);
            this.$router.push('/login');
          }
        });
      } else {
        alert('您尚未登入。');
        this.$router.push('/login');
      }
    },
    signout() {
      document.cookie = 'hexToken=;expires=;';
      alert('token 已清除');
      this.$router.push('/login');
    },
  },
};
</script>
