<template>
    <section class="hero">
        <div class="background-animation">
            <div class="gradient-orb orb-1"></div>
            <div class="gradient-orb orb-2"></div>
            <div class="gradient-orb orb-3"></div>
            <div class="grid-pattern"></div>
        </div>
        <div class="container hero-content">
            <div class="hero-badge">
                <span class="badge-text">🚀 AI 驱动</span>
                <span class="badge-dot"></span>
            </div>
            <h1 class="hero-title">
                <span class="title-line">AI 智能体</span>
                <span class="title-line highlight">一站式开发平台</span>
            </h1>
            <p class="hero-subtitle">
                从灵感到现实，一键构建、部署并扩展您的专属 AI 智能体。
                <br>无需编码，让 AI 为您创造无限可能。
            </p>
            <div class="hero-actions">
                <router-link to="/login" class="cta-button primary">
                    <span>立即开始</span>
                    <svg class="arrow-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd"
                            d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                            clip-rule="evenodd" />
                    </svg>
                </router-link>
                <a href="#features" class="cta-button secondary">
                    <span>探索特性</span>
                    <svg class="play-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd"
                            d="M10 18a8 8 0 100-16 8 8 0 000 16zM9.555 7.168A1 1 0 008 8v4a1 1 0 001.555.832l3-2a1 1 0 000-1.664l-3-2z"
                            clip-rule="evenodd" />
                    </svg>
                </a>
            </div>
            <div class="hero-stats">
                <div class="stat-item">
                    <span class="stat-number">10K+</span>
                    <span class="stat-label">活跃用户</span>
                </div>
                <div class="stat-item">
                    <span class="stat-number">50K+</span>
                    <span class="stat-label">智能体创建</span>
                </div>
                <div class="stat-item">
                    <span class="stat-number">99.9%</span>
                    <span class="stat-label">运行时间</span>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import { RouterLink } from 'vue-router';
</script>

<style scoped>
.hero {
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    padding-top: 80px;
    text-align: center;
    overflow: hidden;
    background: radial-gradient(ellipse at 50% 50%, #0a0a0a 0%, #000000 70%);
}

.background-animation {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 0;
}

.gradient-orb {
    position: absolute;
    border-radius: 50%;
    filter: blur(40px);
    opacity: 0.3;
    animation: float 6s ease-in-out infinite;
}

.orb-1 {
    width: 300px;
    height: 300px;
    background: radial-gradient(circle, #007BFF 0%, transparent 70%);
    top: 20%;
    left: 10%;
    animation-delay: 0s;
}

.orb-2 {
    width: 200px;
    height: 200px;
    background: radial-gradient(circle, #4DA8FF 0%, transparent 70%);
    top: 60%;
    right: 15%;
    animation-delay: 2s;
}

.orb-3 {
    width: 150px;
    height: 150px;
    background: radial-gradient(circle, #00D4FF 0%, transparent 70%);
    bottom: 20%;
    left: 20%;
    animation-delay: 4s;
}

.grid-pattern {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-image:
        linear-gradient(rgba(255, 255, 255, 0.03) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255, 255, 255, 0.03) 1px, transparent 1px);
    background-size: 50px 50px;
    animation: grid-move 20s linear infinite;
}

@keyframes float {

    0%,
    100% {
        transform: translateY(0px) rotate(0deg);
    }

    50% {
        transform: translateY(-20px) rotate(180deg);
    }
}

@keyframes grid-move {
    0% {
        transform: translate(0, 0);
    }

    100% {
        transform: translate(50px, 50px);
    }
}

.hero-content {
    position: relative;
    z-index: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    max-width: 800px;
}

.hero-badge {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    background: rgba(255, 255, 255, 0.1);
    border: 1px solid rgba(255, 255, 255, 0.2);
    border-radius: 50px;
    padding: 0.5rem 1rem;
    margin-bottom: 2rem;
    backdrop-filter: blur(10px);
}

.badge-text {
    font-size: 0.9rem;
    font-weight: 500;
    color: #FFFFFF;
}

.badge-dot {
    width: 6px;
    height: 6px;
    background: var(--color-primary);
    border-radius: 50%;
    animation: pulse 2s infinite;
}

@keyframes pulse {

    0%,
    100% {
        opacity: 1;
    }

    50% {
        opacity: 0.5;
    }
}

.hero-title {
    font-size: clamp(3rem, 8vw, 5rem);
    font-weight: 700;
    line-height: 1.1;
    margin-bottom: 1.5rem;
    text-shadow: 0 0 30px rgba(255, 255, 255, 0.3);
}

.title-line {
    display: block;
    color: #FFFFFF;
}

.title-line.highlight {
    background: linear-gradient(135deg, #007BFF, #00D4FF);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.hero-subtitle {
    font-size: clamp(1.1rem, 2.5vw, 1.4rem);
    color: var(--color-text);
    max-width: 600px;
    margin-bottom: 3rem;
    line-height: 1.6;
    opacity: 0.9;
}

.hero-actions {
    display: flex;
    gap: 1rem;
    margin-bottom: 4rem;
    flex-wrap: wrap;
    justify-content: center;
}

.cta-button {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    padding: 1rem 2rem;
    border-radius: 12px;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s ease;
    font-size: 1rem;
    position: relative;
    overflow: hidden;
}

.cta-button.primary {
    background: linear-gradient(135deg, var(--color-primary), #4DA8FF);
    color: #FFFFFF;
    box-shadow: 0 0 30px var(--color-glow);
}

.cta-button.primary:hover {
    transform: translateY(-3px);
    box-shadow: 0 0 50px var(--color-glow);
}

.cta-button.secondary {
    background: rgba(255, 255, 255, 0.1);
    color: #FFFFFF;
    border: 1px solid rgba(255, 255, 255, 0.2);
    backdrop-filter: blur(10px);
}

.cta-button.secondary:hover {
    background: rgba(255, 255, 255, 0.2);
    transform: translateY(-3px);
}

.arrow-icon,
.play-icon {
    width: 20px;
    height: 20px;
    transition: transform 0.3s ease;
}

.cta-button:hover .arrow-icon {
    transform: translateX(3px);
}

.cta-button:hover .play-icon {
    transform: scale(1.1);
}

.hero-stats {
    display: flex;
    gap: 3rem;
    justify-content: center;
    flex-wrap: wrap;
}

.stat-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0.5rem;
}

.stat-number {
    font-size: 2rem;
    font-weight: 700;
    color: #FFFFFF;
    font-family: var(--font-heading);
}

.stat-label {
    font-size: 0.9rem;
    color: var(--color-text);
    opacity: 0.8;
}

@media (max-width: 768px) {
    .hero-actions {
        flex-direction: column;
        align-items: center;
    }

    .hero-stats {
        gap: 2rem;
    }

    .stat-number {
        font-size: 1.5rem;
    }
}
</style>
