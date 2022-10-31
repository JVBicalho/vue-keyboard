<template >
    
        <span><i>{{ keySymbol }}</i></span>
    
</template>
<script>
export default {
    name : 'Key',
    props : {
      keySymbol : String,
    }
}
</script>
<style >
  span{
    position:relative;
    display:inline-block;
    width: 5.4vw;
    height:5.4vw;
    margin-right: 0.6vw !important;
    border-radius:0.8vw;
    background: linear-gradient(180deg, #282828,#202020);
    box-shadow:inset -0.5vw 0 0.5vw rgba(0,0,0,0.15),
                inset -0px -0.5vw 0.5vw rgba(0,0,0,0.25),
                0 0 0 0.1vw rgba(0,0,0,0.75),
                0.8vw 1.6vw 2vw rgba(0,0,0,0.4);
    overflow:hidden;
    padding:0.2vw 0.2vw;
    margin:0.6vw 0.2vw;
  }
/* Backspace */
span:nth-child(14) {
  width: 10.8vw;
}
/* Tab */
span:nth-child(15) {
  width: 8.1vw;
}
/* \ */
span:nth-child(28) {
  width: 8.1vw;
}
/* Capslock */
span:nth-child(29) {
  width: 11vw;
}
/* Enter */
span:nth-child(41) {
  width: 11.6vw;
}
/* Shift */
span:nth-child(42) {
  width: 13.6vw;
}
/* shift */
span:nth-child(53) {
  width: 15vw;
}
/* CTRL */
span:nth-child(54) {
  width: 7.3vw;
}
/* win */
span:nth-child(55) {
  width: 7.3vw;
}
/* ALT */
span:nth-child(56) {
  width: 7.3vw;
}
/* SPACE */
span:nth-child(57) {
  width: 33.8vw;
  
 
  align-items: center;
}
span:nth-child(57) i{
    display: flex;
    justify-content: center;
   
    align-items: center;
    justify-content: center;
    
    
  }
/* ALT */
span:nth-child(58) {
  width: 7.3vw;
}
/* FN */
span:nth-child(59) {
  width: 7.3vw;
}
/* OPTIONS */
span:nth-child(60) {
  width: 7.3vw;
}
/* CTRL */
span:nth-child(61) {
  width: 7.3vw;
}

  span::before{
    content: '';
    position:absolute;
    top:0.1vw;
    left:0.2vw;
    bottom: 1vw;
    right: 1vw;
    background: linear-gradient(90deg, #232323,#4a4a4a);
    border-radius:0.8vw;
    box-shadow: -0.8vw -0.8vw 0.8vw rgba(255,255,255,0.25),
                0.8vw 0.4vw 0.8vw rgba(0,0,0,0.15);
    
    border-left : 0.1vw solid #0004;
    border-bottom : 0.1vw solid #0004;
    border-top : 0.1vw solid #0004; 
  }
  span i{
    padding-top: 0.1vw;
    padding-left: 0.6vw;
    position: relative;
    color:#fff;
    
    font-size:clamp(0.01em, 2vw ,33.5em);
    font-style:normal;
    text-transform:uppercase;
    
  }
 
</style>