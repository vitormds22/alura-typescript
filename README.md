# CURSO TYPESCRIPT ALURA - Parte 1

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

##
### Aula 04
* Na primeira aula fizemos a criação de um novo modelo para representar as negociações como uma listagem concreta e impedir a modificação posterior ao seu cadastro
* Portanto essa classe irá armazenar uma lista de negociações
* Sabemos que no JS puro um array pode ter vários tipos de conteúdos dentro dele
* Vamos descobrir somente o conteúdo e seus tipos em tempo de compilação
* No Typescript é importante tiparmos o array até mesmo porque tiramos o tipo any implicito do projeto.
* Então vimos que existem os Generic Types, no caso do Array o erro é: Array<T>
* Para isso devemos tipar o array fazendo ele ser apenas de um tipo, evitando problemas futuros.
* Aprendemos a criar métodos que realizam a criação desacoplada de uma Negociação, tranzendo mais robustez ao código
* Evitamos a mutabilidade do nosso Array de Negociações.
* Usamos o spread operator para dividir os itens do Array e assegurar a integridade dos dados
* Usamos o tipo ReadonlyArray para retornar a lista do Array de listagem
* Dessa forma ao operar com o Array desse tipo só aparece e é possível utilizar métodos de visualização


##
### Aula 05
* Nessa aula vamos refatorar para simplificar o código já feito
* Primeiro no construtor, não é necessário declarar os atributos diretamente pelo construtor e sem atribuir o valor dos atributo e dos parâmetros
* Existe uma forma melhor de digitar o Array e Generic Type: Negociacao[] 
* Isso é a mesma coisa que Array<Negociacao>
* Para read only: <readonly Negociacao[]>
* Podemos usar esse modelo também para atributos das classe, retirando o modificador private e retirando os métodos get, reduzindo muito as linhas de código
* Aprendi sobre programação defensiva, com o caso de uso do atributo data que podia ser modificado via método.
* Criando um clone da data para que as modificações em outras classes sejam feitas em uma outra referência

##
