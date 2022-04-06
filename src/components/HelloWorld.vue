<template>
<body>
    <!-- VISTA 1 -->
<section> 
    <div class="container">
    
    <div class="col1">
      <div>
        <img src="/home/slimshady/shiftsystem/src/assets/Calendario.png" alt="calendar">
      </div>
    </div>

    <div class="col2">
      <div>
        <form action="index2.html">
          <div class="select-control">
            <label>¿En dónde querés sacar turno?</label>
            <select  id="lugar" name="lugar">
                <option  value="value1"></option>
                <option  value="Peluquería">Peluquería</option>
                <option  value="Gimnasio">Gimnasio</option>
                <option  value="Centro de Estética">Centro de Estética</option>
            </select>
          </div>
          
          <div class="select-control">
            <label>¿Con quién?</label>
            <select  id="profesional" name="profesional">
                <option  value="value1"></option>
                <option  value="José Luis Espert">José Luis Espert</option>
                <option  value="Javier Milei">Javier Milei</option>
                <option  value="Patricia Bullrrich">Patricia Bullrrich</option>
            </select>
          </div>

          <div class="select-control">
            <label>¿Qué servicio necesitás?</label>
            <select  id="servicio" name="servicio">
                <option  value="value1"></option>
                <option  value="Tintura">Tintura</option>
                <option  value="Pilates">Pilates</option>
                <option  value="Limpieza de cutis">Limpieza de cutis</option>
            </select>
          </div>

          <div class="boton">
            <button id="myButton">ACEPTAR</button>
          </div>
        </form>
        </div>
    </div>
</div>
</section>

    <!-- VISTA 2 -->

<section>
  <div class="container">    
    <div class="col1">
        <div>
            <img id="arrow" src="/home/slimshady/shiftsystem/src/assets/Arrow.svg" alt="arrow">

            <h1 id="dato">Datos de la reserva:</h1>      
            <p id="lugar"></p>       
            <p id="profesional"></p>        
            <p id="servicio"></p>
        </div>
    </div>

    <div class="col2">

        <form action="index3.html">
            <h1 id="titulo2">¡Completá el formulario <br>para finalizar el proceso!</h1>

            <div class="form-control">
                <label for="nombre">Nombre y apellido:</label>
                <input type="text" name="nombre" id="nombre" required="required">
            </div>

            <div class="form-control">   
                <label for="email">E-mail:</label>
                <input type="email" name="email" id="email" required="required">
            </div> 
            
            <div class="form-control">  
                <label for="telefono">Teléfono:</label>
                <input type="text" name="telefono" id="telefono" required="required">
            </div> 
            
            <div class="form-control"> 
                <label for="mensaje">Mensaje:</label>
                <input type="text" name="mensaje" id="inputMensaje" required="required">
            </div>

            <div class="boton">
                <button  id="myButton">ACEPTAR</button>
            </div>
        </form>
    
    </div>
  </div>
</section>

    <!-- VISTA 3 -->

<section>
<div class="container">
    <div class="col1">
        <h1>¡Tu reserva se ha realizado con éxito!</h1>
    </div>

    <div class="col2">
        <img src="/home/slimshady/shiftsystem/src/assets/Women day-rafiki 1.svg" alt="ilustracion">
    </div>
</div>
</section>

</body>
</template>

<script>
export default {
  name: 'HelloWorld',
  // props: {
  //   msg: String
  // }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Lexend+Exa:wght@300&display=swap');

*{
    margin: 0;
    padding: 0;
}

body{
    overflow: hidden;
}  

section{    
    align-items: start;
    width: 100vw;
    height: 100vh;
    background: url('/home/slimshady/shiftsystem/src/assets/background.png') no-repeat;
    display: flex;
    justify-content: center;
    align-items: center;
}

.container{
    display: grid;
    grid-template-columns: 1fr 1fr;

    width: 1197px;
    height: 597px;

    background: rgba(26, 87, 157, 0.5);
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    border-radius: 8px;
}

/* VISTA 1 */
/* IZQUIERDA */
.col1{
    display: flex;
    justify-content: right;
    align-items: center;
}

img{ 
    width: 456px;
    height: 467px;
    display: block;
}

/* DERECHA */

.col2{
    display: flex;
    justify-content: left;
    align-items: center;
}

select{
    width: 375px;
    height: 48px;
    margin-bottom: 10px;
    display: block;
}

label{
    font-family: 'Lexend Exa';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 20px;
    color: #FFFFFF;
    display: block;
} 

.boton{
    text-align: center;
}

button{
    border-style: none;
    width: 171px;
    height: 48px;
    background: #195A9C;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    border-radius: 0px;
    font-family: 'Lexend Exa';
    font-style: normal;
    font-weight: 400;
    font-size: 22px;
    line-height: 28px;
    text-align: center;
    color: #FFFFFF;
    cursor: pointer;
    border: none;
    transition: 0.3s;
    margin: 10px;
}

button:hover {
    box-shadow: 0 5px 10px 0 #6eb4fa;
    transition: 0.3s;
}

/* VISTA 2 */
/* IZQUIERDA */

.col1{
    display: flex;
    justify-content: center;
    align-items: center;
}

#arrow{
    position: absolute;
    left: 120px;
    top: 85px;
    cursor: pointer;
}

#dato{
    font-family: 'Lexend Exa';
    align-items: center;
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    text-align: center;
    margin-bottom: 20px;

    color: #FFFFFF;
    line-height: 40px;
    width: 444px;
    background: rgba(72, 183, 185, 0.5);
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);    
}

p{
    font-family: 'Lexend Exa';
    align-items: center;
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    text-align: center;
    margin-bottom: 20px;

    color: #FFFFFF;
    line-height: 40px;
    width: 444px;
    background: rgba(72, 183, 185, 0.5);
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);    

}

/* DERECHA */
.col2{
    display: flex;
    justify-content: center;
    align-items: center;
}

#titulo2{    
    font-family: 'Lexend Exa';
    font-style: normal;
    font-weight: 400;
    font-size: 22px;
    line-height: 28px;
    margin-bottom: 10px;
    color: #FFFFFF;
}

input{
    width: 375px;
    height: 48px;
    background: #FFFFFF;
    border-radius: 0px;
    display: block;
    margin-bottom: 10px;
}

label{
    font-family: 'Lexend Exa';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 20px;
    display: block;
    color: #FFFFFF;
}

#inputMensaje{
    width: 375px;
    height: 98px;
    background: #FFFFFF;
    border-radius: 0px;
    margin-bottom: 10px;
    display: block;
}

.boton{
    text-align: center;
}

button{
    width: 171px;
    height: 48px;
    border: none;
    background: #1A579D;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    border-radius: 0px;
    cursor: pointer;
    font-family: 'Lexend Exa';
    font-style: normal;
    font-weight: 400;
    font-size: 22px;
    line-height: 28px;
    text-align: center;
    color: #FFFFFF;
    margin: 10px;
}

button:hover {
    box-shadow: 0 5px 10px 0 #6eb4fa;
    transition: 0.3s;
} 


/* VISTA 3 */
/* IZQUIERDA */

.col1{
    display: flex;
    justify-content: center;
    align-items: center;
}

h1{
    display: block;
    width: 335px;
    height: 59px;
    left: 283px;
    top: 459px;

    font-family: 'Lexend Exa';
    font-style: normal;
    font-weight: 400;
    font-size: 22px;
    line-height: 28px;
    text-align: center;

    color: #FFFFFF;
}

/* DERECHA */
.col2{
    display: flex;
    justify-content: left;
    align-items: center;
}

img{
    display: block;
}
</style>
