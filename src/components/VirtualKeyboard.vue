<template>
  <div class="keyboard-container">
    <input 
      type="text" 
      v-model="inputText" 
      @focus="showKeyboard = true" 
      placeholder="Кликните сюда для клавиатуры"
    />
    
    <div class="keyboard" v-if="showKeyboard">
      <div class="keyboard-row">
        <button v-for="key in firstRow" :key="key" @click="addChar(key)">{{ key }}</button>
      </div>
      <div class="keyboard-row">
        <button v-for="key in secondRow" :key="key" @click="addChar(key)">{{ key }}</button>
      </div>
      <div class="keyboard-row">
        <button v-for="key in thirdRow" :key="key" @click="addChar(key)">{{ key }}</button>
      </div>
      <div class="keyboard-row">
        <button @click="addChar(' ')">Space</button>
        <button @click="inputText = ''">Clear</button>
        <button @click="showKeyboard = false">Hide</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      inputText: '',
      showKeyboard: false,
      firstRow: ['a', 'w', 'e', 'r', 't', 'y', 'u', 'i', 'o', 'p'],
      secondRow: ['a', 's', 'd', 'f', 'g', 'h', 'j', 'k', 'l'],
      thirdRow: ['A', 'z', 'x', 'c', 'v', 'b', 'n', 'm'],
    };
  },
  methods: {
    addChar(char) {
      this.inputText += char;
    },
  },
};
</script>
<style scoped>
.keyboard-container {
  max-width: 600px;
  margin: 20px auto;
}
input {
  width: 100%;
  padding: 10px;
  font-size: 16px;
  margin-bottom: 10px;
}
.keyboard {
  background: #f0f0f0;
  padding: 10px;
  border-radius: 5px;
}
.keyboard-row {
  display: flex;
  justify-content: center;
  margin-bottom: 5px;
}
button {
  padding: 10px 15px;
  margin: 2px;
  font-size: 16px;
  cursor: pointer;
  border: 1px solid #ccc;
  border-radius: 3px;
  background: white;
}
button:hover {
  background: #e0e0e0;
}
</style>