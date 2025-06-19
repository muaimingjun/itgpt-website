<template>
  <section class="features" id="features">
    <div class="container">
      <h2 class="section-title">核心特性</h2>
      <p class="section-subtitle">构建下一代 AI 应用所需的一切。</p>
      <div class="features-grid">
        <!-- Feature 1 -->
        <div class="feature-card">
          <div class="card-glow"></div>
          <div class="card-content">
            <div class="feature-icon">
              <!-- Replace with a more modern icon, e.g., from an icon library -->
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" d="M14.25 6.087c0-.66.537-1.197 1.197-1.197h.006c.66 0 1.197.537 1.197 1.197v7.513c0 .66-.537 1.197-1.197 1.197h-.006c-.66 0-1.197-.537-1.197-1.197V6.087zM6.75 6.087c0-.66.537-1.197 1.197-1.197h.006c.66 0 1.197.537 1.197 1.197v11.826c0 .66-.537 1.197-1.197 1.197H7.947c-.66 0-1.197-.537-1.197-1.197V6.087zM10.5 6.087c0-.66.537-1.197 1.197-1.197h.006c.66 0 1.197.537 1.197 1.197v3.756c0 .66-.537 1.197-1.197 1.197h-.006c-.66 0-1.197-.537-1.197-1.197V6.087z"/></svg>
            </div>
            <h3>多模型支持</h3>
            <p>无缝集成主流大语言模型，或接入您的私有模型。</p>
          </div>
        </div>
        <!-- Feature 2 -->
        <div class="feature-card">
          <div class="card-glow"></div>
          <div class="card-content">
            <div class="feature-icon">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" d="M3.75 13.5l10.5-11.25L12 10.5h8.25L9.75 21.75 12 13.5H3.75z" /></svg>
            </div>
            <h3>可视化编排</h3>
            <p>通过拖拽式界面构建复杂的 AI 工作流，无需编码。</p>
          </div>
        </div>
        <!-- Feature 3 -->
        <div class="feature-card">
          <div class="card-glow"></div>
          <div class="card-content">
            <div class="feature-icon">
             <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" d="M9 17.25v1.5m3.75-13.5l-3.75 3.75m3.75-3.75L16.5 7.5M12 21v-1.5m3.75-13.5l-3.75 3.75M12 3v1.5m-3.75 13.5l3.75-3.75m-3.75 3.75L7.5 16.5m9-9l-3.75 3.75M3 12h1.5m16.5 0h-1.5m-12 5.25v-1.5m3.75 0l-3.75-3.75m3.75 3.75l3.75-3.75M12 6v1.5m-3.75 5.25l3.75-3.75m-3.75 3.75L7.5 9m9 9l3.75-3.75" /></svg>
            </div>
            <h3>一键部署</h3>
            <p>将您的智能体快速发布到多个平台和渠道。</p>
          </div>
        </div>
        <!-- Feature 4 -->
        <div class="feature-card">
          <div class="card-glow"></div>
          <div class="card-content">
            <div class="feature-icon">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12.75L11.25 15 15 9.75m-3-7.036A11.959 11.959 0 013.598 6 11.99 11.99 0 003 9.749c0 5.592 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.31-.21-2.571-.598-3.751h-.152c-3.196 0-6.1-1.248-8.25-3.286z" /></svg>
            </div>
            <h3>企业级安全</h3>
            <p>提供数据隔离、加密和访问控制，确保您的数据安全。</p>
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

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

.feature-card {
  position: relative;
  background: rgba(255, 255, 255, 0.05);
  border-radius: 12px;
  padding: 2rem;
  border: 1px solid var(--color-border);
  transition: all 0.3s ease;
  overflow: hidden;
}

.feature-card:hover {
  transform: translateY(-5px);
  border-color: var(--color-border-hover);
}

.feature-card:hover .card-glow {
  opacity: 1;
}

.card-glow {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: radial-gradient(ellipse at 50% -20%, var(--color-glow) 0%, transparent 80%);
  opacity: 0;
  transition: opacity 0.4s ease;
  z-index: 0;
}

.card-content {
  position: relative;
  z-index: 1;
}

.feature-icon {
  width: 48px;
  height: 48px;
  margin-bottom: 1.5rem;
  color: var(--color-primary);
}

.feature-card h3 {
  font-size: 1.5rem;
  font-weight: 600;
  margin-bottom: 0.75rem;
  color: #FFFFFF;
}

.feature-card p {
  font-size: 1rem;
  color: var(--color-text);
  line-height: 1.6;
}
</style>
