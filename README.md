# Interfaces

Foi criado um programa para a leitura de dados referente ao aluguel de automoveis, sendo feita a criação de classes de entidades e serviços.
Na primeira o problema foi resolvido sem a utilização de uma interface, o que acaba gerando uma complicação para a manutenção do aplicativo,
pois seria necessário realizar várias alterações em caso de mudança nas regras do negocio.

Foi então criada a interface de TaxService, implementando a classe BrazilTaxService, fazendo com que fosse necessária apenas uma alteração no programa
em caso de mudança nas regras do negocio.
EX: Caso a taxa a ser cobrada pelo programa seja mudada do Brasil para a taxa do Canada, seria necessário apenas alterar no programa a instanciação de
"new BrazilTaxService" para por exemplo "new CanadaTaxService".
