# DIO - Trilha .NET - Explorando a linguagem C#

## 🐱‍👤 Desafio de projeto
Para este desafio, você precisará usar seus conhecimentos adquiridos no módulo de explorando a linguagem C#, da trilha .NET da DIO.

## 📖 Contexto
Você foi contratado para construir um sistema de hospedagem, que será usado para realizar uma reserva em um hotel. Você precisará usar a classe Pessoa, que representa o hóspede, a classe Suíte, e a classe Reserva, que fará um relacionamento entre ambos.

O seu programa deverá cálcular corretamente os valores dos métodos da classe Reserva, que precisará trazer a quantidade de hóspedes e o valor da diária, concedendo um desconto de 10% para caso a reserva seja para um período maior que 10 dias.

## 📄 Regras e validações
1. Não deve ser possível realizar uma reserva de uma suíte com capacidade menor do que a quantidade de hóspedes. Exemplo: Se é uma suíte capaz de hospedar 2 pessoas, então ao passar 3 hóspedes deverá retornar uma exception.
2. O método ObterQuantidadeHospedes da classe Reserva deverá retornar a quantidade total de hóspedes, enquanto que o método CalcularValorDiaria deverá retornar o valor da diária (Dias reservados x valor da diária).
3. Caso seja feita uma reserva igual ou maior que 10 dias, deverá ser concedido um desconto de 10% no valor da diária.


![Diagrama de classe estacionamento](diagrama_classe_hotel.png)

## 🎯 Solução
Para obter um programa funcional, foi cumprida a missão de continuar o código fornecido incompleto, baseando-se nos requisitos descritos acima. Com o objetivo de aplicar os conhecimentos adquiridos no `Bootcamp Coding The Future Avanade - .NET Developer`, o código foi reformulado e desenvolvido com o objetivo de fornecer um Sistema de Hospedagem em Hotel utizando .NET.

## 📄 Funcionalidades
- Cadastrar hóspedes
- Cadastrar suíte
- Obter quantidade de hóspedes
- Calcular valor da hospedagem

## 📖 Especificações Técnicas
A solução é composta por 4 (quatro) classes:
- *Pessoa.cs:* é uma representação de uma pessoa em um sistema de gerenciamento de hospedagem. Ela oferece três construtores distintos para inicializar objetos Pessoa, permitindo a definição do nome e/ou sobrenome da pessoa de maneiras variadas. A classe possui propriedades públicas para armazenar o nome e sobrenome da pessoa, e uma propriedade de leitura NomeCompleto que retorna o nome completo da pessoa em letras maiúsculas, derivado da concatenação do nome e sobrenome.

- *Suite.cs:* é responsável por representar uma suíte em um sistema de gerenciamento de hospedagem. A classe possui dois construtores: um construtor padrão que não recebe argumentos e não executa nenhuma ação, e um construtor que recebe três parâmetros: tipoSuite para definir o tipo da suíte, capacidade para definir a capacidade máxima de pessoas na suíte e valorDiaria para definir o valor da diária da suíte.

- *Reserva.cs:*  é responsável por representar uma reserva de hospedagem em um sistema de gerenciamento. Seus atributos incluem uma lista de hóspedes (Hospedes), uma suíte reservada (Suite) e o número de dias da reserva (DiasReservados). Oferece funcionalidades como cadastrar hóspedes e associá-los à reserva, bem como definir a suíte reservada e calcular o valor total da reserva com base nos dias reservados e no valor da diária da suíte. Além disso, realiza verificações para garantir que o número de hóspedes não exceda a capacidade da suíte e aplica um desconto se a reserva for para 10 dias ou mais. Essa classe encapsula a lógica essencial para o gerenciamento de reservas de hospedagem em um sistema.

- *Program.cs:* é a classe principal do programa. Nela são criadas instâncias de dois objetos Pessoa, representando os hóspedes. Esses objetos são então adicionados a uma lista de hóspedes. Em seguida, é criada uma instância da classe Suite, definindo suas características. Uma instância da classe Reserva é então criada, especificando a quantidade de dias a ser reservada. A suíte e os hóspedes são associados a essa reserva usando métodos específicos da classe Reserva. Por fim, são exibidos no console a quantidade de hóspedes associados à reserva e o valor total da reserva, calculado com base no número de dias reservados e no valor da diária da suíte.

## 👩🏻‍💻 Versões do Projeto
Versão 1.0: versão original desenvolvida pelo professor Leonardo Buta para o Desafio C# e .NET do `Bootcamp Coding The Future Avanade - .NET Developer`.
Versão 1.1: versão desenvolvida por mim para conclusão do projeto para o `Bootcamp Coding The Future Avanade - .NET Developer.

## 💻 Tecnologias Utilizadas
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=csharp&logoColor=white)

![.Net](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white)

![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)

## ⚙ Dependências e Versões Utilizadas
- **[SDK .NET](https://dotnet.microsoft.com/pt-br/download)** - Versão: 8.0.100 ou 8.0.101 (para compilar e executar a aplicação)
- **[Visual Studio Code](https://code.visualstudio.com/download)** - Versão: 1.84.1 (editor de código)
- **[Git](https://git-scm.com/downloads)** - Versão: 2.43.0 (versionamento do código)

## 🕹 Como Executar a Aplicação
1. Instale em sua máquina as dependências acima, nas versões recomendadas.
2. Clone o repositório para a sua máquina local. Você pode utiizar um dos seguintes comandos:
```
git clone https://github.com/BarbaraLeimig/Sistema-Estacionamento-NET-desafio.git
```
ou
```
git clone git@github.com:BarbaraLeimig/Sistema-Estacionamento-NET-desafio.git
```
3. No Visual Studio Code navegue até a pasta do projeto em sua máquina via menu ou pela linha de comando. Ex:
```
cd Desktop/Projetos/Estacionamento
```
4. Faça o download da bibliotca DocsBRValidator pelo terminal:
```
dotnet add package DocsBRValidator
```
5. Execute o seguinte comando para iniciar o programa:
```
dotnet run
```
6. Interaja com o programa seguindo as informações exibidas no console.

