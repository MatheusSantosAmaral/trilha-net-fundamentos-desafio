# Sistema de Estacionamento

Este projeto foi desenvolvido como parte do desafio de projeto da trilha .NET da DIO. O sistema permite gerenciar veículos estacionados, permitindo adicionar, remover e listar veículos, além de calcular o valor a ser cobrado pelo tempo que o veículo ficou estacionado.

## Funcionalidades

O sistema possui as seguintes funcionalidades:

1. **Cadastrar veículo**: Permite que o usuário adicione a placa de um veículo ao estacionamento.
2. **Remover veículo**: Permite que o usuário remova um veículo, calculando o valor a ser cobrado com base no tempo que o veículo permaneceu estacionado.
3. **Listar veículos**: Exibe todos os veículos atualmente estacionados. Se não houver veículos, uma mensagem apropriada será exibida.
4. **Encerrar**: Finaliza o programa.

## Estrutura do Projeto

O projeto é estruturado em uma classe principal chamada `Estacionamento`, que contém as seguintes variáveis e métodos:

### Variáveis

- **precoInicial**: Tipo `decimal`. Representa o preço cobrado para deixar o veículo estacionado.
- **precoPorHora**: Tipo `decimal`. Representa o preço cobrado por hora que o veículo permanece estacionado.
- **veiculos**: Lista de `string`, representando as placas dos veículos estacionados.

### Métodos

- **AdicionarVeiculo(string placa)**: Adiciona um veículo à lista de veículos estacionados.
- **RemoverVeiculo(string placa)**: Remove um veículo da lista, solicita ao usuário a quantidade de horas que ele permaneceu e calcula o valor a ser cobrado.
- **ListarVeiculos()**: Lista todos os veículos estacionados. Se não houver veículos, exibe uma mensagem informando que não há veículos estacionados.

## Uso

Para utilizar o sistema, siga os passos abaixo:

1. Compile o projeto.
2. Execute o programa.
3. Escolha uma das opções do menu interativo:
   - Cadastrar veículo
   - Remover veículo
   - Listar veículos
   - Encerrar

## Exemplo de Uso

```plaintext
Menu:
1. Cadastrar veículo
2. Remover veículo
3. Listar veículos
4. Encerrar

Escolha uma opção: 1
Digite a placa do veículo: ABC1234
Veículo cadastrado com sucesso!

Escolha uma opção: 3
Veículos estacionados:
1. ABC1234

Escolha uma opção: 2
Digite a placa do veículo: ABC1234
Quantas horas o veículo permaneceu estacionado? 2
Valor a ser pago: R$ 20,00

Escolha uma opção: 4
Encerrando o sistema...