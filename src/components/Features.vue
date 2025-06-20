<template>
    <section id="features" class="features">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">核心特性</h2>
                <p class="section-subtitle">构建下一代 AI 应用所需的一切</p>
            </div>

            <div class="features-grid">
                <!-- Feature 1: Visual Workflow -->
                <div class="feature-card large-card">
                    <div class="card-content">
                        <h3>可视化工作流</h3>
                        <p>通过拖拽式界面构建复杂的 AI 工作流，无需编码。实时预览您的智能体行为。</p>
                        <a href="#" class="learn-more">
                            了解更多
                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"
                                class="arrow-icon">
                                <path fill-rule="evenodd"
                                    d="M3 10a.75.75 0 01.75-.75h10.638L10.23 5.29a.75.75 0 111.04-1.08l5.5 5.25a.75.75 0 010 1.08l-5.5 5.25a.75.75 0 11-1.04-1.08l4.158-3.96H3.75A.75.75 0 013 10z"
                                    clip-rule="evenodd" />
                            </svg>
                        </a>
                    </div>
                    <div class="card-visual">
                        <img src="https://images.unsplash.com/photo-1678483749293-485a3c43b3b2?q=80&w=1932&auto=format&fit=crop"
                            alt="Visual Workflow" />
                    </div>
                </div>

                <!-- Feature 2: Multi-Model Support -->
                <div class="feature-card">
                    <div class="card-content">
                        <h3>多模型支持</h3>
                        <p>无缝集成主流大语言模型，或接入您的私有模型。</p>
                    </div>
                    <div class="card-icon">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M6.429 9.75L2.25 12l4.179 2.25m0-4.5l5.571 3 5.571-3m-11.142 0L2.25 12l4.179 2.25M6.429 15.75l5.571-3m-5.571 3l-4.179-2.25M21.75 12l-5.571 3-5.571-3 5.571-3 5.571 3z" />
                        </svg>
                    </div>
                </div>

                <!-- Feature 3: One-Click Deployment -->
                <div class="feature-card">
                    <div class="card-content">
                        <h3>一键部署</h3>
                        <p>将您的智能体快速发布到多个平台和渠道。</p>
                    </div>
                    <div class="card-icon">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M9 17.25v1.5m3.75-13.5l-3.75 3.75m3.75-3.75L16.5 7.5M12 21v-1.5m3.75-13.5l-3.75 3.75M12 3v1.5m-3.75 13.5l3.75-3.75m-3.75 3.75L7.5 16.5m9-9l-3.75 3.75M3 12h1.5m16.5 0h-1.5m-12 5.25v-1.5m3.75 0l-3.75-3.75m3.75 3.75l3.75-3.75M12 6v1.5m-3.75 5.25l3.75-3.75m-3.75 3.75L7.5 9m9 9l3.75-3.75" />
                        </svg>
                    </div>
                </div>

                <!-- Feature 4: Enterprise Security -->
                <div class="feature-card">
                    <div class="card-content">
                        <h3>企业级安全</h3>
                        <p>提供数据隔离、加密和访问控制，确保数据安全。</p>
                    </div>
                    <div class="card-icon">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M9 12.75L11.25 15 15 9.75m-3-7.036A11.959 11.959 0 013.598 6 11.99 11.99 0 003 9.749c0 5.592 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.31-.21-2.571-.598-3.751h-.152c-3.196 0-6.1-1.248-8.25-3.286z" />
                        </svg>
                    </div>
                </div>

                <!-- Feature 5: Real-time Analytics -->
                <div class="feature-card">
                    <div class="card-content">
                        <h3>实时分析</h3>
                        <p>监控智能体性能，获取用户交互数据洞察。</p>
                    </div>
                    <div class="card-icon">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M7.5 14.25v2.25m3-4.5v4.5m3-6.75v6.75m3-9v9M6 20.25h12A2.25 2.25 0 0020.25 18V5.75A2.25 2.25 0 0018 3.5H6A2.25 2.25 0 003.75 5.75v12.5A2.25 2.25 0 006 20.25z" />
                        </svg>
                    </div>
                </div>

            </div>
        </div>
    </section>
</template>

<script setup>
// No script logic needed
</script>

<style scoped>
.features {
    padding: var(--section-gap) 0;
    position: relative;
    overflow: hidden;
    background: #000;
}

.section-header {
    text-align: center;
    margin-bottom: 4rem;
}

.section-title {
    font-size: clamp(2.5rem, 6vw, 3.5rem);
    font-weight: 700;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, #FFFFFF, #007BFF);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.section-subtitle {
    font-size: clamp(1rem, 2.5vw, 1.2rem);
    color: var(--color-text);
    max-width: 600px;
    margin: 0 auto;
    opacity: 0.8;
}

.features-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(2, auto);
    gap: 1.5rem;
    grid-template-areas:
        "large large small1 small2"
        "large large small3 small4";
}

.feature-card {
    position: relative;
    background: rgba(255, 255, 255, 0.03);
    border-radius: 16px;
    padding: 2rem;
    border: 1px solid var(--color-border);
    transition: all 0.3s ease;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.feature-card:hover {
    transform: translateY(-5px) scale(1.02);
    border-color: var(--color-border-hover);
    background: rgba(255, 255, 255, 0.05);
}

.large-card {
    grid-area: large;
    flex-direction: row;
    align-items: stretch;
    padding: 0;
}

.large-card .card-content {
    padding: 3rem;
    flex: 1;
}

.large-card .card-visual {
    flex: 1;
    overflow: hidden;
    position: relative;
}

.large-card .card-visual img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.4s ease;
}

.large-card:hover .card-visual img {
    transform: scale(1.05);
}

.feature-card:nth-child(2) {
    grid-area: small1;
}

.feature-card:nth-child(3) {
    grid-area: small2;
}

.feature-card:nth-child(4) {
    grid-area: small3;
}

.feature-card:nth-child(5) {
    grid-area: small4;
}

.card-content h3 {
    font-size: 1.75rem;
    font-weight: 600;
    margin-bottom: 1rem;
    color: #FFFFFF;
}

.large-card .card-content h3 {
    font-size: 2rem;
}

.card-content p {
    font-size: 1rem;
    color: var(--color-text);
    line-height: 1.6;
    opacity: 0.8;
}

.learn-more {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    margin-top: 1.5rem;
    color: var(--color-primary);
    font-weight: 600;
    text-decoration: none;
    transition: all 0.3s ease;
}

.learn-more:hover {
    color: #4DA8FF;
    gap: 0.75rem;
}

.arrow-icon {
    width: 18px;
    height: 18px;
}

.card-icon {
    align-self: flex-end;
    margin-top: 1.5rem;
    color: var(--color-primary);
    opacity: 0.7;
}

.card-icon svg {
    width: 48px;
    height: 48px;
}

@media (max-width: 1200px) {
    .features-grid {
        grid-template-columns: repeat(2, 1fr);
        grid-template-areas:
            "large large"
            "small1 small2"
            "small3 small4";
    }
}

@media (max-width: 768px) {
    .features-grid {
        grid-template-columns: 1fr;
        grid-template-areas:
            "large"
            "small1"
            "small2"
            "small3"
            "small4";
    }

    .large-card {
        flex-direction: column-reverse;
    }

    .large-card .card-visual {
        min-height: 250px;
    }
}
</style>
