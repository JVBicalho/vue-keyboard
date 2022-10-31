<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Key from './components/Key.vue'
</script>

<template>
  <main>
    <div class="keyboard">
    <Key v-for="items in KeySimbolsArray" :keySymbol="items"></Key>
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
      KeyTest: ["Q","W",],
    }
  },
}
      
    

</script>
<style scoped>

* {
  padding: 0;
  margin: 0;
  border: 0;
  box-sizing: border-box
}
#app{
  
}
body{
  background-color:#fff !important;
  
}
main{
  display: flex;
  width: 100vw;
  height: 100vh;
  
}
.keyboard{

  width:90vw;
  flex-direction: row;
  justify-content: center;

}

</style>
