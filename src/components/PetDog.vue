<template>
  <div class="pet-container">
    <div class="pet-image" @click="touchPet">
      <span :style="{fontSize: size + 'px'}">🐶</span>
    </div>
    <div class="pet-info">
      <p>成长值：{{ growth }}</p>
      <button @click="feedPet">喂食</button>
      <button @click="touchPet">摸摸</button>
      <p v-if="message">{{ message }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PetDog',
  data() {
    return {
      growth: 0,
      size: 48,
      message: ''
    }
  },
  methods: {
    feedPet() {
      this.growth += 1;
      this.size += 2;
      this.message = '谢谢你的美味食物！';
      setTimeout(() => { this.message = ''; }, 1200);
    },
    touchPet() {
      this.message = '好舒服呀，汪汪！';
      setTimeout(() => { this.message = ''; }, 1200);
    }
  }
}
</script>

<style scoped>
.pet-container {
  position: fixed;
  right: 32px;
  bottom: 32px;
  z-index: 9999;
  margin: 0;
  padding: 20px;
  background: #fffbe6;
  border-radius: 16px;
  width: 220px;
  box-shadow: 0 2px 8px #eee;
  transition: box-shadow 0.2s;
}
.pet-container:hover {
  box-shadow: 0 4px 16px #e0c97f;
}
.pet-image {
  cursor: pointer;
  margin-bottom: 10px;
}
.pet-info button {
  margin: 0 8px;
  padding: 4px 12px;
  border: none;
  border-radius: 6px;
  background: #ffe082;
  color: #7c5c00;
  font-weight: bold;
  cursor: pointer;
}
.pet-info button:hover {
  background: #ffd54f;
}
</style>