<script setup>

import Key from './components/Key.vue'

</script>

<template>
  <header>
    <div class="text"><span>{{ text }}</span></div>
  </header>
  <main>
    
  
      <div class="keyboard">
        <Key v-for="items in KeySimbolsArray" :keySymbol="items" v-on:click="KeyPressed(items)"></Key>
      </div>

  </main>
 
    
   
  
</template>
<script>
  export default {
  data() {
    return {
      KeySimbolsArray: ["Esc","1","2","3","4","5","6","7","8","9","0","-","=","bksp",
                        "Tab","q","w","e","r","t","y","u","i","o","p","[","]","\\",
                        "CapsLk","a","s","d","f","g","h","j","k","l",";","\'","Enter",
                        "Shift","z","x","c","v","b","n","m","\,","\.","\/","Shift",
                        "Ctrl","Win","alt","space","alt","Fn","opitions","Crtl",
                     ],
      text: "JV Bicalho"
    }
  },
  methods: {
    KeyPressed(key) {
      
      console.log(key)
      // Esc
      if (key == "Esc") {
        
        return
      }
      // Backspace
      if (key == "bksp") {
        this.text = this.text.slice(0, -1)
        return
      }
      // Tab
      if (key == "Tab") {
        this.text+= '     '
        return
      }
      // CapsLk
      if (key == "CapsLk") {
        
        return
      }
      // Enter
      if (key == "Enter") {
        
        return
      }
      // Shift
      if (key == "Shift") {
        
        return
      }
      // Ctrl
      if (key == "Ctrl") {
        
        return
      }
      // Win
      if (key == "Win") {
        
        return
      }
      // Alt
      if (key == "Alt") {
        
        return
      }
      // Fn
      if (key == "Fn") {
        
        return
      }
      // Options
      if (key == "Options") {
        
        return
      }
      // Space
      if (key == "space") {
        this.text+= ' '
        return
      }
      this.text += key
    }
  }
}
      
    

</script>
<style scoped>

header{
  display: flex;
  justify-content: center;
  align-items: center;
}
main{
  border-radius: 0.5vw;
  padding-top: 2vw;
  padding: 2vw;
  align-items: center; 
  
  -webkit-box-shadow: inset 0px 0px 20px 14px rgba(237,237,237,1);
-moz-box-shadow: inset 0px 0px 20px 14px rgba(237,237,237,1);
box-shadow: inset 0px 0px 20px 14px rgba(237,237,237,1);
}
.text{
  display: flex;
  justify-content: center;
  align-items: center; 
  height: 15vw;
  /* text-align: center; */
  max-width:80vw;
}
.text span{
   
  overflow-wrap: break-word;
  font-family: Georgia, serif;
  font-size: 25px;
  letter-spacing: 1.2px;
  word-spacing: 2.4px;
  color: #000000;
  font-weight: 400;
  text-decoration: solid rgb(68, 68, 68);
  font-style: normal;
  text-transform: none;
  user-select: none; 
    
}
.text span:after{
   content: '';
    display: inline-block;
    background-color: black;
    margin-left: 2px;
    height: 25px;
    width: 0.1vw;
    animation: cursor 0.4s infinite;
}

  
@keyframes cursor {
  0% { opacity: 1; }
  49% { opacity: 1; }
  50% { opacity: 0; }
  100% { opacity: 0; }
 }
.keyboard{

  width:90vw;
  flex-direction: row;
  justify-content: center;

}

</style>
