<template>
<section class="colum texto_iz bajar"> 
    <div>
        <h2><span class="textoMas">478,99€</span><span class="textoMenos">sin IVA: 395,85€</span></h2>
            <div id="comprarUnidades" class="linea">
                <button class="contarMenos" @click="cambiarContador('-1')" type="button" name="button">-</button>
                <input class="contardor" type="text" name="name" :value="contador">
                <button class="contarMas" @click="cambiarContador('1')" type="button" name="button">+</button>

            </div>
                <button class="anadir"><span class=""></span> AÑADIR A LA CESTA</button>
            
    </div>

    <div>
      <h2>CARACTERISTICAS DEL PRODUCTO</h2>
        <ul>
            <li>HDR10+: El sistema de HDR más completo, avanzado y con soporte dinámico. El mejor complemento para los TVs con el máximo nivel de nits.</li>
            <li>Función One Remote: Controla todos tus dispositivos conectados con tu mando y accede fácilmente a tus contenidos.</li>
            <li>Compatible con Asistentes de Voz: Interactúa con tu televisor a través de Bixby, Hey Google o Alexa.</li>
            <li>Smart TV Powered by TIZEN™: Disfruta de los mejores contenidos de vídeo, música y deporte, a través de una plataforma fácil e intuitiva con las mejores apps.</li>
        </ul>
    </div>
    <div>
        <iframe class="margen" src="https://www.youtube.com/watch?v=0ujKZpELZRc" frameborder="0"></iframe>
    </div>
</section>
</template>

<script>
export default {

      Name: 'ProductoDatos',
    data () {
        return {
            contador: 1
        }
    },
    methods: {
        cambiarContador(num) {
            this.contador += +num;
            if (!isNaN(this.contador) && (this.contador < 0)) {
              this.contador = 0
            }
        }
    }

}
</script>

<style>
.bajar{
    display: flex;
    padding-top: 10rem;
}
.anadir{
    font-size: 1.5rem;
    border-radius: 1rem;
    background-color: rgb(154, 90, 226);
   
}
.contarMenos{
    display: flex;
    align-items:center;
    margin-bottom: 1rem;
    margin-top: 0.8rem;
    margin-right: 0.5rem;
    border-radius: 0.8rem;
    padding-left: 0.9rem;
    height: 3rem;
    width: 3rem;
    font-size: 3rem;
    color:rgb(0, 0, 0);
    background-color: rgb(154, 90, 226);
    border-color: gray;
}
.contarMas{
    display: flex;
    align-items:center;
    margin-bottom: 1rem;
    margin-top: 0.8rem;
    margin-right: 0.5rem;
    border-radius: 0.8rem;
    padding-left: 0.5rem;
    height: 3rem;
    width: 3rem;
    font-size: 3rem;
    color:rgb(0, 0, 0);
    background-color: rgb(154, 90, 226);
    border-color: gray;

}
.contardor{
    display: flex;
    margin-top: 0.7rem;
    margin-right: 0.4rem;
    height: 2.8rem;
    width: 2rem;
    font-size: 2rem;
    color:rgb(0, 0, 0);
    background-color: rgb(233, 233, 233);
    padding-left: 1rem;
}
.textoMenos{
    font-size: small;
    font-weight: normal;

}
.textoMas{
    color: rgb(154, 90, 226);
}

</style>