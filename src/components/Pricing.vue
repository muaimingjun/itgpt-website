<template>
    <section id="pricing" class="pricing">
        <div class="container">
            <h2 class="section-title">灵活的定价方案</h2>
            <p class="section-subtitle">选择适合您团队规模和业务需求的计划。</p>
            <div class="pricing-grid">
                <!-- Pricing Tier 1: Free -->
                <div class="pricing-card">
                    <div class="card-header">
                        <h3>免费版</h3>
                        <p class="price">¥0<span>/月</span></p>
                    </div>
                    <ul class="feature-list">
                        <li><svg class="check-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                                fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                                    clip-rule="evenodd" />
                            </svg>1 个智能体</li>
                        <li><svg class="check-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                                fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                                    clip-rule="evenodd" />
                            </svg>每月 1,000 次调用</li>
                        <li><svg class="check-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                                fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                                    clip-rule="evenodd" />
                            </svg>社区支持</li>
                    </ul>
                    <button class="cta-button secondary">开始使用</button>
                </div>
                <!-- Pricing Tier 2: Pro -->
                <div class="pricing-card popular">
                    <div class="popular-badge">推荐</div>
                    <div class="card-header">
                        <h3>专业版</h3>
                        <p class="price">¥199<span>/月</span></p>
                    </div>
                    <ul class="feature-list">
                        <li><svg class="check-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                                fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                                    clip-rule="evenodd" />
                            </svg>最多 10 个智能体</li>
                        <li><svg class="check-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                                fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                                    clip-rule="evenodd" />
                            </svg>每月 50,000 次调用</li>
                        <li><svg class="check-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                                fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                                    clip-rule="evenodd" />
                            </svg>优先邮件支持</li>
                        <li><svg class="check-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                                fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                                    clip-rule="evenodd" />
                            </svg>API 访问</li>
                    </ul>
                    <button class="cta-button primary">选择专业版</button>
                </div>
                <!-- Pricing Tier 3: Enterprise -->
                <div class="pricing-card">
                    <div class="card-header">
                        <h3>企业版</h3>
                        <p class="price">定制</p>
                    </div>
                    <ul class="feature-list">
                        <li><svg class="check-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                                fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                                    clip-rule="evenodd" />
                            </svg>无限智能体</li>
                        <li><svg class="check-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                                fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                                    clip-rule="evenodd" />
                            </svg>按需调用</li>
                        <li><svg class="check-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                                fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                                    clip-rule="evenodd" />
                            </svg>专属技术支持</li>
                        <li><svg class="check-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                                fill="currentColor">
                                <path fill-rule="evenodd"
                                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                                    clip-rule="evenodd" />
                            </svg>私有化部署</li>
                    </ul>
                    <button class="cta-button secondary">联系我们</button>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
</script>

<style scoped>
.pricing {
    padding: var(--section-gap) 0;
    background: #000;
}

.section-title {
    text-align: center;
    font-size: clamp(2rem, 5vw, 3rem);
    font-weight: 700;
    margin-bottom: 1rem;
}

.section-subtitle {
    text-align: center;
    font-size: clamp(1rem, 2.5vw, 1.2rem);
    color: var(--color-text);
    max-width: 500px;
    margin: 0 auto var(--section-gap) auto;
}

.pricing-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    align-items: stretch;
}

.pricing-card {
    position: relative;
    display: flex;
    flex-direction: column;
    background: rgba(255, 255, 255, 0.05);
    border-radius: 12px;
    padding: 2.5rem;
    border: 1px solid var(--color-border);
    transition: all 0.3s ease;
    overflow: hidden;
}

.pricing-card.popular {
    border-color: var(--color-primary);
    box-shadow: 0 0 30px var(--color-glow);
    transform: scale(1.05);
}

.popular-badge {
    position: absolute;
    top: 1rem;
    right: 1rem;
    background: var(--color-primary);
    color: #fff;
    padding: 0.25rem 0.75rem;
    border-radius: 12px;
    font-size: 0.8rem;
    font-weight: 600;
}

.card-header {
    text-align: center;
    margin-bottom: 2rem;
}

.card-header h3 {
    font-size: 1.75rem;
    font-weight: 600;
    margin-bottom: 0.75rem;
}

.price {
    font-size: 3rem;
    font-weight: 700;
    color: #fff;
}

.price span {
    font-size: 1rem;
    font-weight: 400;
    color: var(--color-text);
}

.feature-list {
    list-style: none;
    padding: 0;
    margin-bottom: 2rem;
    flex-grow: 1;
}

.feature-list li {
    display: flex;
    align-items: center;
    gap: 0.75rem;
    margin-bottom: 1rem;
    color: var(--color-text);
}

.check-icon {
    width: 20px;
    height: 20px;
    color: var(--color-primary);
}

.cta-button {
    width: 100%;
    padding: 1rem;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s ease;
    font-size: 1rem;
    border: 1px solid transparent;
    cursor: pointer;
    text-align: center;
}

.cta-button.primary {
    background: var(--color-primary);
    color: #FFFFFF;
    box-shadow: 0 0 20px var(--color-glow);
}

.cta-button.primary:hover {
    background: #4DA8FF;
    transform: translateY(-3px);
    box-shadow: 0 0 30px var(--color-glow);
}

.cta-button.secondary {
    background: transparent;
    color: #FFFFFF;
    border-color: var(--color-border);
}

.cta-button.secondary:hover {
    background: var(--color-border);
}
</style>