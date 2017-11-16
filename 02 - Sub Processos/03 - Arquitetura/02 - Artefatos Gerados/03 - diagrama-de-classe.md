## Especificação do Diagrama de Classe

### Introdução
Este diagrama tem como objetivo especificar as principais modelos de dados da aplicação, além de estruturar o relacionamento das classes que compõem o corpo da aplicação.

* Persistence model: É a classe principal do projeto. Ela armazena o id da aplicação, a data do registro do usuário e a data da última atualização, além dos métodos referentes ao registro e à atualização.
* Usuário: É uma especialização da classe Persistence Model e tem o objetivo de armazenar os dados de nome e senha dos usuários.
* Passageiro: 
É um especialização da classe usuário, com objetivo de armazenar dados específicos do usuário do sistema que se enquadra na categoria de passageiro. Tem como atributo obrigatório e único o CPF, utilizado para identificar a identidade física do passageiro. Os demais dados provém de suas superclasses.
* Motorista: 
É um especialização da classe usuário, com objetivo de armazenar dados específicos do usuário do sistema que se enquadra na categoria de motorista. Tem como atributos o CNPJ do usuário, seu veículo de trabalho e seus itinerários.  Os demais dados provém de suas superclasses.
* Itinerário: 
É uma especialização da classe Persistence Model e tem o objetivo de armazenar os dados dos itinerários percorridos pelo motorista em suas viagens.
* Veículo: 
É uma especialização da classe Persistence Model e tem o objetivo de armazenar os dados de modelo,  cor e placa do veículo utilizado pelo motorista (usuário do sistema) para o percurso dos itinerários.
