<div align="center">
<picture>
    <source srcset="https://imgur.com/5bYAzsb.png" media="(prefers-color-scheme: dark)">
    <source srcset="https://imgur.com/Os03JoE.png" media="(prefers-color-scheme: light)">
    <img src="https://imgur.com/Os03JoE.png" alt="Escudo UNAL" width="350px">
</picture>

<h3>AUTOMATIZACIÓN DE PROCESOS DE MANUFACTURA</h3>

<h1>Módulo 8 - Sistema de supevisión SCADA</h1>

<h2>Mep Mep Raideres</h2>

<h5>Joan Sebastian Arcila <br>
    Juan Sebastian Daleman Martinez<br>
    Daniel Santiago Muñoz Bernal<br>
    Maria Alejandra Pérez Petro<br>
    Emma Carolina Sarmiento Cabarcas</h5>

<h6>Universidad Nacional de Colombia<br>
    Facultad de Ingeniería<br>
    Departamento de Ingeniería Mecánica y Mecatrónica<br>
    Bogotá, Colombia<br>
    2025</h6>
</div>


<details>
    <summary>🗂️ Tabla de Contenido</summary>

<!-- TOC -->
- [1. 📡 Estructura de cominicaciones](#1--estructura-de-cominicaciones)
- [2. 🧩 Componentes del SCADA](#2--componentes-del-scada)
- [3. ⚙️ Funcionamiento del SCADA](#3-️-funcionamiento-del-scada)




</details>

# 1. 📡 Estructura de cominicaciones

Para el desarrollo del la interfaz HMI se comenzo creando la estructura de comunicaciones de los elementos que interactuarian para su desarrollo y validación. Como se muestra en la imagen se creo un contenedor de Azure el cual tiene una imagen de ignition en donde se desarrollo la creación del HMI este recibe datos por medio de una comunicación MQTT de un ignition corriendo de forma local en un computador. Adicionalmente en el computador se tendria corriendo Node-red para una intergración de google assistan, Studio 5000 para la progrmación del PLC y NX para la visualización del comportamiento de la fabrica al ejecutarse toda la logica.

<div align="center">
    <img src="https://imgur.com/yMipFHe.png" alt="Estructura comunicaciones" width="800px">
</div>

# 2. 🧩 Componentes del SCADA

Es asi que usando el ignition designer se desarrollo el HMI aprovechando diferentes elementos de este se creo una interfaz navegable con un menú general, una parte especifica para las máquinas en este caso las bandas donde se pueden ver loes elementos de control y una variable de interes que es la velocidad del motor, una página para visualizar historicos y una para visualizar alarmas. Asi mismo ver si algun elemento esta en la entrada o salida de la banda y el estado del motor si esta parado o andando.

**Página principal**
<div align="center">
    <img src="https://imgur.com/3nfp9h1.png" alt="Home_page" width="800px">
</div>

**Página máquina**
<div align="center">
    <img src="https://imgur.com/B94Q8ul.png" alt="Conveyor_page" width="800px">
</div>

**Página historicos**
<div align="center">
    <img src="https://imgur.com/IcadNnp.png" alt="Chars_page" width="800px">
</div>

**Página alarmas**
<div align="center">
    <img src="https://imgur.com/vstfMae.png" alt="Alarms_page" width="800px">
</div>


[IP del SCADA azure](http://20.241.187.29:8088/data/perspective/client/Cloud_1)

Credenciales:
- admin password


# 3. ⚙️ Funcionamiento del SCADA

En el siguiente video se puede ver todo el proceso del SCADA junto a la validación de los diferentes elementos de este.

<div align="center">
  <a href="https://www.youtube.com/watch?v=09Rm8bv1LeY">
    <img src="https://img.youtube.com/vi/09Rm8bv1LeY/0.jpg" alt="video dual boot Ubuntu"  width="600px">
  </a>
</div>


