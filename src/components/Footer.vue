<template>
  <footer class="footer">
    <div class="container footer-content">
      <div class="footer-links">
        <a href="#">关于我们</a>
        <a href="#">加入我们</a>
        <a href="#">联系方式</a>
        <a href="#">隐私政策</a>
      </div>
      <div class="social-links">
        <!-- Replace with actual social media icons -->
        <a href="#"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M..."></path></svg></a>
        <a href="#"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M..."></path></svg></a>
        <a href="#"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M..."></path></svg></a>
      </div>
      <p class="copyright">© {{ new Date().getFullYear() }} ITGPT Inc. 保留所有权利。</p>
    </div>
  </footer>
</template>

<script setup>
// No script logic needed
</script>

<style scoped>
.footer {
  padding: 4rem 0;
  background-color: #050505;
  border-top: 1px solid var(--color-border);
}

.footer-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
}

.footer-links {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 1.5rem;
}

.footer-links a {
  color: var(--color-text);
  text-decoration: none;
  transition: color 0.3s ease;
}

.footer-links a:hover {
  color: var(--color-primary);
}

.social-links {
  display: flex;
  gap: 1.5rem;
}

.social-links a {
  color: var(--color-text);
  transition: color 0.3s ease;
}

.social-links a:hover {
  color: var(--color-primary);
}

.social-links svg {
  width: 24px;
  height: 24px;
}

.copyright {
  color: #888;
  font-size: 0.9rem;
}
</style>
