<template>
    <div class="auth-view">
        <div class="auth-container">
            <div class="auth-header">
                <router-link to="/" class="logo">
                    <svg width="28" height="28" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M12 2L2 7V17L12 22L22 17V7L12 2Z" stroke="white" stroke-width="2"
                            stroke-linejoin="round" />
                        <path d="M2 7L12 12L22 7" stroke="white" stroke-width="2" stroke-linejoin="round" />
                        <path d="M12 12V22" stroke="white" stroke-width="2" stroke-linejoin="round" />
                    </svg>
                    <span>ITGPT</span>
                </router-link>
                <h2>开启您的 AI 之旅</h2>
                <p>创建一个账户，探索智能体的无限可能</p>
            </div>

            <form @submit.prevent="handleRegister" class="auth-form">
                <div class="input-group">
                    <label for="username">用户名</label>
                    <input type="text" id="username" v-model="username" placeholder="选择一个用户名" required />
                </div>
                <div class="input-group">
                    <label for="email">邮箱地址</label>
                    <input type="email" id="email" v-model="email" placeholder="you@example.com" required />
                </div>
                <div class="input-group">
                    <label for="password">密码</label>
                    <input type="password" id="password" v-model="password" placeholder="••••••••" required />
                </div>
                <div class="input-group">
                    <label for="confirmPassword">确认密码</label>
                    <input type="password" id="confirmPassword" v-model="confirmPassword" placeholder="••••••••"
                        required />
                </div>

                <button type="submit" class="cta-button">立即注册</button>
            </form>

            <div class="auth-footer">
                <p>已经有账户了？ <router-link to="/login">立即登录</router-link></p>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'
import { RouterLink, useRouter } from 'vue-router'

const router = useRouter()
const username = ref('')
const email = ref('')
const password = ref('')
const confirmPassword = ref('')

const handleRegister = () => {
    // TODO: Implement actual registration logic
    if (password.value !== confirmPassword.value) {
        alert("Passwords do not match!");
        return;
    }
    console.log('Registering with:', username.value, email.value, password.value)
    // Redirect to a dashboard or home page after successful registration
    router.push('/')
}
</script>

<style scoped>
/* Styles are identical to LoginView.vue for consistency */
.auth-view {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    background: radial-gradient(ellipse at 50% 50%, #0a0a0a 0%, #000000 70%);
    padding: 2rem;
}

.auth-container {
    max-width: 450px;
    width: 100%;
    background: rgba(255, 255, 255, 0.03);
    border: 1px solid var(--color-border);
    border-radius: 16px;
    padding: 3rem;
    backdrop-filter: blur(10px);
    position: relative;
    overflow: hidden;
}

.auth-container::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(0, 123, 255, 0.1), transparent 30%);
    animation: rotate-glow 10s linear infinite;
}

@keyframes rotate-glow {
    from {
        transform: rotate(0deg);
    }

    to {
        transform: rotate(360deg);
    }
}

.auth-header {
    text-align: center;
    margin-bottom: 2rem;
}

.logo {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.75rem;
    color: #FFFFFF;
    font-family: var(--font-heading);
    font-weight: 600;
    font-size: 1.5rem;
    text-decoration: none;
    margin-bottom: 1.5rem;
}

.auth-header h2 {
    font-size: 2rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
}

.auth-header p {
    color: var(--color-text);
    opacity: 0.8;
}

.auth-form {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
}

.input-group {
    display: flex;
    flex-direction: column;
}

.input-group label {
    margin-bottom: 0.5rem;
    font-weight: 500;
    font-size: 0.9rem;
}

.input-group input {
    padding: 0.8rem 1rem;
    background: rgba(0, 0, 0, 0.3);
    border: 1px solid var(--color-border);
    border-radius: 8px;
    color: #FFFFFF;
    font-size: 1rem;
    transition: all 0.3s ease;
}

.input-group input:focus {
    outline: none;
    border-color: var(--color-primary);
    box-shadow: 0 0 10px var(--color-glow);
}

.cta-button {
    padding: 1rem;
    margin-top: 1rem;
    background: linear-gradient(135deg, var(--color-primary), #4DA8FF);
    color: #FFFFFF;
    border: none;
    border-radius: 8px;
    font-size: 1rem;
    font-weight: 600;
    cursor: pointer;
    transition: all 0.3s ease;
    box-shadow: 0 0 20px var(--color-glow);
}

.cta-button:hover {
    transform: translateY(-3px);
    box-shadow: 0 0 30px var(--color-glow);
}

.auth-footer {
    margin-top: 2rem;
    text-align: center;
    font-size: 0.9rem;
}

.auth-footer a {
    color: var(--color-primary);
    font-weight: 600;
}
</style>
