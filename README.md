<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Loja de Produtos Gerais</title>
    <link href="https://fonts.googleapis.com/css2?family=Sacramento&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">
                <h1>Loja Geral</h1>
            </div>
            <ul class="nav-links">
                <li><a href="#">Início</a></li>
                <li><a href="#">Produtos</a></li>
                <li><a href="#">Contato</a></li>
            </ul>
        </nav>
    </header>

    <section class="intro">
        <h2>Bem-vindo à Loja Geral</h2>
        <p>Encontre os melhores produtos para o seu dia a dia!</p>
    </section>

    <section class="products">
        <h3>Produtos em Destaque</h3>
        <div class="product-card">
            <img src="https://sgfm.elcorteingles.es/SGFM/dctm/MEDIA03/201903/29/00194611000269____3__1200x1200.jpg" alt="Produto 1">
            <h4>Produto 1</h4>
            <p>R$ 1581,90</p>
            <button>Comprar</button>
        </div>
        <div class="product-card">
            <img src="https://th.bing.com/th/id/R.543f0b7f9eea639a5b104ea92e0e391f?rik=EYuH5Y%2fd0bWCzg&riu=http%3a%2f%2fwww.celex.com%2fcdn%2fshop%2ffiles%2fROSA16_1200x1200.jpg%3fv%3d1726588419&ehk=xLKWSNSvDfq4UmhqY0pSEVV3iM90IdGWnbvHOTcpr7Q%3d&risl=&pid=ImgRaw&r=0" alt="Produto 2">
            <h4>Produto 2</h4>
            <p>R$ 5000,90</p>
            <button>Comprar</button>
        </div>
        <div class="product-card">
            <img src="https://netpc.uy/wp-content/uploads/2022/09/5-18.jpg" alt="Produto 3">
            <h4>Produto 3</h4>
            <p>R$ 3599,90</p>
            <button>Comprar</button>
        </div>
    </section>

    <footer>
        <p>© 2025 Loja Geral - Todos os direitos reservados</p>
    </footer>

    <script src="script.js"></script>
</body>
<style>
    /* Definições gerais */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Sacramento', cursive;
    background-color: #000;
    color: #fff;
}

/* Cabeçalho */
header {
    background-color: #6a0dad; /* Roxo */
    padding: 20px;
    text-align: center;
}

header nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

header .logo h1 {
    font-size: 3rem;
    color: #fff;
}

header .nav-links {
    list-style: none;
    display: flex;
    gap: 20px;
}

header .nav-links li {
    font-size: 1.2rem;
}

header .nav-links li a {
    text-decoration: none;
    color: #fff;
}

header .nav-links li a:hover {
    color: #32cd32; /* Verde */
}

/* Seção de introdução */
.intro {
    text-align: center;
    padding: 50px;
    background-color: #4b0082; /* Roxo escuro */
}

.intro h2 {
    font-size: 2.5rem;
    margin-bottom: 10px;
}

.intro p {
    font-size: 1.2rem;
    color: #ff6347; /* Tom de laranja-avermelhado */
}

/* Seção de produtos */
.products {
    display: flex;
    justify-content: space-around;
    padding: 40px;
    background-color: #333;
    flex-wrap: wrap;
}

.products h3 {
    width: 100%;
    text-align: center;
    margin-bottom: 20px;
    font-size: 2rem;
    color: #fff;
}

.product-card {
    background-color: #222;
    padding: 20px;
    text-align: center;
    border-radius: 10px;
    width: 200px;
    margin: 15px;
}

.product-card img {
    width: 100%;
    height: auto;
    border-radius: 5px;
}

.product-card h4 {
    margin-top: 15px;
    font-size: 1.2rem;
    color: #fff;
}

.product-card p {
    font-size: 1.1rem;
    color: #32cd32; /* Verde */
    margin-top: 5px;
}

.product-card button {
    background-color: #ff6347; /* Tom de laranja-avermelhado */
    color: white;
    padding: 10px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    margin-top: 10px;
}

.product-card button:hover {
    background-color: #ff4500; /* Cor mais escura */
}

/* Rodapé */
footer {
    background-color: #4b0082; /* Roxo escuro */
    text-align: center;
    padding: 15px;
    margin-top: 40px;
}

footer p {
    color: #fff;
    font-size: 1rem;
}

</style>
<script>
    // Função para simular a compra de um produto
document.querySelectorAll('.product-card button').forEach(button => {
    button.addEventListener('click', () => {
        alert('Produto adicionado ao carrinho!');
    });
});

</script>
</html>

