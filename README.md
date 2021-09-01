- 👋 Hi, I’m @Beluhga
- 👀 Tenho interesse em ser um Dev Front-End
- 🌱 Atualmente estou aprendendo JS
- 💞️ Estou procurando colaborar em tudo o que eu aprender.
- 📫 Como me encontrar michaelfernando@live.com

HTML
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" id="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemplo - Menu com FLEX-DROW</title>
    <link rel="stylesheet" href="estilo.css">
  
  </head>
  <body>
    <nav>
      <ul class="container">
        <li class="item primeiro">
          <a href="#"><span class="text">Futebol</span></a>

        </li>
        <li class="item segundo">
          <a href="#"><span class="text">Natação</span></a>
        </li>
        <li class="item terceiro">
          <a href="#"><span class="text">Basquete</span></a>
        </li>
        <li class="item quarto">
          <a href="#"><span class="text">Corrida</span></a>
        </li>
        
      </ul>
    </nav>
  </body>
</html>
--->
CSS

boddy, ul {padding:0; margin:0}

.container{
    width: 100vw;
    height: 100vh;
    display: flex;
    flex-direction: row;
}

.item {
    flex-grow:1;
    background-position: center;
    background-size: cover;
    -webkit-filter:grayscale(100%);
    filter:grayscale(100%);
    position:relative;
    list-style:none;
    transition:all .7s ease-in-out;
}

.item:hover{
    flex-grow:10;
    -webkit-filter:grayscale(0%);
    filter:grayscale(0%)
}

.item a{
    width:100%;
    height:100%;
    display:flex;
    position:absolute;
    align-items:center;
    justify-content:center;
    text-decoration:none;
}
.text{
    font-size:0;
    font-family:sans-serif;
    font-weight:bold;
    text-transform:uppercase;
    color:white;
    text-decoration:none;
    transition:all .5s ease-in-out;
}
.item:hover .text{
    font-size:32px;
    text-shadow:2px epx 12ps black;
}
.primeiro{
    background-image:url(img/item1.png);
}
.segundo{
    background-image:url(img/item2.png);
}
.terceiro{
    background-image:url(img/item3.png);
}
.quarto{
    background-image:url(img/item4.png);
}

@media screen and (max-width:768px){
    .container{
        flex-direction:column;

    }
    .text{
        font-size: 16px;
    }
}




