<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Burger Mania - Seu Cardápio Digital</title>
    <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Open+Sans:wght@400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #393a3b;
            --secondary-color: #ffd800;
            --dark-color: #ff9d00;
            --light-color: #4f4d4d;
            --text-color: #d38237;
        }

        body {
            font-family: 'Open Sans', sans-serif;
            margin: 0;
            background-color: var(--light-color);
            color: var(--text-color);
            line-height: 1.6;
        }

        header {
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 2.5rem 1rem;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        header h1 {
            font-family: 'Bebas Neue', cursive;
            font-size: 3.5rem;
            margin-bottom: 0.5rem;
            letter-spacing: 2px;
        }

        header p {
            font-size: 1.1rem;
            margin-top: 0;
        }

        .container {
            max-width: 900px;
            margin: 30px auto;
            padding: 0 20px;
        }

        .categoria {
            font-family: 'Bebas Neue', cursive;
            font-size: 2.5rem;
            color: var(--dark-color);
            border-bottom: 4px solid var(--secondary-color);
            padding-bottom: 10px;
            margin-top: 40px;
            margin-bottom: 25px;
            text-align: center;
        }

        .item {
            display: flex;
            flex-direction: column; /* Para empilhar em telas pequenas */
            justify-content: space-between;
            align-items: flex-start; /* Alinhar itens no início */
            margin: 20px 0;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.2s ease-in-out;
        }

        .item:hover {
            transform: translateY(-5px);
        }

        .detalhes {
            flex-grow: 1; /* Permite que os detalhes ocupem o espaço disponível */
            margin-bottom: 10px; /* Espaço entre detalhes e preço em telas pequenas */
        }

        .detalhes h3 {
            margin: 0;
            color: var(--primary-color);
            font-size: 1.8rem;
            font-family: 'Bebas Neue', cursive;
            letter-spacing: 1px;
        }

        .detalhes p {
            margin: 8px 0 0;
            font-size: 1rem;
            color: var(--text-color);
        }

        .preco {
            font-weight: bold;
            color: var(--dark-color);
            font-size: 1.6rem;
            align-self: flex-end; /* Alinha o preço à direita em telas maiores */
        }
        
        .whatsapp-button {
            display: block;
            width: fit-content;
            margin: 40px auto;
            background-color: #25d366; /* Verde WhatsApp */
            color: white;
            padding: 15px 30px;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            font-size: 1.3rem;
            transition: background-color 0.3s ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .whatsapp-button:hover {
            background-color: #1da851;
        }

        footer {
            text-align: center;
            padding: 25px;
            font-size: 0.9rem;
            color: #777;
            margin-top: 50px;
            background-color: var(--dark-color);
            color: var(--light-color);
        }

        /* Responsividade para telas maiores */
        @media (min-width: 768px) {
            .item {
                flex-direction: row; /* Volta a alinhar lado a lado em telas maiores */
                align-items: center;
            }
            .detalhes {
                margin-bottom: 0;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>OXE BURGUER</h1>
    <p>Os hambúrgueres mais suculentos da cidade!</p>
    <p>Aberto de quinta a Domingo, das 18h às 23h</p>
</header>

<div class="container">

    <h2 class="categoria">Hambúrgueres Especiais</h2>
    
    <div class="menu-column">
                    <h3>HAMBÚRGUERS</h3>
                    <div class="menu-item">
                        <h4>X ONION <span>R$ 20</span></h4>
                        <p>Pão tradicional, Blend 150g, fatia de queijo cheddar, anel de onion, molho barbecue</p>
                    </div>
                    <div class="menu-item">
                        <h4>X COALHO <span>R$ 20</span></h4>
                        <p>Pão tradicional, blend 150g, queijo coalho, cebola crispim, bacon, molho especial</p>
                    </div>
                    <div class="menu-item">
                        <h4>X BACON <span>R$ 20</span></h4>
                        <p>Pão tradicional, blend 150g, fatia de queijo cheddar, bacon, cebola caramelizada, molho especial</p>
                    </div>
                    <div class="menu-item">
                        <h4>X CHARQUE <span>R$ 25</span></h4>
                        <p>Pão tradicional, blend 150g, queijo coalho, charque desfiada, cebola caramelizada, molho especial</p>
                    </div>
                    <div class="menu-item">
                        <h4>DUPLO CHEESE <span>R$ 20</span></h4>
                        <p>Pão tradicional, duplo smash 80g, creme cheese, farofa de bacon</p>
                    </div>
                     <div class="menu-item">
                        <h4>ARTESANAL SIMPLES <span>R$ 12</span></h4>
                        <p>Pão tradicional, blend 150g, fatia de queijo cheddar, cebola caramelizada, molho especial</p>
                    </div>
                </div>

                <div class="menu-column right-column">
                    
                    <h3>PORÇÕES</h3>
                    <div class="menu-item simple-item">
                        <h4>Batata p <span>R$ 7</span></h4>
                    </div>
                    <div class="menu-item simple-item">
                        <h4>Batata g <span>R$ 12</span></h4>
                    </div>
                    <div class="menu-item simple-item">
                        <h4>Batata especial <span>R$ 20</span></h4>
                    </div>
                    <div class="menu-item simple-item">
                        <h4>Porção onios <span>R$ 15</span></h4>
                    </div>
                    
                    <h3 class="mt-3">BEBIDAS</h3>
                    <div class="menu-item simple-item">
                        <h4>Coca cola 1 litro <span>R$ 10</span></h4>
                    </div>
                    <div class="menu-item simple-item">
                        <h4>Antárctica <span>R$ 10</span></h4>
                    </div>
                    <div class="menu-item simple-item">
                        <h4>Sukita <span>R$ 10</span></h4>
                    </div>
                    <div class="menu-item simple-item">
                        <h4>Água mineral <span>R$ 3</span></h4>
                    </div>
                </div>
            </div>
        </section>
        
        <section id="delivery" class="section delivery-section">
            <h2 class="section-title">🛵 Delivery & Contato</h2>
            <p>Peça o seu Oxe Burguer hoje e receba na sua casa! Qualidade e sabor garantidos.</p>
            
            <div class="contact-info">
                <p>📍 **Instagram para Pedidos:**</p>
                <a href="https://www.instagram.com/oxeburguer.pe_/" target="_blank" class="instagram-link">@oxeburguer.pe</a>
                <p>📞 **Telefone/WhatsApp para Pedidos*: (81) 99519-3045</p>
            </div>

          
