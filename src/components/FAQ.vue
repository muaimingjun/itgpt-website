<template>
    <section id="faq" class="faq">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">常见问题</h2>
                <p class="section-subtitle">关于 ITGPT 的一切，都在这里找到答案</p>
            </div>

            <div class="faq-grid">
                <div class="faq-item" v-for="(item, index) in faqItems" :key="index">
                    <button class="faq-question" @click="toggleFAQ(index)" :class="{ active: activeIndex === index }">
                        <span class="question-text">{{ item.question }}</span>
                        <svg class="arrow-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none"
                            stroke="currentColor" stroke-width="2" :class="{ rotated: activeIndex === index }">
                            <path d="M19 9l-7 7-7-7" />
                        </svg>
                    </button>
                    <div class="faq-answer" :class="{ active: activeIndex === index }">
                        <p>{{ item.answer }}</p>
                    </div>
                </div>
            </div>

            <div class="faq-cta">
                <p>还有问题？加入我们的社区</p>
                <div class="cta-buttons">
                    <a href="#" class="cta-button primary">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
                            <path
                                d="M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0 12.64 12.64 0 0 0-.617-1.25.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057a.082.082 0 0 0 .031.057 19.9 19.9 0 0 0 5.993 3.03.078.078 0 0 0 .084-.028 14.09 14.09 0 0 0 1.226-1.994.076.076 0 0 0-.041-.106 13.107 13.107 0 0 1-1.872-.892.077.077 0 0 1-.008-.128 10.2 10.2 0 0 0 .372-.292.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127 12.299 12.299 0 0 1-1.873.892.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028 19.839 19.839 0 0 0 6.002-3.03.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03zM8.02 15.33c-1.183 0-2.157-1.085-2.157-2.419 0-1.333.956-2.419 2.157-2.419 1.21 0 2.176 1.096 2.157 2.42 0 1.333-.956 2.418-2.157 2.418zm7.975 0c-1.183 0-2.157-1.085-2.157-2.419 0-1.333.955-2.419 2.157-2.419 1.21 0 2.176 1.096 2.157 2.42 0 1.333-.946 2.418-2.157 2.418z" />
                        </svg>
                        加入 Discord
                    </a>
                    <a href="#" class="cta-button secondary">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
                            <path
                                d="M1.5 8.67v8.58a3 3 0 003 3h15a3 3 0 003-3V8.67l-8.928 5.493a3 3 0 01-3.144 0L1.5 8.67z" />
                            <path
                                d="M22.5 6.908V6.75a3 3 0 00-3-3h-15a3 3 0 00-3 3v.158l9.714 5.978a1.5 1.5 0 001.572 0L22.5 6.908z" />
                        </svg>
                        联系我们
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue'

const activeIndex = ref(null)

const faqItems = [
    {
        question: "ITGPT 是什么？",
        answer: "ITGPT 是一个基于 AI 的智能体开发平台，让您无需编码即可创建、部署和管理 AI 智能体。我们提供可视化的开发工具和强大的 AI 模型支持。"
    },
    {
        question: "我需要编程经验吗？",
        answer: "完全不需要！ITGPT 采用无代码设计，通过简单的拖拽和配置即可创建智能体。我们的 AI 助手会帮助您完成所有技术细节。"
    },
    {
        question: "支持哪些 AI 模型？",
        answer: "我们支持主流的大语言模型，包括 GPT-4、Claude、Gemini 等，同时也支持私有化部署的模型。您可以根据需求选择合适的模型。"
    },
    {
        question: "如何保证数据安全？",
        answer: "我们采用企业级的安全措施，包括数据加密、访问控制、审计日志等。所有数据都存储在安全的云端环境中，确保您的隐私和数据安全。"
    },
    {
        question: "可以自定义智能体的外观吗？",
        answer: "当然可以！我们提供丰富的主题和样式选项，您可以自定义智能体的界面、颜色、字体等，打造独特的品牌体验。"
    },
    {
        question: "支持哪些部署方式？",
        answer: "我们支持多种部署方式，包括云端部署、私有化部署、API 集成等。您可以根据业务需求选择最适合的部署方案。"
    }
]

const toggleFAQ = (index) => {
    activeIndex.value = activeIndex.value === index ? null : index
}
</script>

<style scoped>
.faq {
    padding: var(--section-gap) 0;
    background: linear-gradient(180deg, #0a0a0a 0%, #000000 100%);
    position: relative;
}

.faq::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: radial-gradient(circle at 20% 80%, rgba(0, 123, 255, 0.05) 0%, transparent 50%);
    pointer-events: none;
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
    font-size: clamp(1.1rem, 2.5vw, 1.3rem);
    color: var(--color-text);
    max-width: 600px;
    margin: 0 auto;
    opacity: 0.8;
}

.faq-grid {
    max-width: 800px;
    margin: 0 auto 4rem auto;
}

.faq-item {
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 12px;
    margin-bottom: 1rem;
    overflow: hidden;
    background: rgba(255, 255, 255, 0.02);
    backdrop-filter: blur(10px);
    transition: all 0.3s ease;
}

.faq-item:hover {
    border-color: rgba(255, 255, 255, 0.2);
    background: rgba(255, 255, 255, 0.05);
}

.faq-question {
    width: 100%;
    padding: 1.5rem 2rem;
    background: none;
    border: none;
    color: #FFFFFF;
    font-size: 1.1rem;
    font-weight: 600;
    text-align: left;
    cursor: pointer;
    display: flex;
    justify-content: space-between;
    align-items: center;
    transition: all 0.3s ease;
}

.faq-question:hover {
    background: rgba(255, 255, 255, 0.05);
}

.faq-question.active {
    background: rgba(0, 123, 255, 0.1);
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.question-text {
    flex: 1;
    margin-right: 1rem;
}

.arrow-icon {
    width: 20px;
    height: 20px;
    color: var(--color-primary);
    transition: transform 0.3s ease;
    flex-shrink: 0;
}

.arrow-icon.rotated {
    transform: rotate(180deg);
}

.faq-answer {
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.3s ease, padding 0.3s ease;
    padding: 0 2rem;
}

.faq-answer.active {
    max-height: 200px;
    padding: 1.5rem 2rem;
}

.faq-answer p {
    color: var(--color-text);
    line-height: 1.6;
    opacity: 0.9;
    margin: 0;
}

.faq-cta {
    text-align: center;
    padding: 3rem;
    background: rgba(255, 255, 255, 0.02);
    border-radius: 16px;
    border: 1px solid rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(10px);
}

.faq-cta p {
    font-size: 1.2rem;
    color: #FFFFFF;
    margin-bottom: 2rem;
    font-weight: 500;
}

.cta-buttons {
    display: flex;
    gap: 1rem;
    justify-content: center;
    flex-wrap: wrap;
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

.cta-button svg {
    width: 20px;
    height: 20px;
}

@media (max-width: 768px) {
    .faq-question {
        padding: 1rem 1.5rem;
        font-size: 1rem;
    }

    .faq-answer.active {
        padding: 1rem 1.5rem;
    }

    .cta-buttons {
        flex-direction: column;
        align-items: center;
    }

    .cta-button {
        width: 100%;
        max-width: 300px;
        justify-content: center;
    }
}
</style>