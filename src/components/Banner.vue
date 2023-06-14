<template>
    <div class="banner">
       <div class="content">
        <h1>HOLA, SOY BRAYAN</h1>
        <h2>Y SOY FRONT END DEVELOPER.</h2>

        <div class="box-btn">
            <a href="" @click.prevent="goToSection('works')" class="button-works">Mis trabajos</a>
        </div>
       </div>
    </div>
</template>

<script>
 /* eslint-disable */

 export default{
    name: 'Baner',
    methods:{
        goToSection(value) {
            const element = document.getElementById(value);
            element.scrollIntoView({ behavior: "smooth", block: "start", inline: "nearest" });
    },
    }
 }
</script>

<style scoped>
h1, h2, .box-btn{
    color: #fff;
    padding: 20px;
}
h1{
    
    font-size: 60px;

}
h2{
    font-size: 30px;  
    font-weight: lighter;
}
.banner{
    width: 100%;
    height: 100vh;
    background: #020912;
    margin: 0;
    padding: 0;
    display: flex;
    align-items: center;
}
.content{
    margin-left: 90px;
}

.button-works{
  border: 2px solid #98E8CD;
  color: #fff;
  padding: 12px 20px;
  font-size: 16px;
  text-decoration: none;
  background: none;
  cursor: pointer;
  border-radius: 30px;
  transition:all .5s;
}

.button-works:hover{
    background: #98E8CD;
    color: #000;
}

@media only screen and (max-width: 600px) {
 .banner{
    display: flex;
    align-items: center;
    justify-content: center;
 }
 .content{
    margin-left: 00px;
}
}
</style>