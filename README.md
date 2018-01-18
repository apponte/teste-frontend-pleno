# Teste Apponte - Front-End Pleno
Desenvolver uma aplicação HTML5

## Instruções
- Siga as especificações abaixo.
- Crie um README com as instruções para compilar e rodar o projeto.
- O link do projeto rodando em produção deverá ser enviado ao término do prazo.

## Especificações tecnicas
- Utilizar diretrizes do [Google Material Design](https://www.google.com/design/spec/material-design/introduction.html)
- Utilizar a [API de busca do YouTube](https://developers.google.com/youtube/v3/docs/search/list)
- Mobile first e responsivo
- Utilizar o framework Angular
- Testes automatizados é um diferencial

## Especificações funcionais
### Tela Inicial
Essa tela terá um formulário de busca posicionado no meio da tela com campo de texto com placeholder "Pesquisar" e um botão "Buscar". Esse formulário deverá ter validação.

Essa busca deverá chamar a url https://www.googleapis.com/youtube/v3/search?part=id,snippet&q={termo_de_busca}&key={API_KEY}

Ao fazer a busca, o formulário deve ser movido para o topo da tela usando css animate e mostrar a lista de resultados com os campos título, descrição, thumbnail e um link para a página de detalhes.

Essa página deverá ter paginação, utilizando os [recursos de paginação da api](https://developers.google.com/youtube/v3/guides/implementation/pagination?hl=pt-br).

### Tela de detalhes
A partir do videoId retornado na outra chamada, deve ser feito uma chamada para https://www.googleapis.com/youtube/v3/videos?id={VIDEO_ID}&part=snippet,statistics&key={API_KEY}

A partir desse retorno, deve-se montar uma tela contendo embed do video, título, descrição e visualizações.

Essa tela deve ter um botão para voltar para resultados da busca.

## O que será avaliado?
- Organização do projeto
- Lógica do código
- Design das páginas
