<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Página de Login</title>
<style>
body {
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #ff9a9e, #fad0c4);
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
.login-container {
    background: white;
    padding: 30px;
    border-radius: 10px;
    box-shadow: 0 0 15px rgba(0,0,0,0.2);
    text-align: center;
    width: 300px;
}
input {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border-radius: 5px;
    border: 1px solid #ccc;
}
button {
    width: 100%;
    padding: 10px;
    background: #ff4b8b;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
button:hover {
    background: #e63a75;
}
#mensagem {
    margin-top: 15px;
    font-weight: bold;
}
</style>
</head>
<body>
<div class="login-container">
    <h2>Login</h2>
    <input type="text" id="usuario" placeholder="Usuário">
    <input type="password" id="senha" placeholder="Senha">
    <button onclick="login()">Entrar</button>
    <p id="mensagem"></p>
</div>

<script>
function login() {
    const usuario = document.getElementById("usuario").value;
    const senha = document.getElementById("senha").value;

    if(usuario === "Ketilly" && senha === "Amor") {
        window.location.href = "homenagem.html";
    } else {
        document.getElementById("mensagem").innerText = "Usuário ou senha incorretos.";
    }
}
</script>
</body>
</html>
