# Exercício de Avaliação de POO com Foco em Herança, Polimorfismo e Encapsulamento

## Descrição

Neste exercício, você deve desenvolver um sistema simples em Java para gerenciar informações sobre veículos em uma concessionária. O sistema deve ser capaz de registrar diferentes tipos de veículos (carros e motos), permitindo a adição de novos veículos, a visualização de detalhes específicos e a execução de operações específicas de cada tipo de veículo.

O objetivo deste exercício é demonstrar a aplicação dos conceitos de herança, polimorfismo e encapsulamento na implementação de um sistema de gerenciamento de veículos.

## Cenário

A concessionária "AutoVendas" deseja informatizar o registro dos veículos disponíveis em seu catálogo. Eles precisam de um sistema que permita gerenciar informações sobre diferentes tipos de veículos. Cada tipo de veículo (carros e motos) deve ter características específicas e realizar ações próprias. 

## Requisitos do Exercício

### 1. `Carro`

- **Atributos:**
  - `marca`: Representa a marca do veículo (por exemplo, Honda, Toyota).
  - `modelo`: Representa o modelo do veículo (por exemplo, Civic, CB500).
  - `ano`: Representa o ano de fabricação do veículo.
  - `preco`: Representa o preço do veículo.
  - `numeroDePortas`: Número de portas do carro.
  - `tipoCombustivel`: Tipo de combustível usado pelo carro (por exemplo, gasolina, etanol).

- **Ações:**
  - **Registrar Veículo:** Adicionar um novo veículo ao catálogo da concessionária.
    - *Descrição:* Esta ação deve permitir o registro das informações básicas do veículo, como marca, modelo, ano e preço.
  - **Exibir Detalhes do Veículo:** Exibir as informações detalhadas sobre o veículo.
    - *Descrição:* Esta ação deve permitir a visualização de todas as informações do veículo, encapsulando os detalhes específicos.. Imprimir na tela os atributos do carro.
  - **Calcular Valor de Seguro:** Calcular o valor do seguro para o carro.
    - *Descrição:* Esta ação deve calcular o valor do seguro com base no preço do carro e no tipo de combustível. Se o tipo de combustível do carro é etanol ou flex, o seguro é calculado como sendo 0.1% do preço do veículo. Caso contrário, o seguro é 0.2% do preço do veículo

### 2. `Moto`

- **Atributos:**
  - `marca`: Representa a marca do veículo (por exemplo, Honda, Toyota).
  - `modelo`: Representa o modelo do veículo (por exemplo, Civic, CB500).
  - `ano`: Representa o ano de fabricação do veículo.
  - `preco`: Representa o preço do veículo.
  - `cilindrada`: Cilindrada do motor da moto (por exemplo, 500cc, 1000cc).
  - `tipoTransmissao`: Tipo de transmissão da moto (por exemplo, manual, automática).

- **Ações:**
  - **Registrar Veículo:** Adicionar um novo veículo ao catálogo da concessionária.
    - *Descrição:* Esta ação deve permitir o registro das informações básicas do veículo, como marca, modelo, ano e preço.
  - **Exibir Detalhes do Veículo:** Exibir as informações detalhadas sobre o veículo.
    - *Descrição:* Esta ação deve permitir a visualização de todas as informações do veículo, encapsulando os detalhes específicos. Imprimir na tela os atributos da moto.
  - **Calcular Valor de Seguro:** Calcular o valor do seguro para a moto.
    - *Descrição:* Esta ação deve calcular o valor do seguro com base no preço da moto e na cilindrada do motor. Se a cilindrada do motor é maior que 125, o seguro é calculado como sendo 0.1% do preço do veículo. Caso contrário, o seguro é 0.2% do preço do veículo

### 3. `Concessionaria` (Classe para Gerenciamento)

- **Atributos:**
  - `veiculos`: Lista de veículos disponíveis na concessionária.

- **Ações:**
  - **Adicionar Veículo:** Adicionar um novo veículo (carro ou moto) ao catálogo.
    - *Descrição:* Esta ação deve permitir adicionar um veículo à lista de veículos, utilizando o polimorfismo para lidar com diferentes tipos de veículos.
  - **Listar Veículos:** Exibir uma lista de todos os veículos disponíveis na concessionária.
    - *Descrição:* Esta ação deve exibir todos os veículos cadastrados, utilizando os métodos encapsulados para acessar e exibir as informações.

## Desafios

- Implementar o sistema de forma que as classes derivadas possam sobrescrever os métodos da classe base de maneira polimórfica.
- Garantir que os atributos das classes sejam encapsulados.
- Implementar um mecanismo para listar e detalhar as informações dos veículos registrados na concessionária.

Este exercício deve ser desenvolvido no Eclipse, onde você criará um projeto Java com as classes e métodos descritos. A implementação deve demonstrar a compreensão dos conceitos de herança, polimorfismo e encapsulamento na prática. Compactar a pasta do projeto e enviar para o email **ricardojulio@univas.edu.br**. Adicionar no título **Avaliação de POO - Seu nome completo**. No corpo do email, anexar o arquivo zipado.
