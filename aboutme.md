---
layout: page
title: 关于我
subtitle: 你好呀，欢迎来到我的小世界
---

你好！我是大帅哥 👋

我喜欢看剧、旅游和打游戏～

---

<!-- 导航标签 -->
<div class="tab-nav">
  <button class="tab-btn active" onclick="openTab(event, 'about')">📖 个人介绍</button>
  <button class="tab-btn" onclick="openTab(event, 'travel')">✈️ 旅游</button>
  <button class="tab-btn" onclick="openTab(event, 'game')">🎮 游戏</button>
</div>

<!-- 个人介绍内容 -->
<div id="about" class="tab-content" style="display: block;">
  <p>你好！我是马笑杰，河北张家口人，目前在河北工程技术学院读网络工程，即将毕业。</p>
  
  <p>我喜欢研究网络怎么"跑"得更稳、更快，也喜欢动手搭环境、做实验。从 VLAN 划分到 VRRP 冗余，从防火墙策略到无线 AP 配置，这些事做起来挺有意思的。</p>
  
  <p>最近在折腾 Zabbix 监控和 Docker 容器，也在用 AI 帮忙写文档、查资料，确实是提高效率的好工具。</p>
  
  <p>这个博客会记录我的一些学习笔记、项目实践和生活感悟，欢迎来聊～</p>
</div>

<!-- 旅游内容 -->
<div id="travel" class="tab-content" style="display: none;">
  <h2>打卡武汉</h2>
  <p>今天去了武汉，记录一下～</p>
  <h3>去了哪些地方</h3>
  <ul>
    <li>黄鹤楼</li>
    <li>长江大桥</li>
    <li>户部巷</li>
    <li>东湖绿道</li>
  </ul>
  <h3>吃了什么</h3>
  <ul>
    <li>热干面</li>
    <li>三鲜豆皮</li>
    <li>糊汤粉</li>
  </ul>
  <p><img src="/assets/img/63068c85320872f957a341294ff55876.jpg" alt="武汉街景" style="max-width: 100%; border-radius: 8px;" /></p>
  <p>下次再来玩～</p>
</div>

<!-- 游戏内容 -->
<div id="game" class="tab-content" style="display: none;">
  <h2>最近在玩什么 🎮</h2>
  <ul>
    <li>🎯 <strong>王者荣耀</strong> - 我是百星高手</li>
    <li>🎯 <strong>金铲铲</strong> - 宗师在榜</li>
  <p>你最近在玩什么？欢迎推荐给我～</p>
</div>

<!-- CSS 样式（控制标签样式） -->
<style>
.tab-nav {
  display: flex;
  gap: 6px;
  border-bottom: 2px solid #e5e5ea;
  padding-bottom: 0;
  margin: 20px 0 16px 0;
  flex-wrap: wrap;
}
.tab-btn {
  background: transparent;
  border: none;
  padding: 8px 18px;
  font-size: 15px;
  font-weight: 500;
  color: #6e6e73;
  cursor: pointer;
  border-radius: 20px 20px 0 0;
  transition: all 0.2s;
}
.tab-btn:hover {
  color: #1d1d1f;
  background: #f0f0f2;
}
.tab-btn.active {
  color: #007aff;
  background: #e8f2ff;
  border-bottom: 3px solid #007aff;
}
.tab-content {
  padding-top: 12px;
}
.tab-content h2 {
  font-size: 1.4rem;
  margin-bottom: 8px;
}
.tab-content ul {
  padding-left: 20px;
}
.tab-content li {
  margin-bottom: 4px;
}
</style>

<!-- JavaScript（控制标签切换） -->
<script>
function openTab(evt, tabName) {
  // 隐藏所有标签内容
  var contents = document.getElementsByClassName("tab-content");
  for (var i = 0; i < contents.length; i++) {
    contents[i].style.display = "none";
  }
  // 移除所有标签的 active 样式
  var btns = document.getElementsByClassName("tab-btn");
  for (var i = 0; i < btns.length; i++) {
    btns[i].className = btns[i].className.replace(" active", "");
  }
  // 显示当前选中的标签内容
  document.getElementById(tabName).style.display = "block";
  // 给当前点击的标签添加 active 样式
  evt.currentTarget.className += " active";
}
</script>
