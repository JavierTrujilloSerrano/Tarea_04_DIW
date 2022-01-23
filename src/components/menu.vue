<template>
    <section>
        <div class="fondo">
            <lu class="fondo">
                <li><a href="#">INICIO</a></li>
                <li><a href="#">ORDENADORES</a></li>
                <li><a href="#">TELEVISIONES</a></li>
                <li><a href="#">MÓVILES</a></li>
                <li><a href="#">TABLETS</a></li>
                <li><a href="#">MULTIMEDIA</a></li>
            </lu>
        </div>
        <div id="corte">
            <a href="#"> Inicio </a> >
            <a href="#"> Televisiones </a> > 
            <a href="#"> Smart TV</a> 
        </div>
    </section>
</template>

<script>
export default {
     Name: 'cambiarFoto',
     data () {
        return {
            fotos: [
                require ('../assets/01.jpg'),
                require ('../assets/02-1.jpg'),
                require ('../assets/03-1.jpg'),
                require ('../assets/04-1.jpg'),
                require ('../assets/05-1.jpg')]
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
.fondo{
    display: flex;
    width: auto;
    justify-content: space-between;
    font-size: 1.2rem;
    height: 3rem;
    padding-bottom: 0.6rem;
    flex-direction: row;
    background-color: rgb(154, 90, 226);
    
}
#corte{
    text-align: start;
    font-size: 1.4rem;
    padding:0.5rem;
    background: rgb(223, 167, 103);
}
li{

    text-decoration: none;
    list-style: none;
    padding:1rem;
}
a:hover{
    border: solid;
    border-radius: 0.5rem;
    color: rgb(154, 90, 226);
    border-color: rgb(154, 90, 226);
    background: rgb(223, 167, 103);
    padding: 1.1rem;
}
</style>