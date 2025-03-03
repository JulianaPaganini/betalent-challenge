Neste projeto, criei uma API simulada utilizando a ferramenta json-server para atuar como o back-end e fornecer os dados dos funcionários consumidos pela página de visualização. O objetivo foi criar um ambiente simples e rápido para testar a integração entre o front-end e a API, sem a necessidade de um back-end real.

Primeiro, instalei o json-server como dependência de desenvolvimento. Com ele, foi possível gerar um servidor RESTful completo a partir de um arquivo JSON. Criei o arquivo db.json, no qual armazenei os dados fictícios dos funcionários, como nome, cargo, data de admissão, telefone e imagem. Esse arquivo passou a ser a base de dados da API.

Em seguida, configurei o servidor do json-server para rodar na porta 3001, expondo os dados através de endpoints como GET /employees, que retorna todos os funcionários, e GET /employees/:id, que busca um funcionário específico. Além disso, configurei os métodos POST, PUT e DELETE para permitir a manipulação de dados, caso seja necessário adicionar, atualizar ou excluir informações.

A integração com o front-end foi feita utilizando a biblioteca axios no React. Quando o componente da tabela é carregado, ele faz uma requisição GET para obter os dados da API e exibi-los. Também implementei um filtro de pesquisa para que o usuário possa procurar rapidamente entre os funcionários, utilizando os campos de nome e cargo.

Essa abordagem me permitiu testar a visualização e interação com os dados de forma ágil, sem a necessidade de um back-end completo, facilitando o desenvolvimento e permitindo validar a interface e a integração com a API.
