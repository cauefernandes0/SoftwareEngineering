# Sistema de Gestão e Controle de Estacionamento

**Link do Repositório:** https://github.com/cauefernandes0/SoftwareEngineering#

## Descrição do Projeto
O produto consiste em uma solução de software integrada projetada para a gestão e controle de operações de um estacionamento de alta capacidade (5.000 vagas) e operação de totens de *self check-in*. O sistema visa automatizar o espaço, substituindo processos manuais realizados em papel ou planilhas Excel, o que reduz a margem de erro humano, inconsistências de dados e otimiza o tempo de operação, sanando falhas de segurança no controle de acesso de veículos.

## Funcionalidades Principais
* **Controle de Acessos e Vagas:** O sistema gerencia as vagas disponíveis e ocupadas, registrando o horário de entrada e saída de veículos.
* **Setorização Digital:** O sistema divide o estacionamento em setores (ex: Setor A - Azul) e sugere ao manobrista a melhor vaga/setor para estacionar no momento do *check-in*, vinculando o carro à vaga exata para facilitar a saída.
* **Validação Digital e Física:** O *check-in* do veículo gera a emissão de um ticket físico ou a autenticação por cadastramento digital, como QR Code ou leitura de placa (câmera LPR).
* **Gestão de Tarifas e Cobranças:** Cálculo automático no *checkout* baseado na hora exata do *check-in*, diferindo clientes avulsos de mensalistas, cobrando por fração de hora e garantindo isenção de tarifa para saídas em até 15 minutos.
* **Painel Gerencial:** Criação de painéis visuais para o gerente acompanhar o fluxo em tempo real, picos de entrada/saída, taxa de ocupação, além de extrair relatórios consolidados de faturamento diário, semanal e mensal.
* **Auditoria (Logs):** Cada movimento de inclusão, alteração e exclusão de dados é registrado em um log, identificando quem fez (ID do usuário/operador), a data, a hora e o que foi editado.

## Tecnologias e Arquitetura
A base estrutural e os requisitos técnicos foram definidos visando o equilíbrio com base nas dimensões do modelo FURPS (Funcionalidade, Usabilidade, Confiabilidade, Desempenho e Suportabilidade):
* **Linguagem e Banco de Dados:** O desenvolvimento é feito em Java e o banco de dados utilizado é o SQL Server.
* **Paradigmas e Modelagem:** A arquitetura de software é Orientada a Objetos, com o desenvolvimento baseado em *Clean Code* e a modelagem feita com UML.
* **Performance e Escalabilidade:** A infraestrutura permite picos de até 5.000 transações por segundo e garante um tempo de resposta de no máximo 5 segundos nas consultas.
* **Confiabilidade e Operação Offline:** O totem de entrada/saída possui a capacidade de operar temporariamente *offline* e sincronizar os dados posteriormente com o servidor principal, com rotinas robustas de validação.
* **Segurança de Rede:** Toda a comunicação do sistema instalado nos dispositivos externos (totens e mobile) com o banco de dados e a internet passa obrigatoriamente por um Firewall físico.

## Equipe e Autores
Projeto planejado e desenvolvido pela equipe "Time Impactados":
* **Cauê** - 2501106
* **Pedro Fusco** - 2401933
* **Pedro Luiz** - 2501585
