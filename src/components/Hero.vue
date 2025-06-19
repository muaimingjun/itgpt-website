<template>
  <section class="hero">
    <div class="background-animation">
      <div class="star"></div>
      <!-- Add more stars or other animated elements here -->
    </div>
    <div class="container hero-content">
      <h1 class="hero-title">AI智能体一站式开发平台</h1>
      <p class="hero-subtitle">
        从灵感到现实，一键构建、部署并扩展你的专属AI智能体。
      </p>
      <div class="hero-actions">
        <a href="#" class="cta-button primary">立即开始</a>
        <a href="#features" class="cta-button secondary">探索特性</a>
      </div>
    </div>
  </section>
</template>

<script setup>
// No script logic needed for this component
</script>

<style scoped>
.hero {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh; /* Full viewport height */
  padding-top: 80px; /* Offset for the fixed header */
  text-align: center;
  overflow: hidden;
  background: radial-gradient(ellipse at 50% 50%, #1a0c33 0%, #000000 70%);
}

.background-animation {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 0;
}

/* Example of a simple star animation */
.star {
  position: absolute;
  width: 2px;
  height: 2px;
  background: white;
  border-radius: 50%;
  box-shadow: 0 0 5px white, 0 0 10px white, 0 0 15px white;
  animation: twinkle 5s infinite;
}

/* You would need to generate multiple stars with different positions and delays */
.star:nth-child(1) { top: 20%; left: 25%; animation-delay: 0s; }
.star:nth-child(2) { top: 80%; left: 50%; animation-delay: 1s; }
/* ... and so on ... */


.hero-content {
  position: relative;
  z-index: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.hero-title {
  font-size: clamp(2.5rem, 6vw, 4.5rem);
  font-weight: 700;
  color: #FFFFFF;
  margin-bottom: 1.5rem;
  line-height: 1.2;
  text-shadow: 0 0 20px rgba(255, 255, 255, 0.3);
}

.hero-subtitle {
  font-size: clamp(1rem, 2.5vw, 1.25rem);
  color: var(--color-text);
  max-width: 650px;
  margin-bottom: 2.5rem;
  line-height: 1.6;
}

.hero-actions {
  display: flex;
  gap: 1rem;
}

.cta-button {
  padding: 0.8rem 2rem;
  border-radius: 8px;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s ease;
  font-size: 1rem;
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
  border: 1px solid var(--color-border);
}

.cta-button.secondary:hover {
  background: var(--color-border);
  transform: translateY(-3px);
}

@keyframes twinkle {
  0% { opacity: 0; }
  50% { opacity: 1; }
  100% { opacity: 0; }
}
</style>
