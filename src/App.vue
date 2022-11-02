<script setup>

import Key from './components/Key.vue'

</script>

<template>
  <header>
    <div class="text">{{ text }}</div>
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
                        "CapsLK","a","s","d","f","g","h","j","k","l",";","\'","Enter",
                        "Shift","z","x","c","v","b","n","m","\,","\.","\/","Shift",
                        "Ctrl","win","alt","space","alt","Fn","opitions","Crtl",
                     ],
      text: "TESTE"
    }
  },
  methods: {
    KeyPressed(key) {
      
      console.log(key)
      // Backspace
      if (key == "bksp") {
        this.text = this.text.slice(0, -1)
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
  text-align: center;
  overflow-wrap: break-word;
  font-family: Georgia, serif;
font-size: 25px;
letter-spacing: 1.2px;
word-spacing: 2.4px;
color: #000000;
font-weight: 400;
text-decoration: solid rgb(68, 68, 68);
font-style: normal;
font-variant: small-caps;
text-transform: none;
  
}
.keyboard{

  width:90vw;
  flex-direction: row;
  justify-content: center;

}

</style>
