<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta http-equiv="X-UA-Compatible" content="ie=edge">
<meta name="Description" content="Enter your description here"/>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/5.1.0/css/bootstrap.min.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
<link rel="stylesheet" href="assets/css/style.css">
<style>
    .painel {
  font-weight: bold;
  box-shadow: rgba(17, 17, 26, 0.1) 0px 0px 16px;
  border-radius: 10px;
}

.painel2 {
  font-weight: bold;
  box-shadow: rgba(17, 17, 26, 0.1) 0px 0px 16px;
}

</style>
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-light bg-info painel2">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">Estácio Brasilia DF</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a class="nav-link active" aria-current="page" href="#">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Link</a>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                            Cadastrar
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <li><a class="dropdown-item" href="#">Pessoa</a></li>
                            <li><a class="dropdown-item" href="#">Cursos</a></li>
                            <li><a class="dropdown-item" href="#">Professores</a></li>
                        </ul>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
                    </li>
                </ul>
                
            </div>
        </div>
    </nav>
    
    <div class="container pt-5">
        <div class="card painel">
            <div class="card-header bg-info">
                CADASTRO DE FUNCIONÁRIO
            </div>
            <div class="card-body">
                <div class="row">
                    <div class="col-md-3">
                        <label for="cpf">CPF</label>
                        <input type="text" class="form-control" name="txtCPF" id="txtCPF">
                    </div>
                    <div class="col-md-6">
                        <label for="cpf">Nome</label>
                        <input type="text" class="form-control" name="txtNome" id="txtNome">
                    </div>
                    <div class="col-md-3">
                        <label for="dataNascimento">Data de Nascimento</label>
                        <input type="date" class="form-control" name="txtDataNascimento" id="txtDataNascimento">
                    </div>
                </div>
                <div class="row">
                    <div class="col-md-6">
                        <label for="nomeMae">Nome da Mãe</label>
                        <input type="text" class="form-control" name="txtNomeMae" id="txtNomeMae">
                    </div>
                    <div class="col-md-6">
                        <label for="NomePai">Nome do Pai</label>
                        <input type="text" class="form-control" name="txtNomePai" id="txtNomePai">
                    </div>
                </div>
                <div class="row">
                    <div class="col-md-4">
                        <label for="">Área de Atuação</label>
                        <select class="form-select" aria-label="Default select example">
                            <option selected>Selecione Uma Opção</option>
                            <option value="1">Desenvolvimento Full Stack</option>
                            <option value="2">Desenvolvimento Front-End</option>
                            <option value="3">Desenvolvimento Back-End</option>
                            <option value="4">Segurança da Informação</option>
                            <option value="5">Requisitos</option>
                            <option value="6">Infraestrutura</option>
                        </select>
                    </div>
                    <div class="col-md-5">
                        <label for="">E-mail</label>
                        <input type="text" class="form-control" name="txtEmail" id="txtEmail">
                    </div>
                    <div class="col-md-3">
                        <label for="">Salário</label>
                        <input type="text" class="form-control" name="txtSalario" id="txtSalario">
                    </div>
                </div>
                <div class="form-group">
                    <label for="">Observação</label>
                    <input type="text" class="form-control" name="txtObs" id="txtObs">
                </div>
            </div>
            <div class="card-footer">
                <div class="row">
                    <div class="col-md-3">
                        <button type="button" class="btn btn-outline-info form-control active">Salvar</button>
                    </div>
                    <div class="col-md-3">
                        <button type="button" class="btn btn-outline-info form-control">Limpar</button>
                    </div>
                    <div class="col-md-3">
                        <button type="button" class="btn btn-outline-info form-control">Excluir</button>
                    </div>
                    <div class="col-md-3">
                        <button type="button" class="btn btn-outline-info form-control">Sair</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/2.9.2/umd/popper.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/5.1.0/js/bootstrap.min.js"></script>
</body>
</html>
