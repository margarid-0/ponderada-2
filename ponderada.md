## Design de Arquitetura
![Design de Arquitetura](/mvc.png)


# Nome do Projeto
C³ - Code Conecting Cultures

## Descrição
Este site possui diversas páginas que possibilitam aos estudantes criarem perfis, se auto avaliarem e avaliarem seus pares, receberem feedback e interagirem com o grupo, além de uma visão para o tutor, permitindo-o monitorar o andamento do projeto. Por meio desse sistema, os estudantes podem adquirir um conhecimento mais aprofundado sobre as diversidades culturais, aprimorar suas habilidades de interação intercultural e aprender a atuar de forma eficaz em um contexto multicultural. Assim, este software online é uma ferramenta útil para auxiliar os alunos do programa IBSM na sua aprendizagem intercultural, capacitando-os a serem profissionais de negócios com foco internacional.

## Arquitetura
MVC (Model View Controller)

## Ferramenta de Diagramação
*kitt.lewagon.com*

## Modelos (Models)
- **User**: Gerencia os dados dos usuários, incluindo identificação, tipo, nome, email, senha, identificação do grupo, data de aniversário, país de perspectiva, país de nascimento e gênero.
- **Group**: Guarda informações sobre grupos, incluindo identificação, nome, identificação dos usuários membros e identificação do tutor.
- **Feedback**: Permite que usuários criem e gerenciem feedbacks com conteúdo, identificação do remetente, destinatário e identificação do grupo.

## Controladores (Controllers)
- **User Controller**: Gerencia as operações CRUD (Create, Read, Update, Delete) para usuários.
- **Group Controller**: Lida com as operações CRUD para grupos.
- **Feedback Controller**: Permite a criação, leitura, atualização e exclusão de feedbacks.

## Views (Views)
- **Homepage**: Exibe a página inicial com navbar, perfis, membros do grupo, informações do jogo, indicadores do jogo e logo.
- **Feedback Form**: Fornece um formulário para os usuários submeterem feedbacks e visualizarem feedbacks recebidos.

## Infraestrutura
- O projeto é construído usando JavaScript, usa o Render para hospedagem e se conecta a um banco de dados em postgreSQL que pode ser editado pelo DBeaver.
- A comunicação entre o cliente e o servidor é realizada via internet.

## Justifique as escolhas feitas e como elas impactam o projeto
As escolhas pelas tecnologias citadas se dão por contextos externos do projeto, sendo requisitos da faculdade para o aprendizado durante esse módulo.

## Implicações da Arquitetura
O MVC comporta a escalabilidade do projeto, permitindo que novas funcionalidades sejam adicionadas com de forma simples. Modelos e controladores podem ser expandidos e novas views podem ser introduzidas sem que sejam exigidas grandes reformulações da estrutura e do código já existentes.