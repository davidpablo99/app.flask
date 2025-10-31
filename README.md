# Flask Livros Project

Um projeto Flask para gerenciamento de livros com funcionalidades CRUD (Create, Read, Update, Delete).

## Funcionalidades

- ✅ Listagem de livros
- ✅ Adição de novos livros
- ✅ Edição de livros existentes
- ✅ Integração com API de filmes (TMDB)
- ✅ Interface responsiva com Bootstrap

## Tecnologias Utilizadas

- **Flask** - Framework web Python
- **SQLAlchemy** - ORM para banco de dados
- **SQLite** - Banco de dados
- **Bootstrap 5** - Framework CSS
- **Jinja2** - Template engine

## Estrutura do Projeto

```
flask/
├── projeto/                 # Pacote principal da aplicação
│   ├── __init__.py         # Inicialização do Flask e SQLAlchemy
│   ├── routes.py           # Rotas da aplicação
│   ├── livro.py           # Modelo do livro
│   ├── lista_filmes.py    # Integração com API de filmes
│   └── templates/         # Templates HTML
├── instance/              # Banco de dados SQLite
├── .venv/                # Ambiente virtual Python
├── app.py                # Arquivo de configuração alternativo
└── requirements.txt      # Dependências (a ser criado)
```

## Como Executar

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/SEU_USUARIO/flask-livros-project.git
   cd flask-livros-project
   ```

2. **Crie e ative o ambiente virtual:**
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # No Windows: .venv\Scripts\activate
   ```

3. **Instale as dependências:**
   ```bash
   pip install flask flask-sqlalchemy requests
   ```

4. **Execute a aplicação:**
   ```bash
   FLASK_APP=projeto flask run --debug --port 5050
   ```

5. **Acesse no navegador:**
   ```
   http://127.0.0.1:5050
   ```

## Rotas Disponíveis

- `/` - Página inicial
- `/livros` - Lista de livros
- `/add_livro` - Adicionar novo livro
- `/<id>/atualiza_livro` - Editar livro
- `/filmes/<propriedade>` - Lista de filmes por categoria
- `/diario` - Diário de notas
- `/sobre` - Página sobre

## Banco de Dados

O projeto usa SQLite com as seguintes tabelas:

### Livro
- `id` (Integer, Primary Key)
- `nome` (String, Nome do livro)
- `descricao` (String, Descrição do livro)
- `valor` (Float, Preço do livro)

## Contribuição

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## Autor

Desenvolvido como projeto de aprendizado Flask.