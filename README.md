Pequeno teste para entender como funciona o deploy de uma aplicação ReactJS no GitHub Pages.

1. Criar um projeto React
  -> npx create-react-app Teste.

2. Adicionar a biblioteca do GitHub Pages no projeto.
  -> yarn add -D gh-pages

3. Adicionar as seguintes propriedades no arquivo package.json:
<br/>
  ...
  "homepage": "https://seuNomeNoGitHub.github.io/your-app-name",
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",
  },
  ...
  (Confira no meu package.json o exemplo)
  
4. Execute o comando abaixo no terminal: 
  $ yarn run deploy
  
5. Fim! depois de alguns segundos a sua aplicação já esta no mesmo link
da "homepage"
  
Link do meu teste: https://randelfreitas.github.io/teste/

(Bonus: para aplicações somente com HTML, CSS E JS, basta somente ir em 
-> Configurações (Settings)
-> GitHub Pages
e mudar o branch de none para master.
