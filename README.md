# Sistema Osvaldo Motors

Este repositório contém o projeto desenvolvido para o cliente Osvaldo Motors.

O objetivo do sistema é auxiliar no gerenciamento de reparos de veículos, permitindo registrar informações dos clientes e dos carros, além dos serviços realizados e dos valores cobrados.

O sistema busca facilitar a organização das informações dos reparos e tornar o controle dos serviços da oficina mais simples e eficiente.

## MER — Osvaldo Motors
### 1. Entidades
- Cliente: armazena os dados dos clientes da oficina.
- Serviço: armazena as informações dos serviços realizados nos veículos.

  
### 2. Atributos
- Cliente:
- id_cliente — identificador do cliente (PK).
- nome — nome do cliente.
- telefone — telefone do cliente.
- Serviço:
- id_servico — identificador do serviço (PK).
- id_cliente — identificador do cliente (FK).
- placa — placa do veículo.
- modelo_carro — modelo do veículo.
- servico_realizado — descrição do serviço realizado.
- valor_cobrado — valor cobrado pelo serviço.

  
### 3. Relacionamento
- Um cliente pode realizar vários serviços na oficina.
- Cada serviço está associado a um único cliente.
- A cardinalidade do relacionamento é 1:N (um para muitos).

  
4. Regras de negócio
- Cada cliente possui um identificador único.
- Cada serviço possui um identificador único.
- Todo serviço deve estar vinculado a um cliente cadastrado.
- O sistema deve registrar a placa e o modelo do veículo, o serviço realizado e o valor cobrado.


![Diagrama DER](./der.png)

