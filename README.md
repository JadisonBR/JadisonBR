<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cadastro de Funcionários</title>
    <link rel="stylesheet" href="style.css">
    <script src="script.js" defer></script>
</head>
<body>

    <main class="container">
        <header class="cabecalho">
            <div class="icone">👥</div>
            <h1>Cadastro de Funcionários</h1>
            <p>Preencha os dados para cadastrar um novo funcionário.</p>
        </header>

        <form id="formFuncionario">

            <h2>Dados pessoais</h2>

            <div class="campo">
                <label for="nome">Nome completo *</label>
                <input type="text" id="nome" name="nome"
                       placeholder="Digite o nome completo" required>
            </div>

            <div class="linha">
                <div class="campo">
                    <label for="cpf">CPF *</label>
                    <input type="text" id="cpf" name="cpf"
                           placeholder="000.000.000-00"
                           maxlength="14" required>
                </div>

                <div class="campo">
                    <label for="nascimento">Data de nascimento *</label>
                    <input type="date" id="nascimento"
                           name="nascimento" required>
                </div>
            </div>

            <div class="linha">
                <div class="campo">
                    <label for="email">E-mail *</label>
                    <input type="email" id="email" name="email"
                           placeholder="funcionario@email.com" required>
                </div>

                <div class="campo">
                    <label for="telefone">Telefone *</label>
                    <input type="tel" id="telefone" name="telefone"
                           placeholder="(00) 00000-0000" required>
                </div>
            </div>

            <h2>Dados profissionais</h2>

            <div class="linha">
                <div class="campo">
                    <label for="cargo">Cargo *</label>
                    <input type="text" id="cargo" name="cargo"
                           placeholder="Ex.: Assistente administrativo"
                           required>
                </div>

                <div class="campo">
                    <label for="departamento">Departamento *</label>
                    <select id="departamento" name="departamento" required>
                        <option value="">Selecione</option>
                        <option>Administrativo</option>
                        <option>Recursos Humanos</option>
                        <option>Financeiro</option>
                        <option>Tecnologia da Informação</option>
                        <option>Comercial</option>
                        <option>Marketing</option>
                        <option>Operacional</option>
                    </select>
                </div>
            </div>

            <div class="linha">
                <div class="campo">
                    <label for="admissao">Data de admissão *</label>
                    <input type="date" id="admissao"
                           name="admissao" required>
                </div>

                <div class="campo">
                    <label for="salario">Salário (R$) *</label>
                    <input type="number" id="salario" name="salario"
                           placeholder="Ex.: 2500.00"
                           min="0" step="0.01" required>
                </div>
            </div>

            <div class="campo">
                <label for="status">Status do funcionário *</label>
                <select id="status" name="status" required>
                    <option value="Ativo">Ativo</option>
                    <option value="Em experiência">Em experiência</option>
                    <option value="Afastado">Afastado</option>
                </select>
            </div>

            <div class="botoes">
                <button type="reset" class="btn-limpar">
                    Limpar
                </button>
                <button type="submit" class="btn-cadastrar">
                    Cadastrar funcionário
                </button>
            </div>

            <p id="mensagem" role="status" aria-live="polite"></p>
        </form>

        <section class="resultado">
            <h2>Funcionários cadastrados</h2>
            <p id="contador">Total de funcionários: 0</p>
            <div class="tabela-container">
                <table>
                    <thead>
                        <tr>
                            <th>Nome</th>
                            <th>Cargo</th>
                            <th>Departamento</th>
                            <th>Status</th>
                            <th>Ação</th>
                        </tr>
                    </thead>
                    <tbody id="listaFuncionarios"></tbody>
                </table>
            </div>
        </section>

        <footer>
            Sistema de Cadastro de Funcionários
        </footer>
    </main>

</body>
</html>
