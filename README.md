# Pagina_Web_Basica
Página web básica.

# Index.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="styles.css">
  <title>Document</title>
</head>
<body>
  <header class="animado">
    <div class="header_nav">
      <div class="contenedor">
        <h1>Institución Universitaria Pascual Bravo</h1>
        <nav>
          <a href="https://pascualbravo.edu.co/" target="_blank">Inicio</a>
          <a href="https://pascualbravo.edu.co/academico/bibliotecas/" target="_blank">Biblioteca</a>
          <a href="#">Contacto</a>
        </nav>
      </div>
    </div>

    <section class="banner contenedor">
      <section class="banner_titulo">
        <h2>¡Bienvenido a tu <br>segundo hogar!</br></h2>
        <a href="#registro" class="Estudia_con_nosotros">Estudia con nosotros</a>
      </section>
      <div class="banner_imagen">
        <img src="Libros.png" alt="">
      </div>
      <div class="efectos">
        <div class="efecto"></div>
        <div class="efecto"></div>
        <div class="efecto"></div>
        <div class="efecto"></div>
        <div class="efecto"></div>
      </div>
    </section>
    <section class="registro" id="registro">
      <h4>Formulario de registro</h4>
      <input class="control" type="text" name="nombres" id="nombres" placeholder="Ingrese su nombre">
      <input class="control" name="apellidos" id="apellidos" placeholder="Ingrese su apellido">
      <input class="control" name="correo" id="correo" placeholder="Ingrese su correo">
      <br><br>
      <input class="boton" type="submit" value="Registrar">
    </section>
  </header>
</body>
</html>

# styles.css
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body{
  font-family: Georgia, serif;
}

.contenedor{
  width: 90%;
  max-width: 1200px;
  margin: auto;
}

.animado{
  width: 100%;
  height: 100vh;
  background: linear-gradient(to right, #1280c4, #0313c7);
  position: relative;
}

.header_nav{
  width: 100%;
  position: absolute;
  top: 0;
  left: 0;
}

.header_nav .contenedor{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px;
}

.header_nav h1{
  color: white;
  font-family: 'Gagalin';
  font-size: 40px;
}

.header_nav nav a{
  color:aliceblue;
  text-decoration: none;
  margin-right: 10px;
}

.banner{
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100%;
}

.banner_titulo h2{
  color:white;
  font-size: 60px;
  font-weight: 800;
  margin-bottom: 20px;
}

.banner_titulo .Estudia_con_nosotros{
  color: #fff;
  font-size: 20px;
  text-decoration: none;
  display: inline-block;
  background: rgb(19, 19, 128);
  padding: 20px;
}

.banner_imagen img{
  width: 350px;
  display: block;
  margin-right: 150px;
}

.efecto{
  border-radius: 50%;
  background: rgb(255, 255, 255);
  opacity: .3;

  position: absolute;
  bottom: -150vh;

  animation: efectos 3s linear infinite;
}

.efecto:nth-child(1){
  width: 80px;
  height: 80px;
  left: 5%;
  animation-duration: 3s;
  animation-delay: 2s;
}

.efecto:nth-child(2){
  width: 100px;
  height: 100px;
  left: 30%;
  animation-duration: 3s;
  animation-delay: 6s;
}

.efecto:nth-child(3){
  width: 60px;
  height: 60px;
  left: 50%;
  animation-duration: 3s;
  animation-delay: 4s;
}

.efecto:nth-child(4){
  width: 70px;
  height: 70px;
  left: 75%;
  animation-duration: 3s;
  animation-delay: 5s;
}

.efecto:nth-child(5){
  width: 80px;
  height: 80px;
  left: 85%;
  animation-duration: 3s;
  animation-delay: 1s;
}

@keyframes efectos {
  0%{
    bottom: 0;
    opacity: 0;
  }
  30%{
    transform: translate(30px);
  }
  50%{
    opacity: .4;
  }
  100%{
    bottom: 100vh;
    opacity: 0;
  }
}


.registro{
  width: 400px;
  background: rgb(28, 18, 66);
  padding: 50px;
  margin-left: 500px;
  margin-top: 200px;
  margin-bottom: 100px;
  border-radius: 4px;
  font-family: 'Calibri';
  color: white;
}
