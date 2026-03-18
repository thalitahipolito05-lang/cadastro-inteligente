<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TechConnect - Cadastro Inteligente</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <div class="container">
        <div class="form-container">
            <h1>Criar Conta</h1>
            <p>Junte-se à TechConnect e transforme sua experiência</p>
            
            <form id="cadastroForm" novalidate>
                <!-- Nome Completo -->
                <div class="form-group">
                    <label for="nome">Nome Completo *</label>
                    <input type="text" id="nome" name="nome" 
                           placeholder="Seu nome completo" 
                           required minlength="3" 
                           autocomplete="name">
                    <span class="error-msg" id="nome-error"></span>
                </div>

                <!-- E-mail -->
                <div class="form-group">
                    <label for="email">E-mail *</label>
                    <input type="email" id="email" name="email" 
                           placeholder="seu@email.com" 
                           required autocomplete="email">
                    <span class="error-msg" id="email-error"></span>
                </div>

                <!-- Senha -->
                <div class="form-group">
                    <label for="senha">Senha *</label>
                    <input type="password" id="senha" name="senha" 
                           placeholder="Mínimo 8 caracteres" 
                           required minlength="8">
                    <span class="error-msg" id="senha-error"></span>
                    
                    <!-- Indicador de força da senha (Exercício 5) -->
                    <div class="password-strength">
                        <div class="strength-bar" id="strengthBar"></div>
                    </div>
                    <span class="strength-text" id="strengthText"></span>
                </div>

                <!-- Confirmar Senha -->
                <div class="form-group">
                    <label for="confirmarSenha">Confirmar Senha *</label>
                    <input type="password" id="confirmarSenha" name="confirmarSenha" 
                           placeholder="Digite a senha novamente" 
                           required>
                    <span class="error-msg" id="confirmarSenha-error"></span>
                </div>

                <!-- Botão de Submit -->
                <button type="submit" id="submitBtn">
                    <span class="btn-text">Criar Conta</span>
                    <span class="spinner hidden"></span>
                </button>
            </form>

            <!-- Mensagem de sucesso -->
            <div id="successMessage" class="success-message hidden">
                ✅ Cadastro realizado com sucesso!
            </div>
        </div>
    </div>

    <script src="js/validation.js"></script>
</body>
</html>
