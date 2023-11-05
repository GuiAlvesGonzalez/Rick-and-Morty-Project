# Rick-and-Morty-Project
*Utilizei o Visual Studio Code para criar meu codigo, e usei a ferramenta Live Server para deixar meu codigo on-line, para fazer o site funcionar, basta copiar e colar a pasta index.html e a character.html, o nome da segunda pasta está sendo usado dentro do código, portanto
não deve ser alterado, dito isso agora basta da um "go live" na pasta index.html que o código ira funcionar! Para utilizar o site, você pode pesquisar o nome de um personagem em especifico ou clicar na lupa que ela trará alguns personagems padrôes para você, e ao clicar na
imagem ou no nome do personagem, você será redirecionado para outra página com as informações do personagem.

Meu código funciona em duas páginas:

A primeira página:
/* Na Head comecei por definir od requisitos padrões em todo HTML<!DOCTYPE html> e as fontes que eu iria usar no meu código utilizei também o <style> para dar o design aos componentes do meu código exemplo (background-image:) e as fontes de cada texto aparente (font-family:) */
/* No Body comecei por criar meu título(h1) e criar o meu botão e barra de pesquisa. Defini suas classes e adicionei o manipulador de eventos como "submit", quando algo é escrito e enviado, o manipulador é chamado e em seguida ele obtem o valor do que foi escrito no campo
de pesquisa (var searchInput), utilizando o (var searchURL) que está apontado para a API do Rick and Morty ele cria uma URL usando o que foi escrito no campo de pesquisa.
Usei a função fetch para fazer a solicitação (GET) para a URL de pesquisa, o fetch retorna uma promise que quando concluída retorna a solicitção em forma JSON, após a promessa ser resolvida (.then) o JSON é convertido em um elemento JavaScript que contem um array de elementos
de cada personagem da série, utlizei a função data.results.forEach para reiterar sobre os objetos do JSON e criar uma lista pelo ID de cada personagem contendo a imagem e o nome deles, esta lista é colocada junto do ID result (que foi definido antes do script, <div id="result"></div>
exibindo os resultados da pesquisa na página (character ID, image, name) que no caso o "result" está apontado para a minha segunda página com um código semelhante porém como mais resultados além dos exibidos nesta primeira página (type, status, origin, location e species)./*

A segunda página:
/* A segunda página é basicamente uma cópia da primeira, na questão do fetch, apesar das outras informações que serão exibidas a mais que o fetch da primeira página, entretanto criei o objeto URLSearchParams a partir da string queryString para pegar o valor dos objetos (id do personagem)
e ela constroi a URL que mostra o personagem em especifico que foi clicado na primeira página do códgio.*/
