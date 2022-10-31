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
    height:8vw;
    margin-right: 0.6vw !important;
    border-radius:10px;
    background: linear-gradient(180deg, #282828,#202020);
    box-shadow:inset -8px 0 8px rgba(0,0,0,0.15),
                inset -0px -8px 8px rgba(0,0,0,0.25),
                0 0 0 2px rgba(0,0,0,0.75),
                10px 20px 25px rgba(0,0,0,0.4);
    overflow:hidden;
    padding:8px 15px;
    margin:8px 4px;
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
span:nth-child(53) {
  width: 15vw;
}
span:nth-child(54) {
  width: 7.3vw;
}
span:nth-child(55) {
  width: 7.3vw;
}
span:nth-child(56) {
  width: 7.3vw;
}
span:nth-child(57) {
  width: 33.8vw;
}
span:nth-child(58) {
  width: 7.3vw;
}
span:nth-child(59) {
  width: 7.3vw;
}
span:nth-child(60) {
  width: 7.3vw;
}
span:nth-child(61) {
  width: 7.3vw;
}

  span::before{
    content: '';
    position:absolute;
    top:4%;
    left:5%;
    bottom: 14px;
    right: 12px;
    background: linear-gradient(90deg, #232323,#4a4a4a);
    border-radius:10px;
    box-shadow: -10px -10px 10px rgba(255,255,255,0.25),
                10px 5px 10px rgba(0,0,0,0.15);
    
    border-left : 1px solid #0004;
    border-bottom : 1px solid #0004;
    border-top : 1px solid #0004; 
  }
  span i{
    padding-top: 30%;
    padding-left: 10%;
    position: relative;
    color:#fff;
    
    font-size:clamp(0.01em, 2vw ,33.5em);
    font-style:normal;
    text-transform:uppercase;
    
  }
</style>