# 🚗 Sistema de Gestão e Controle de Estacionamento

> **Status do Projeto:** Planejamento e Iniciação 🏗️  
> [cite_start]**Data de Entrega Prevista:** 23 de março de 2026 [cite: 37]

## 📝 Visão Geral
[cite_start]Este projeto consiste em uma solução de software integrada para a automação e controle total de operações de estacionamento de grande porte[cite: 45]. [cite_start]O sistema visa substituir processos manuais (papel e planilhas) por uma operação tecnológica que inclui **totens de self check-in**, controle de vagas em tempo real e gestão financeira automatizada[cite: 45, 52].

[cite_start]A solução é desenhada para **alta disponibilidade**, sendo capaz de operar **offline** temporariamente, garantindo que o fluxo de veículos não pare mesmo em caso de falhas de conectividade[cite: 48, 89].

---

## 🚀 Principais Funcionalidades

### **Operacional**
* [cite_start]**Check-in Inteligente:** Registro de entradas via ticket físico ou autenticação digital (QR Code/Placa)[cite: 46, 83].
* [cite_start]**Gestão de Vagas:** Controle em tempo real das 5.000 vagas disponíveis[cite: 12, 61].
* [cite_start]**Setorização Digital:** Divisão do pátio em setores (Ex: Setor A, Setor B) para facilitar a localização pelos manobristas[cite: 28, 65].
* [cite_start]**Sugestão de Vaga:** O sistema indica ao manobrista o setor mais vazio para otimizar o fluxo[cite: 66, 67].

### **Financeiro e Administrativo**
* [cite_start]**Cálculo Automático:** Cobrança baseada no tempo de permanência, diferenciando clientes avulsos de mensalistas[cite: 30, 68].
* [cite_start]**Regras de Negócio:** Suporte a períodos de tolerância (ex: 15 min grátis) e cobrança por frações de hora[cite: 31, 70, 85].
* [cite_start]**Dashboards Gerenciais:** Painéis visuais para acompanhar picos de fluxo e taxa de ocupação em tempo real[cite: 33, 71].
* [cite_start]**Relatórios:** Extração de dados consolidados de faturamento diário, semanal e mensal[cite: 34, 73].

---

## 🛠️ Especificações Técnicas

* [cite_start]**Linguagem:** Java[cite: 91, 148].
* [cite_start]**Arquitetura:** Orientada a Objetos (POO) fundamentada em *Clean Code*[cite: 91, 148].
* [cite_start]**Banco de Dados:** SQL Server[cite: 148].
* [cite_start]**Modelagem:** Utilização de diagramas UML[cite: 93, 148].
* [cite_start]**Segurança:** Comunicação protegida por Firewall físico e lógico[cite: 48, 87].
* [cite_start]**Performance:** Capacidade para até 5.000 transações por segundo com tempo de resposta inferior a 5 segundos[cite: 75, 149].

---

## 📊 Qualidade do Software (Modelo FURPS)
[cite_start]O projeto é validado sob as cinco dimensões de qualidade[cite: 134, 153]:
1.  [cite_start]**F (Functionality):** Atendimento total aos requisitos de negócio e regras de cálculo[cite: 154].
2.  [cite_start]**U (Usability):** Interface intuitiva para clientes (totem) e operadores[cite: 76, 156].
3.  [cite_start]**R (Reliability):** Logs de auditoria para cada alteração de dado e operação offline segura[cite: 80, 100, 158].
4.  [cite_start]**P (Performance):** Respostas rápidas e alta fluidez sob carga[cite: 160].
5.  [cite_start]**S (Supportability):** Documentação UML e código estruturado para fácil manutenção[cite: 161, 162].

---

## 💰 Estrutura de Custos Estimada
O investimento total é de **R$ 166.000,00**, distribuído da seguinte forma:

| Categoria | Descrição | Total |
| :--- | :--- | :--- |
| **Recursos Humanos** | [cite_start]Gerente, Analista, Engenheiro e Desenvolvedores [cite: 111, 112] | R$ 97.000,00 |
| **Software** | [cite_start]Licenças de SGBD, SO e Firewall [cite: 113] | R$ 21.000,00 |
| **Infraestrutura** | [cite_start]Servidores, Totens, Câmeras LPR e Rede [cite: 114, 115] | R$ 48.000,00 |

---

## 👥 Equipe (Time Impactados)
* [cite_start]**Cauê** (RA: 2501106) [cite: 39]
* [cite_start]**Pedro Fusco** (RA: 2401933) [cite: 39]
* [cite_start]**Pedro Luiz** (RA: 2501585) [cite: 39]

---

## ⚠️ Riscos e Mitigação
* **Sincronização Offline:** Risco de conflito de dados. [cite_start]*Mitigação:* Implementação de rotinas de validação (*checksum*)[cite: 100, 103].
* **Falha de Hardware:** Atolamento de papel ou erro em leitores ópticos. [cite_start]*Mitigação:* Manutenção preventiva e liberação manual pelo sistema[cite: 104, 108].
