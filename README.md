# Projeto CRUD com Autenticação em PHP + PDO

Sistema completo de Cadastro, Leitura, Atualização e Exclusão (CRUD) com autenticação de usuários, desenvolvido em PHP com PDO e MySQL.

## Funcionalidades

- Registro e login de usuários com senha criptografada (bcrypt)
- Listagem de todos os usuários no portal
- Edição de dados do usuário
- Exclusão de usuário com confirmação
- Controle de sessão e logout
- Saudação dinâmica (Bom dia / Boa tarde / Boa noite)

## Estrutura do Projeto

\```
Projeto_crud/
├── index.php        # Página de login
├── registrar.php    # Cadastro de novo usuário
├── portal.php       # Listagem de usuários (área restrita)
├── editar.php       # Edição de usuário
├── deletar.php      # Exclusão de usuário
├── logout.php       # Encerramento de sessão
├── bdcrud.sql       # Script SQL do banco de dados
├── classes/
│   ├── Database.php # Classe de conexão PDO
│   └── Usuario.php  # Classe com operações CRUD e autenticação
└── config/
    └── config.php   # Inicialização da conexão
\```

## Como Executar

### Pré-requisitos
- PHP 7.4+ com extensão PDO_MySQL
- MySQL 5.7+ ou MariaDB
- Servidor web (Apache/Nginx) ou PHP built-in server

### Passo a Passo

1. **Clone o repositório:**
   https://github.com/Guilherme-SRibeiro/desafio9.git
   cd Projeto_crud
   \```

2. **Importe o banco de dados:**
   \```bash
   mysql -u root -p < bdcrud.sql
   \```

3. **Configure a conexão** em `classes/Database.php` se necessário (host, usuário, senha).

4. **Inicie o servidor:**
   \```bash
   php -S localhost:8000
   \```

5. **Acesse no navegador:** `http://localhost:8000`

## Tecnologias Utilizadas

- PHP 8+
- PDO (PHP Data Objects)
- MySQL
- HTML5 / CSS3
- Sessões PHP
