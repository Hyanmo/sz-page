<template>
  <div id="app">
    <header class="site-header">
      <h1>门外的专属小站</h1>
      <p class="subtitle">由狗老师亲手打造</p>
    </header>

    <section class="profile">
      <img class="avatar" src="./assets/avatar.png" alt="门外大人头像">
      <h2>门外</h2>
      <p>Bonjour 门外饱饱～</p>
      <p>希望你能天天开心。</p>
    </section>

    <section class="links">
      <h3>🐾 狗老师精心准备的链接</h3>
      <ul>
        <li><a href="https://github.com/Hyanmo" target="_blank">狗老师的 GitHub</a></li>
        <li><a href="https://hyanmo.github.io/sz-page" target="_blank">本站地址</a></li>
      </ul>
    </section>

    <footer class="site-footer">
      © 2025 狗老师特别献给门外大人 | 永远支持你
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style scoped>
#app {
  font-family: 'Helvetica Neue', Avenir, sans-serif;
  text-align: center;
  color: #333;
  background-color: #fdfcf8;
  min-height: 100vh;
  padding: 20px;
}

/* Header */
.site-header {
  margin-bottom: 40px;
}

.site-header h1 {
  font-size: 32px;
  color: #5c8374;
  margin-bottom: 10px;
}

.subtitle {
  font-size: 16px;
  color: #999;
}

/* Profile Section */
.profile {
  margin-bottom: 40px;
}

.avatar {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid #d2dedb;
  margin-bottom: 10px;
}

/* Links Section */
.links ul {
  list-style: none;
  padding: 0;
}

.links li {
  margin: 10px 0;
}

.links a {
  color: #4b7064;
  text-decoration: none;
  font-weight: bold;
}

.links a:hover {
  text-decoration: underline;
}

/* Footer */
.site-footer {
  margin-top: 60px;
  padding: 20px;
  font-size: 14px;
  color: #aaa;
  border-top: 1px solid #eee;
}
</style>
