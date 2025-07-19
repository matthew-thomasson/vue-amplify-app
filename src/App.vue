<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<template>
  <div class="app">
    <header class="header">
      <h1>My Vue SPA</h1>
      <p>Ready for AWS Amplify deployment</p>
    </header>
    
    <main class="main">
      <div class="counter">
        <button @click="count--">-</button>
        <span>{{ count }}</span>
        <button @click="count++">+</button>
      </div>
      
      <div class="info">
        <h2>Welcome!</h2>
        <p>This is a simple Vue 3 Single Page Application built with Vite.</p>
        <p>It's ready to be deployed to AWS Amplify.</p>
      </div>
    </main>
  </div>
</template>

<style scoped>
.app {
  max-width: 800px;
  margin: 0 auto;
  padding: 2rem;
  text-align: center;
}

.header {
  margin-bottom: 2rem;
}

.header h1 {
  color: #42b883;
  font-size: 3rem;
  margin-bottom: 0.5rem;
}

.header p {
  color: #666;
  font-size: 1.2rem;
}

.main {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.counter {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
  font-size: 2rem;
}

.counter button {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  border: 2px solid #42b883;
  background: white;
  color: #42b883;
  font-size: 1.5rem;
  cursor: pointer;
  transition: all 0.2s;
}

.counter button:hover {
  background: #42b883;
  color: white;
}

.counter span {
  min-width: 60px;
  font-weight: bold;
}

.info {
  background: #f8f9fa;
  padding: 2rem;
  border-radius: 10px;
  border: 1px solid #e9ecef;
}

.info h2 {
  color: #333;
  margin-bottom: 1rem;
}

.info p {
  color: #666;
  line-height: 1.6;
  margin-bottom: 1rem;
}
</style>
