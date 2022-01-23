<template>
<section id="paralelo centrar">
    <div class="colum principal">
        <h1>Samsung UE55TU7045 55" Crystal UltraHD 4K HDR10+</h1>
        <img v-bind:src="fotos[0]" alt="imagen Tv frontal"/>
    </div>
    <div class="linea fotos">

            <a @click="cambiarFoto(1)"><img class="mini" v-bind:src="fotos[1]" alt="foto televisor Samsung"/></a>
            <a @click="cambiarFoto(2)"><img class="mini" v-bind:src="fotos[2]" alt="foto televisor Samsung"/></a>
            <a @click="cambiarFoto(3)"><img class="mini" v-bind:src="fotos[3]" alt="foto televisor Samsung"/></a>
            <a @click="cambiarFoto(4)"><img class="mini" v-bind:src="fotos[4]" alt="foto televisor Samsung"/></a>
            <a @click="cambiarFoto(5)"><img class="mini" v-bind:src="fotos[5]" alt="foto televisor Samsung"/></a>
        
    </div>
</section>        
</template>

<script>

export default {
    Name: 'imagen',
    data () {
        return {
            fotos: [
                require ('../assets/01opt.jpg'),
                require ('../assets/01opt.jpg'),
                require ('../assets/02_opt.jpg'),
                require ('../assets/03_opt.jpg'),
                require ('../assets/04_opt.jpg'),
                require ('../assets/05_opt.jpg')
                ]
        }
    },
    methods: {
        cambiarFoto(id) {
            this.fotos[0] = this.fotos[id]
        }
    }
}


</script>


<style scoped>
#paralelo{
    
    flex: 1 2 18rem;
    margin-bottom: -7rem;
}
.mini {
    display: flex;
    border: solid 1px;
    width: 80px;
    margin-top: 4rem;

}
#centrar{
    display:flex;
    align-items: center;
    
  
}
.fotos{
    
    align-items: center;
    margin: 2rem;
    justify-content: space-around;
    
}
.principal{
    align-items: center;
    height: 500px;
    width: 500px;
}

</style>