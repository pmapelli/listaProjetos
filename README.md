# listaProjetos
Exemplo de Api em NodeJs com Express

Aplicação que armazena lista de projetos com tarefas.

# Rotas

- POST /projects: A rota deve receber id e title dentro corpo de cadastrar um novo projeto dentro de um array no seguinte formato: { id: "1", title: 'Novo projeto', tasks: [] }; Certifique-se de enviar tanto o ID quanto o título do projeto no formato string com àspas duplas.

- GET /projects: Rota que lista todos projetos e suas tarefas;

- PUT /projects/:id: A rota deve alterar apenas o título do projeto com o id presente nos parâmetros da rota;

- DELETE /projects/:id: A rota deve deletar o projeto com o id presente nos parâmetros da rota;

- POST /projects/:id/tasks: A rota deve receber um campo title e armazenar uma nova tarefa no array de tarefas de um projeto específico escolhido através do id presente nos parâmetros da rota;

# Middlewares
- Utilizado em todas rotas que recebem o ID do projeto nos parâmetros da URL que verifica se o projeto com aquele ID existe. 
Se não existe retorna um erro, caso contrário permite a requisição continuar normalmente;

- Middleware global chamado em todas requisições que imprime (console.log) uma contagem de quantas requisições foram feitas na 
aplicação até então;

# Extensões utilizadas
- Express
- Nodemon
