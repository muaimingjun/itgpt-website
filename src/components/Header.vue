<template>
  <header class="header">
    <div class="container">
      <a href="#" class="logo">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M12 2L2 7V17L12 22L22 17V7L12 2Z" stroke="white" stroke-width="2" stroke-linejoin="round"/>
          <path d="M2 7L12 12L22 7" stroke="white" stroke-width="2" stroke-linejoin="round"/>
          <path d="M12 12V22" stroke="white" stroke-width="2" stroke-linejoin="round"/>
        </svg>
        <span>ITGPT</span>
      </a>
      <nav class="nav">
        <a href="#features">Features</a>
        <a href="#pricing">Pricing</a>
        <a href="#faq">FAQ</a>
      </nav>
      <a href="#" class="cta-button">Get Started</a>
    </div>
  </header>
</template>

<script setup>
// No script logic needed for this simple component
</script>

<style scoped>
.header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000;
  padding: 1rem 0;
  background: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border-bottom: 1px solid var(--color-border);
  transition: background 0.3s ease;
}

.container {
  max-width: 1280px;
  margin: 0 auto;
  padding: 0 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  color: #FFFFFF;
  font-family: var(--font-heading);
  font-weight: 600;
  font-size: 1.25rem;
  text-decoration: none;
}

.logo svg {
  transition: transform 0.3s ease;
}

.logo:hover svg {
  transform: rotate(15deg);
}

.nav {
  display: flex;
  gap: 2rem;
}

.nav a {
  color: var(--color-text);
  font-size: 1rem;
  font-weight: 500;
  text-decoration: none;
  position: relative;
  transition: color 0.3s ease;
}

.nav a::after {
  content: '';
  position: absolute;
  width: 0;
  height: 2px;
  bottom: -4px;
  left: 50%;
  transform: translateX(-50%);
  background-color: var(--color-primary);
  transition: width 0.3s ease;
}

.nav a:hover {
  color: #FFFFFF;
}

.nav a:hover::after {
  width: 100%;
}

.cta-button {
  background: var(--color-primary);
  color: #FFFFFF;
  padding: 0.6rem 1.2rem;
  border-radius: 6px;
  text-decoration: none;
  font-weight: 500;
  transition: all 0.3s ease;
  box-shadow: 0 0 15px var(--color-glow);
}

.cta-button:hover {
  background: #4DA8FF;
  transform: translateY(-2px);
  box-shadow: 0 0 25px var(--color-glow);
}
</style>
