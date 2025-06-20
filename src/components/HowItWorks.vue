<template>
    <section class="how-it-works">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">AI 工作流程</h2>
                <p class="section-subtitle">从想法到部署，只需三步</p>
            </div>

            <div class="pipeline">
                <div class="pipeline-step">
                    <div class="step-number-wrapper">
                        <div class="step-number">01</div>
                    </div>
                    <div class="step-content">
                        <h3>智能分析</h3>
                        <p>AI 深度理解您的需求，分析主题和风格要求</p>
                        <div class="step-visual">
                            <div class="visual-element analyzing">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="1.5" stroke="currentColor" class="icon">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M7.5 8.25h9m-9 3H12m-2.25 3h5.25" />
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                                </svg>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="pipeline-connector">
                    <div class="connector-arrow"></div>
                </div>

                <div class="pipeline-step">
                    <div class="step-number-wrapper">
                        <div class="step-number">02</div>
                    </div>
                    <div class="step-content">
                        <h3>智能生成</h3>
                        <p>基于分析结果，AI 自动生成代码、设计和内容</p>
                        <div class="step-visual">
                            <div class="visual-element generating">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="1.5" stroke="currentColor" class="icon">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M9.813 15.904L9 18.75l-.813-2.846a4.5 4.5 0 00-3.09-3.09L2.25 12l2.846-.813a4.5 4.5 0 003.09-3.09L9 5.25l.813 2.846a4.5 4.5 0 003.09 3.09L15.75 12l-2.846.813a4.5 4.5 0 00-3.09 3.09zM18.259 8.715L18 9.75l-.259-1.035a3.375 3.375 0 00-2.455-2.456L14.25 6l1.036-.259a3.375 3.375 0 002.455-2.456L18 2.25l.259 1.035a3.375 3.375 0 002.456 2.456L21.75 6l-1.035.259a3.375 3.375 0 00-2.456 2.456zM16.898 20.624l.216.962-.216.962a.75.75 0 001.061 1.06l.962-.215.962.215a.75.75 0 001.06-1.06l-.215-.962.215-.962a.75.75 0 00-1.06-1.06l-.962.215-.962-.215a.75.75 0 00-1.061 1.06z" />
                                </svg>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="pipeline-connector">
                    <div class="connector-arrow"></div>
                </div>

                <div class="pipeline-step">
                    <div class="step-number-wrapper">
                        <div class="step-number">03</div>
                    </div>
                    <div class="step-content">
                        <h3>一键部署</h3>
                        <p>生成的智能体立即部署到云端，立即可用</p>
                        <div class="step-visual">
                            <div class="visual-element deploying">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="1.5" stroke="currentColor" class="icon">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M3 16.5v2.25A2.25 2.25 0 005.25 21h13.5A2.25 2.25 0 0021 18.75V16.5M16.5 12L12 16.5m0 0L7.5 12m4.5 4.5V3" />
                                </svg>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="demo-section">
                <div class="demo-content">
                    <h3>观看演示</h3>
                    <p>了解 AI 如何从简单描述创建完整的智能体</p>
                    <button class="demo-button">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
                            <path d="M8 5v14l11-7z" />
                        </svg>
                        播放演示
                    </button>
                </div>
                <div class="demo-placeholder">
                    <div class="video-placeholder">
                        <div class="play-overlay">
                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
                                <path d="M8 5v14l11-7z" />
                            </svg>
                        </div>
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
.how-it-works {
    padding: var(--section-gap) 0;
    background: #000;
    position: relative;
    overflow: hidden;
}

.how-it-works::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: radial-gradient(circle at 30% 20%, rgba(0, 123, 255, 0.1) 0%, transparent 50%),
        radial-gradient(circle at 70% 80%, rgba(0, 212, 255, 0.1) 0%, transparent 50%);
    pointer-events: none;
}

.section-header {
    text-align: center;
    margin-bottom: 5rem;
}

.section-title {
    font-size: clamp(2.5rem, 6vw, 3rem);
    font-weight: 700;
    color: var(--color-primary);
    margin-bottom: 1rem;
}

.section-subtitle {
    font-size: clamp(1rem, 2.5vw, 1.2rem);
    color: var(--color-text);
    max-width: 600px;
    margin: 0 auto;
    opacity: 0.8;
}

.pipeline {
    display: grid;
    grid-template-columns: 1fr auto 1fr auto 1fr;
    align-items: start;
    gap: 1.5rem;
}

.pipeline-step {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
}

.step-number-wrapper {
    margin-bottom: 1.5rem;
}

.step-number {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background: var(--color-primary);
    color: #FFFFFF;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.25rem;
    font-weight: 700;
    box-shadow: 0 0 20px var(--color-glow);
}

.step-content h3 {
    font-size: 1.5rem;
    font-weight: 600;
    margin-bottom: 1rem;
    color: #FFFFFF;
}

.step-content p {
    color: var(--color-text);
    line-height: 1.6;
    margin-bottom: 2rem;
    opacity: 0.8;
    min-height: 50px;
}

.step-visual {
    width: 120px;
    height: 120px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.visual-element {
    width: 90px;
    height: 90px;
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: rgba(0, 123, 255, 0.1);
    border: 1px solid rgba(0, 123, 255, 0.2);
    color: var(--color-primary);
    transition: all 0.3s ease;
}

.visual-element:hover {
    transform: scale(1.05);
    background: rgba(0, 123, 255, 0.15);
}

.icon {
    width: 40px;
    height: 40px;
}

.visual-element.generating {
    animation: rotate 4s linear infinite;
}

@keyframes rotate {
    from {
        transform: rotate(0deg);
    }

    to {
        transform: rotate(360deg);
    }
}

.pipeline-connector {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 135px;
    /* Aligns with the middle of the text */
}

.connector-arrow {
    position: relative;
    width: 40px;
    height: 1px;
    background-color: var(--color-primary);
    opacity: 0.6;
}

.connector-arrow::after {
    content: '';
    position: absolute;
    right: -1px;
    top: -4px;
    width: 0;
    height: 0;
    border-top: 5px solid transparent;
    border-bottom: 5px solid transparent;
    border-left: 7px solid var(--color-primary);
}

.demo-section {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 4rem;
    align-items: center;
    margin-top: 4rem;
}

.demo-content h3 {
    font-size: 2rem;
    font-weight: 600;
    margin-bottom: 1rem;
    color: #FFFFFF;
}

.demo-content p {
    color: var(--color-text);
    line-height: 1.6;
    margin-bottom: 2rem;
    opacity: 0.8;
}

.demo-button {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    background: linear-gradient(135deg, var(--color-primary), #4DA8FF);
    color: #FFFFFF;
    border: none;
    padding: 1rem 2rem;
    border-radius: 12px;
    font-size: 1rem;
    font-weight: 600;
    cursor: pointer;
    transition: all 0.3s ease;
    box-shadow: 0 0 30px var(--color-glow);
}

.demo-button:hover {
    transform: translateY(-3px);
    box-shadow: 0 0 50px var(--color-glow);
}

.demo-button svg {
    width: 20px;
    height: 20px;
}

.demo-placeholder {
    display: flex;
    justify-content: center;
}

.video-placeholder {
    width: 100%;
    max-width: 500px;
    height: 300px;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0.05));
    border-radius: 16px;
    border: 1px solid rgba(255, 255, 255, 0.2);
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    overflow: hidden;
    backdrop-filter: blur(10px);
}

.video-placeholder::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: linear-gradient(45deg, transparent 30%, rgba(255, 255, 255, 0.1) 50%, transparent 70%);
    animation: shimmer 2s infinite;
}

.play-overlay {
    width: 80px;
    height: 80px;
    background: rgba(0, 123, 255, 0.9);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    transition: all 0.3s ease;
    position: relative;
    z-index: 1;
}

.play-overlay:hover {
    transform: scale(1.1);
    background: var(--color-primary);
}

.play-overlay svg {
    width: 30px;
    height: 30px;
    color: #FFFFFF;
    margin-left: 4px;
}

@keyframes shimmer {
    0% {
        transform: translateX(-100%);
    }

    100% {
        transform: translateX(100%);
    }
}

@media (max-width: 992px) {
    .pipeline {
        grid-template-columns: 1fr;
        gap: 2rem;
    }

    .pipeline-connector {
        transform: rotate(90deg);
        margin: 0;
    }
}
</style>