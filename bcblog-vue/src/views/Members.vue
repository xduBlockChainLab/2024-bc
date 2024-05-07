<template>
  <div>
    <Header></Header>
    <br/><br/><br/><br/>
    <div class="members-page">
      <h1 class="title">链融工作室2020级毕业去向</h1>
      <div class="university-logos" >
        <div class="logo-container">
          <img src="@/assets/Uni1logo.jpg" alt="中国科学院大学" class="logo">
          <p>洪铭锋：中国科学院大学</p>
        </div>
        <div class="logo-container">
          <img src="@/assets/Uni2logo.png" alt="杜克大学" class="logo">
          <p>王渝普：杜克大学</p>
        </div>
        <div class="logo-container">
          <img src="@/assets/Uni3logo.jpg" alt="宾夕法尼亚大学" class="logo">
          <p>张云儿：宾夕法尼亚大学</p>
        </div>
        <div class="logo-container">
          <img src="@/assets/Uni4logo.jpg" alt="华为" class="logo">
          <p>胡雨安：华为</p>
        </div>
      </div>
      <div class="group">
        <h1 class="group-title">2021级成员</h1>
        <ul>
          <li v-for="name in y2021Group" :key="name">{{ name }}</li>
        </ul>
      </div>
      <div class="group">
        <h1 class="group-title">2022级成员</h1>
        <ul>
          <li v-for="name in y2022Group" :key="name">{{ name }}</li>
        </ul>
      </div>
      <div class="group">
        <h1 class="group-title">2023级成员</h1>
        <ul>
          <li v-for="name in y2023Group" :key="name">{{ name }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<template>
  <div>
    <Header></Header>
    <br/><br/><br/><br/>
    <div class="members-page">
      <h1 class="title">链融工作室2020级毕业去向</h1>
      <div class="university-logos" >
        <div class="logo-container">
          <img src="@/assets/Uni1logo.jpg" alt="中国科学院大学" class="logo">
          <p>洪铭锋：中国科学院大学</p>
        </div>
        <div class="logo-container">
          <img src="@/assets/Uni2logo.png" alt="杜克大学" class="logo">
          <p>王渝普：杜克大学</p>
        </div>
        <div class="logo-container">
          <img src="@/assets/Uni3logo.jpg" alt="宾夕法尼亚大学" class="logo">
          <p>张云儿：宾夕法尼亚大学</p>
        </div>
        <div class="logo-container">
          <img src="@/assets/Uni4logo.jpg" alt="华为" class="logo">
          <p>胡雨安：华为</p>
        </div>
      </div>
      <div class="group">
        <h1 class="group-title">2021级成员</h1>
        <ul>
          <li v-for="name in y2021Group" :key="name">{{ name }}</li>
        </ul>
      </div>
      <div class="group">
        <h1 class="group-title">2022级成员</h1>
        <ul>
          <li v-for="name in y2022Group" :key="name">{{ name }}</li>
        </ul>
      </div>
      <div class="group">
        <h1 class="group-title">2023级成员</h1>
        <ul>
          <li v-for="name in y2023Group" :key="name">{{ name }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "../components/Header";
export default {      
  name: 'Members',
  components: {Header},
  data() {
    return {
      y2021Group: ['张富尧', '魏子翔', '郑屿蓬', '李庆和','覃朗'],
      y2022Group: ['丁旭阳'],
      y2023Group: ['王子姗', '姜灿', '沈新旸']
    };
  }
}
</script>

<style scoped>
.members-page {
  text-align: center;
  padding: 0 120px;
}
.title {
  color: #0056b3;
  font-size: 24px;
  margin-bottom: 10px;
}
.logo-container {
  margin: 10px 5px;
  display: inline-block;
  text-align: center;
}
.logo-container p {
  margin-top: 5px;
  font-size: 16px;
}
.university-logos {
  display: flex;
  justify-content: space-between;
  margin-bottom: 20px;
}
.logo {
  transition: transform 0.3s;
  width: auto;
  height: 120px;
}
.logo:hover {
  transform: scale(1.1);
}
.group {
  background-color: #f0f4f8;
  border-left: 5px solid #0056b3;
  margin-bottom: 20px;
  padding: 10px 20px;
}
.group-title {
  color: #0056b3;
  font-size: 24px;
  margin-bottom: 10px;
}
.group ul {
  list-style-type: none;
  padding: 0;
}
.group li {
  color: #333;
  margin-bottom: 5px;
  font-size: 16px;
}
</style>
