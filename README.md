<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css" />
    <title>Document</title>
    <link rel="stylesheet" href="CSS/style.css">
</head>

<body>
    <header>
        <a href="#" class="logo"><i class="fas fa-utensils"></i></a>

        <nav class="navbar">
            <a class="active" href="#home">home</a>
            <a href="#pratos">Pratos</a>
            <a href="#sobre">Sobre</a>
            <a href="#cardapio">Cardapio</a>
            <a href="#avaliacao">Avaliacao</a>
            <a href="#pedido">Pedido</a>
        </nav>
        <div class="icons">
            <i class="fas fa-bars" id="manu-bars"></i>
            <i class="fas fa-search" id="search-icon"></i>
            <a href="#" class="fas fa-heart"></a>
            <a href="#" class="fas fa-shopping-cart"></a>

      </div>
    </header>

    <form action="" id="search-form">
      <input type="search" placeholder="pesquise aqui..." name="" id="search-box">
      <label for="search-box" class="fas fa-search"></label>
      <i class="fas fa-times" id="close"></i>
    </form>

</body>
</html>

/* CCS */

:root {
    --green: #27ae60;
    --black: #192a56;
    --light-color: #667;
    --box-shadow: 0 .5rem 1.5rem rgba(0,0,0,.1);
}
*{
    font-family: 'nunito', sans-serif;
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
    background: w #fff;
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
    font-weight: bolder;
}
header .logo i{
    color: var(--green);

}
header .navbar a{
    font-size: 1.7rem;
    border-radius: .5rem;
    padding: .5rem 1.5rem;
    color: var(--light-color);
}
header .navbar a.active, header .navbar a:hover {
    color: #fff;
    background: var(--green);
}
header .icons i, header .icons a{
    cursor: pointer;
    margin-left: 5rem;
    height: 4.5rem;
    line-height: 3.5rem;
    width: 4.5rem;
    text-align: center;
    font-size: 1.7rem;
    color: var(--black);
    border-radius: 50%;
    background: #eee;
} 
header .icons i:hover, header .icons a:hover{
    color: #fff;
    background: var(--green);
    transform: rotate(360deg);
}
#search-form{
    position: fixed;
    top: -110;
    left: 0;
    height: 100%;
    width: 100%;
    z-index: 1004;
    background: rgba(0,0,0,.8);
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0 1rem;
}
#search-form.active {
    top: 0;
}
#search-form #search-box{
    width: 50rem;
    border-bottom: .1rem solid #fff;
    padding: 1rem 0;
    font-size: 3rem;
    text-transform: none;
    background: none;

}
