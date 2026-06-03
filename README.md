<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="pt-BR">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="CSS/style.css">
</head>
<body>

    <header>
        <a href="#" class="logo"><i class="fas fa-utensils"></i></a>
        <nav class="navber">
        <a class="active" href="#home">home</a>
        <a href="#pratos">Pratos</a>
        <a href="#sobre">Sobre</a>
        <a href="#cardapio">Cardapio</a>
        <a href="#avaliacao">Avaliação</a>
        <a href="#pedido">Pedido</a>
      </nav>

      <div class="incons">
        <i class="fas fa-bars" id="manu-bars"></i>
        <i class="fas fa-search" id="search-icon"></i>
        <a href="#" class="fas fa-heart"></a>
        <a href="#" class="fas fa-shopping-cart"></a>


      </div>
    </header>

</body>
</html>

/* CCS */

:root {
    --green: #27ae60;
    --black: #192a56;
    --light-color:#667;
    --box-shadow:0 .5rem rgba(0,0,0,.1);
}
*{
    font-family: 'Nunito' sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    text-transform: capitalize;
    transition: all .2s linear;

}
header{
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    background: white;
    padding: 1rem 7%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    z-index: 1000;
    box-shadow: var(--box-shadow);
}

header .logo{
    color: var(--black);
    font-size: 2.5rem;
    font-weight: bold;
}

header .logo i{
    color: var(--green);

}

header.navbar a{
    font-size: 1.7rem;
    border-radius: .5rem;
    padding: .5rem 1.5rem;
    color: var(--light-color);
}
