<template>
    <div>
      <Header></Header>
      <div class="showcase">
    <header class="header">
      <!-- <img src="@/assets/logo.png" alt="公司logo" class="logo"> -->
      <h1>成果展示</h1>
    </header>
    <div class="projects-container">
      <div class="project-card" v-for="project in projects" :key="project.id">
        <img :src="project.image" :alt="project.title" class="project-image">
        <div class="project-info">
          <h3>{{ project.title }}</h3>
          <p>{{ project.description }}</p>
        </div>
      </div>
    </div>
    <footer class="footer">
      © {{ new Date().getFullYear() }} 公司名. 版权所有.
    </footer>
  </div>
    </div>
  </template>
  
  
  <script>
  import Header from "../components/Header";
  export default {
    name: 'Achievement',
    components: {Header},
    data() {
    return {
      projects: [
        { id: 1, title: '互联网+', description: '第八届中国国际“互联网+”大学生创新创业大赛国际铜奖', image: '@/assets/project1.jpg' },
        { id: 2, title: '项目二', description: '第九届中国国际“互联网+”大学生创新创业大赛陕西省银奖', image: '@/assets/project2.jpg' },
        { id: 3, title: '项目三', description: '入选首届蚂蚁链Web3.0与产业创新应用孵化营,入围微众银行2022 FinTechaton金融科技高校大赛',
image: '@/assets/project3.jpg' }
      ]
    }
  }
}
  
  </script>
  
  <style scoped>
.showcase {
  text-align: center;
  font-family: 'Arial', sans-serif;
  background-color: #f4f9fd; /* 浅蓝色的底色 */
}

.header {
  background-color: #e0f2fe; /* 更浅的蓝色背景 */
  padding: 20px;
  text-align: center;
}

.logo {
  width: 100px;
}

.projects-container {
  display: flex;
  justify-content: space-around;
  padding: 20px;
}

.project-card {
  width: 30%;
  background-color: #ffffff; /* 白色背景 */
  box-shadow: 0 4px 8px rgba(0, 123, 255, 0.2); /* 浅蓝色阴影 */
  border: 1px solid #b3e5fc; /* 浅蓝色边框 */
  margin: 20px;
  padding: 20px;
  border-radius: 8px; /* 圆角边框 */
}

.project-image {
  width: 100%;
  height: auto;
  border-top-left-radius: 8px;
  border-top-right-radius: 8px;
}

.project-info h3 {
  color: #0277bd; /* 深蓝色字体 */
}

.project-info p {
  color: #546e7a; /* 深灰蓝色字体 */
}

.footer {
  background-color: #e0f2fe; /* 浅蓝色背景 */
  color: #ffffff; /* 白色字体 */
  padding: 10px;
  text-align: center;
  position: fixed;
  bottom: 0;
  width: 100%;
}
</style>
