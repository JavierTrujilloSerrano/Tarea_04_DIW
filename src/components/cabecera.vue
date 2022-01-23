<template>
    <section>
        <div class="cabecera background">
                <div class="colum">
                <img class="icono" src="../assets/dibujo3.svg" alt="Logo empresa" />
                <h1 class="texto_iz">Tu tienda informatica</h1>
                </div>
        
        <form class="linea">
            <input class ="caja" type ="text" placeholder="Buscar artículos ..."/>
            <button class="boton texto"> Buscar </button>
        </form>
        <div class="margen">
           
            <a class="" href="#">Bienvenido<br> Entrar / Registro </a> 
            <a class="margen" href="#"> <img class="cesta" src="../assets/cesta2.png"/>Mi cesta </a>
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style>

.background{
    
    background: rgb(223, 167, 103);
    flex-wrap: nowrap;
}
.cabecera{
    display:flex;
    flex-direction: row;
    justify-content: space-around;
    height: 110px;
    width: auto;
    padding: 15px;
    box-sizing: content-box;
}
.linea{
    display: flex;
    flex-direction: row;
    margin-top: 2rem;
}
.colum{
    display:flex;
    flex-direction: column;
    margin-top: 1rem;
}

.texto{
    font-size: 1.5rem;
    text-align: center;
    padding-left: 1rem;
}
.texto_iz{
    text-align: left;
    margin: 1rem;
    margin-top: 0rem;
    color: rgb(0, 0, 0);
}
.margen{
    display: flex;
    flex-direction: row;
    align-items: center;
    margin-left: 2rem;
     
}
.caja{
    display: flex;
    height: 33px;
    width: 300px;
    margin: 0rem;
    border:solid;
    border-radius: 20rem;
    text-align: center;
    border-color:rgb(154, 90, 226);
    flex-grow: 1;
    
}
.boton{
    display: flex;
    box-sizing: content-box;
    background-color: rgb(154, 90, 226);
    border-radius: 20rem;
    height: 33px;
    width: 90px;
    margin: 0rem;
    
    
}
.icono{
    display: flex;
    height: 3rem;
    margin-left: 3rem;
}
.cesta{
    display: flex;
    height: 4rem;
    width: 4rem;
    margin-top: 0rem;
    
}
a{
    text-decoration: none;
    color: black;
}

</style>