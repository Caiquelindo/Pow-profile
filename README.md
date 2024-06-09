<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mega Checkout de Bolas Esportivas</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        
        .container {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        
        h1, h2 {
            text-align: center;
            color: #333;
        }
        
        .product {
            display: flex;
            justify-content: space-between;
            margin-bottom: 20px;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 8px;
        }
        
        .product img {
            width: 150px;
            height: auto;
        }
        
        .product-details {
            flex: 1;
            margin-left: 20px;
        }
        
        .product-details h2 {
            margin-top: 0;
            color: #333;
        }
        
        .product-details p {
            margin-bottom: 10px;
            color: #555;
        }
        
        .discount {
            color: #FF0000;
            font-weight: bold;
        }
        
        button {
            display: block;
            width: 100%;
            padding: 10px;
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
        button:hover {
            background-color: #0056b3;
        }

        /* Estilos para o Mega Checkout */
        .checkout-container {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background-color: #f9f9f9;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        .checkout-form {
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            font-weight: bold;
            margin-bottom: 5px;
        }

        .form-group input {
            width: calc(100% - 12px);
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        .form-group input[type="submit"] {
            width: 100%;
            padding: 10px;
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .form-group input[type="submit"]:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Escolha sua Bola Esportiva</h1>
        
        <div class="product">
            <img src="bola_futebol.jpg" alt="Bola de Futebol">
            <div class="product-details">
                <h2>Bola de Futebol</h2>
                <p>Preço: R$ 50,00</p>
                <p class="discount">Desconto: 10%</p>
                <button onclick="showCheckoutForm()">Comprar</button>
            </div>
        </div>
        
        <div class="product">
            <img src="bola_basquete.jpg" alt="Bola de Basquete">
            <div class="product-details">
                <h2>Bola de Basquete</h2>
                <p>Preço: R$ 60,00</p>
                <button onclick="showCheckoutForm()">Comprar</button>
            </div>
        </div>
    </div>

    <!-- Mega Checkout -->
    <div id="checkout" class="checkout-container" style="display: none;">
        <h2>Mega Checkout de Bolas Esportivas</h2>
        <div class="checkout-form">
            <form>
                <div class="form-group">
                    <label for="nome">Nome Completo:</label>
                    <input type="text" id="nome" name="nome" required>
                </div>
                <div class="form-group">
                    <label for="cpf">CPF:</label>
                    <input type="text" id="cpf" name="cpf" required>
                </div>
                <div class="form-group">
                    <label for="data_nascimento">Data de Nascimento:</label>
                    <input type="date" id="data_nascimento" name="data_nascimento" required>
                </div>
                <div class="form-group">
                    <label for="numero_cartao">Número do Cartão:</label>
                    <input type="text" id="numero_cartao" name="numero_cartao" required>
                </div>
                <div class="form-group">
                    <input type="submit" value="Finalizar Compra">
                </div>
            </form>
        </div>
    </div>

    <script>
        function showCheckoutForm() {
            document.getElementById("checkout").style.display = "block";
        }
    </script>
</body>
</html>
