<template lang="">
    <div>Bai 2
        <h2 :class="{ red: isRed }">Red</h2>
        <h2 :class="{blue: isBlue}"> Blue</h2>
        <h2 :class="{green: isGreen}">Green</h2>
    </div>
    
</template>
<script>
export default{
    data(){
        return{
            isRed:true,
            isBlue:true,
            isGreen:true,
            
        }
    }
}
</script>
<style scoped lang="scss">
   .red{
    background-color: red;
    height: 200px;
    width: 200px;
   }
   .blue{
    background-color: blue;
    height: 200px;
    width: 200px;
   }
   .green{
    background-color: green;
    height: 200px;
    width: 200px;
   }
</style>