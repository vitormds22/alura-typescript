# CURSO TYPESCRIPT ALURA

* Nesse curso vamos aprender a como utlizar o Typescript nos nossos projetos.
* Para utilizar esse projeto é necessário antes rodar o comando: npm i && npm run server

## O que aprendi nesse curso?

### Aula 01/02
* Instalamos a biblioteca do TypeScript no projeto
* Revisamos a forma estrutural do JS.
* O básico da configuração do TSCONFIG para que a compilação dos arquivos TS sejam feitas corretamente.
* Aprendi a configurar o arquivo package.json para ouvir/observar alterações nos arquivos TS e compilar automaticamente com a diretiva "watch":tsc -w
* O benefício do modificador private assim como em outras linguagens

##

### Aula 03
* Depois de um entendimento geral começamos a construção do aplicativo
* Usamos o conceito de controller para controlar os dados do formulário e criar o modelo
* Aprendemos a utilizar o modificador private para deixar os atributos da classe controller visiveis somente para a classe
* Usamos o conceito de POO para instanciar um objeto da classe NegociacaoController
* Fizemos o envio de dados de um form via addEventListener impedindo o reload da página, que por padrão isso já acontece
* Configuramos o compilador para não aceitar o tipo **any** implicitamente
* Começamos a utilizar as tipagens do typescript na classe de negociação
* O Typescript carrega consigo várias tipagens (number, string, etc) e até mesmo do DOM
* É importante para o Typescript que o valor seja sempre igual ao que foi instanciado na classe, nesse caso realizamos a conversão dos dados do formulário (que sempre vem em string) para seus respectivos tipos
* O Typescript tem a função de tipagens até mesmo em funções, assim como no java, por exemplo. Se não houver retorno é do tipo void, se houver um retorno de string é do tipo string.
* **Evite os tipos any**
* **Tipagem de tudo!!!!**
