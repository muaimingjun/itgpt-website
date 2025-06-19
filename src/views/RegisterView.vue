<template>
  <div class="register-view">
    <div class="register-container">
      <div class="register-form">
        <h1 class="title">创建账户</h1>
        <p class="subtitle">加入 ITGPT，开启您的 AI 之旅</p>
        <form @submit.prevent="handleRegister">
          <div class="input-group">
            <label for="name">全名</label>
            <input type="text" id="name" v-model="name" required placeholder="请输入您的姓名">
          </div>
          <div class="input-group">
            <label for="email">邮箱地址</label>
            <input type="email" id="email" v-model="email" required placeholder="you@example.com">
          </div>
          <div class="input-group">
            <label for="password">密码</label>
            <input type="password" id="password" v-model="password" required placeholder="至少8个字符">
          </div>
           <div class="input-group">
            <label for="confirm-password">确认密码</label>
            <input type="password" id="confirm-password" v-model="confirmPassword" required placeholder="再次输入密码">
          </div>
          <button type="submit" class="cta-button">立即注册</button>
        </form>
        <p class="signin-link">
          已经有账户了？ <router-link to="/login">立即登录</router-link>
        </p>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { useRouter } from 'vue-router';

const router = useRouter();
const name = ref('');
const email = ref('');
const password = ref('');
const confirmPassword = ref('');

const handleRegister = () => {
  if (password.value !== confirmPassword.value) {
    alert("Passwords do not match!");
    return;
  }
  // Handle register logic here
  console.log('Registering with:', name.value, email.value, password.value);
  // On success, redirect to login or home
  // router.push('/login');
};
</script>

<style scoped>
.register-view {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  padding-top: 80px; /* Header offset */
  background: #000;
  position: relative;
  overflow: hidden;
}

.register-view::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle, rgba(63, 94, 251, 0.3) 0%, rgba(252, 70, 107, 0) 60%),
              radial-gradient(circle at top right, rgba(76, 175, 80, 0.3) 0%, rgba(252, 70, 107, 0) 70%),
              radial-gradient(circle at bottom left, rgba(255, 193, 7, 0.3) 0%, rgba(252, 70, 107, 0) 70%);
  animation: rotate 20s linear infinite;
}

@keyframes rotate {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

.register-container {
  max-width: 480px;
  width: 100%;
  padding: 2rem;
  z-index: 1;
}

.register-form {
  background: rgba(10, 10, 25, 0.6);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 16px;
  padding: 2.5rem;
  backdrop-filter: blur(20px) saturate(180%);
  -webkit-backdrop-filter: blur(20px) saturate(180%);
  text-align: center;
  box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
  animation: fadeInScaleUp 0.5s ease-out forwards;
}

@keyframes fadeInScaleUp {
  from {
    opacity: 0;
    transform: scale(0.95) translateY(10px);
  }
  to {
    opacity: 1;
    transform: scale(1) translateY(0);
  }
}

.title {
  font-size: 2.5rem;
  font-weight: 700;
  margin-bottom: 0.5rem;
}

.subtitle {
  color: var(--color-text);
  margin-bottom: 2.5rem;
}

.input-group {
  margin-bottom: 1.5rem;
  text-align: left;
}

.input-group label {
  display: block;
  margin-bottom: 0.5rem;
  font-weight: 500;
  color: #FFFFFF;
}

.input-group input {
  width: 100%;
  padding: 0.8rem 1rem;
  background: rgba(0, 0, 0, 0.3);
  border: 1px solid var(--color-border);
  border-radius: 6px;
  color: #FFFFFF;
  font-size: 1rem;
  transition: border-color 0.3s, box-shadow 0.3s;
}

.input-group input:focus {
  outline: none;
  border-color: var(--color-primary);
  box-shadow: 0 0 10px var(--color-glow);
}

.cta-button {
  width: 100%;
  padding: 0.8rem 2rem;
  border-radius: 8px;
  border: none;
  background: var(--color-primary);
  color: #FFFFFF;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
  font-size: 1rem;
  box-shadow: 0 0 20px var(--color-glow);
}

.cta-button:hover {
  background: #4DA8FF;
  transform: translateY(-3px);
}

.signin-link {
  margin-top: 2rem;
  color: var(--color-text);
}

.signin-link a {
  color: var(--color-primary);
  font-weight: 600;
  text-decoration: none;
}

.signin-link a:hover {
  text-decoration: underline;
}

.input-group input::placeholder {
  color: rgba(255, 255, 255, 0.4);
}
</style>
