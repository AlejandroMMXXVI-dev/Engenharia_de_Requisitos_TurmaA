 <div align="center">
  <h1>Atividade Prática - Engenharia de Requisitos</h1>
  <p><b>Disciplina:</b> Engenharia de Requisitos | <b>Tema:</b> Análise e Modelagem de Processos de Negócio</p>
  <p><b>Projeto:</b> Clínica Vida + Saúde - Sistema de Agendamento de Consultas Médicas</p>
</div>

---

## 📑 Sumário

- [Identificação do Grupo](#-identificação-do-grupo)
- [Análise do Problema](#-análise-do-problema)
- [Stakeholders](#-stakeholders)
- [Processo Atual — AS-IS](#-processo-atual--as-is)
- [Problemas e Melhorias](#-problemas-e-melhorias)
- [Processo Futuro — TO-BE](#-processo-futuro--to-be)
- [Regras de Negócio](#-regras-de-negócio)
- [Requisitos Funcionais](#-requisitos-funcionais)
- [Requisitos Não Funcionais](#-requisitos-não-funcionais)
- [Qualidade do Sistema — ISO/IEC 25010](#-qualidade-do-sistema--isoiec-25010)
- [Restrições](#-restrições)
- [Indicadores de Desempenho](#-indicadores-de-desempenho)
- [Priorização dos Requisitos](#-priorização-dos-requisitos)
- [Justificativa Técnica](#-justificativa-técnica)
- [Reflexão Final do Grupo](#-reflexão-final-do-grupo)
- [Referências](#-referências)

---

## 👥 Identificação do Grupo

| Informação | Preenchimento |
| :--- | :--- |
| **Turma** | Turma A |
| **Nome do Projeto** | Clínica Vida + Saúde |
| **Integrante 1** | Augusto Alejandro de M. Alves |
| **Integrante 2** | Elton Eduardo Viana Lopes |
| **Integrante 3** | Daniel Oliveira Dias |
| **Integrante 4** | Danilo Andrade da Silva |
| **Integrante 5** | Gabriel Marciano de Melo Alves |
| **Integrante 6** | Rafael Cardoso de Barros |

---

## 🎯 Análise do Problema

> **Cenário:** A Clínica Vida + Saúde enfrenta dificuldades no gerenciamento de consultas médicas devido ao processo de agendamento manual, realizado por telefone, atendimento presencial, mensagens via WhatsApp e planilhas eletrônicas.

O principal problema está na incompatibilidade de horários, demora no atendimento e formação de filas de espera, ocasionando falhas de comunicação e um alto índice de faltas dos pacientes.

**Objetivo da solução:** Desenvolver um sistema de agendamento de consultas médicas que permita organizar as agendas, facilitar o acesso dos pacientes aos horários disponíveis, automatizar notificações e melhorar o gerenciamento dos atendimentos.

**Resultados esperados:**

- Reduzir o tempo de espera para agendamentos.
- Diminuir o índice de faltas por meio de lembretes automáticos.
- Evitar conflitos e duplicidade de horários.
- Melhorar a organização das agendas médicas.
- Proporcionar mais autonomia aos pacientes.

---

## 👥 Stakeholders

Os stakeholders são as pessoas ou grupos que possuem interesse ou são afetados pelo funcionamento do sistema.

| ID | Stakeholder | Papel | Necessidade / Interesse |
| :--- | :--- | :--- | :--- |
| ST01 | Paciente | Usuário final | Agendar, remarcar e cancelar consultas online. |
| ST02 | Recepcionista | Operador | Visualizar e ajustar os horários dos médicos. |
| ST03 | Médico | Prestador de serviço | Consultar a agenda diária atualizada. |
| ST04 | Administrador | Gestor | Acompanhar métricas de atendimento e faltas. |
| ST05 | Equipe de TI | Suporte | Garantir segurança e disponibilidade do sistema. |

**Stakeholder principal: Paciente (ST01)**

O paciente é o principal usuário do sistema, pois participa diretamente do processo de agendamento. A solução precisa oferecer um fluxo acessível, intuitivo e ágil, reduzindo a dependência de ligações telefônicas e atendimentos presenciais.

---

## 🔄 Processo Atual — AS-IS

O processo AS-IS representa a maneira como os agendamentos são realizados atualmente, antes da implementação de melhorias.

**Etapas do processo atual:**

1. O paciente entra em contato com a clínica por telefone, WhatsApp ou presencialmente.
2. A recepcionista recebe a solicitação de agendamento.
3. A recepcionista consulta manualmente as agendas dos médicos.
4. O paciente informa sua disponibilidade e preferência de horário.
5. A recepcionista registra a consulta em uma planilha ou agenda de papel.
6. A confirmação é realizada manualmente por telefone ou mensagem.
7. O paciente comparece à clínica no dia agendado.

**Representação simplificada do processo:**

```text
[Paciente solicita consulta]
             |
             v
[Contato por telefone, WhatsApp
 ou atendimento presencial]
             |
             v
[Recepcionista consulta agenda]
             |
             v
[Verificação manual de horários]
             |
             v
[Registro em planilha ou papel]
             |
             v
[Confirmação manual]
             |
             v
[Paciente comparece à consulta]
```

**Características do processo atual:**

- Dependência do atendimento humano.
- Informações distribuídas em diferentes meios.
- Ausência de lembretes automáticos estruturados.
- Possibilidade de duplicidade nos agendamentos.
- Dificuldade para acompanhar cancelamentos e faltas.

---

## ⚠️ Problemas e Melhorias

| Problema identificado | Melhoria proposta |
| :--- | :--- |
| Alto índice de absenteísmo. | Envio automático de lembretes antes das consultas. |
| Conflitos de horários e duplicidade. | Verificação automática da disponibilidade dos médicos. |
| Linhas telefônicas ocupadas. | Disponibilização de agendamento online. |
| Filas na recepção. | Cadastro e gerenciamento de pacientes pela plataforma. |
| Falta de atualização das agendas. | Centralização das informações em um único sistema. |
| Dificuldade para acompanhar resultados. | Geração de relatórios administrativos. |

---

## 🚀 Processo Futuro — TO-BE

O processo TO-BE representa o funcionamento esperado após a implantação do sistema de agendamento.

**Etapas do processo futuro:**

1. O paciente acessa a plataforma.
2. Realiza seu cadastro ou entra com seus dados de acesso.
3. Consulta as especialidades, médicos e horários disponíveis.
4. Seleciona o horário desejado.
5. O sistema verifica automaticamente a disponibilidade.
6. O agendamento é registrado e confirmado.
7. O paciente recebe uma notificação por e-mail ou WhatsApp.
8. O médico consulta sua agenda atualizada.
9. O administrador acompanha os indicadores e relatórios.

**Representação simplificada do processo:**

```text
[Paciente acessa o sistema]
             |
             v
[Realiza cadastro ou login]
             |
             v
[Consulta médicos e horários]
             |
             v
[Seleciona data e horário]
             |
             v
[Sistema verifica disponibilidade]
             |
       +-----+-----+
       |           |
       v           v
 [Disponível]  [Indisponível]
       |           |
       v           v
 [Confirmação] [Escolher outro
       |          horário]
       v
[Registro da consulta]
       |
       v
[Envio de notificação]
       |
       v
[Atualização da agenda médica]
       |
       v
[Consulta e acompanhamento]
```

**Benefícios esperados:**

- Maior autonomia para os pacientes.
- Redução do trabalho manual da recepção.
- Melhor controle das agendas médicas.
- Diminuição de erros de agendamento.
- Acompanhamento dos resultados por indicadores.

---

## 📜 Regras de Negócio

As regras de negócio estabelecem condições que devem ser respeitadas durante o funcionamento do sistema.

| ID | Regra de Negócio |
| :--- | :--- |
| RN01 | Um paciente não pode agendar duas consultas com horários coincidentes na mesma clínica. |
| RN02 | O cancelamento sem cobrança de taxa de retenção deve ser realizado com antecedência mínima de 24 horas. |
| RN03 | Apenas pacientes com cadastro ativo e dados de contato válidos podem realizar agendamentos online. |

---

## ⚙️ Requisitos Funcionais

Os requisitos funcionais representam as funcionalidades que o sistema deve oferecer aos usuários.

| ID | Descrição do Requisito | Stakeholder | Prioridade |
| :--- | :--- | :--- | :--- |
| RF01 | O sistema deve permitir que o paciente cadastre e atualize seus dados pessoais. | Paciente | Alta |
| RF02 | O sistema deve permitir a consulta de horários disponíveis por médico e especialidade. | Paciente | Alta |
| RF03 | O sistema deve permitir que o paciente realize o agendamento de consultas. | Paciente | Alta |
| RF04 | O sistema deve permitir que o médico consulte os dados necessários do paciente e realize o atendimento agendado. | Médico | Alta |
| RF05 | O sistema deve enviar notificações por e-mail ou WhatsApp com lembretes das consultas. | Paciente | Média |
| RF06 | O sistema deve verificar automaticamente a disponibilidade de horários antes de confirmar um agendamento. | Médico / Paciente | Alta |
| RF07 | O sistema deve permitir que a recepcionista bloqueie horários na agenda dos médicos. | Recepcionista | Média |
| RF08 | O sistema deve gerar relatórios com o quantitativo de consultas e faltas por período. | Administrador | Baixa |

---

## 🛡️ Requisitos Não Funcionais

Os requisitos não funcionais definem características de qualidade e condições de funcionamento que o sistema deve apresentar.

| ID | Característica | Descrição do Requisito |
| :--- | :--- | :--- |
| RQ01 | Desempenho | O sistema deve exibir os horários disponíveis em no máximo 2 segundos para 95% das requisições. |
| RQ02 | Segurança | O sistema deve armazenar senhas utilizando algoritmo hash BCrypt e transmitir dados por HTTPS/TLS. |
| RQ03 | Usabilidade | O sistema deve permitir que o agendamento seja concluído em no máximo 4 cliques a partir da tela inicial. |
| RQ04 | Confiabilidade | O sistema deve apresentar disponibilidade mínima de 99% durante o horário comercial. |
| RQ05 | Compatibilidade | O sistema deve ser responsivo e compatível com Chrome, Edge e Safari, em dispositivos desktop e mobile. |

---

## 🛡️ Qualidade do Sistema — ISO/IEC 25010

A qualidade de um software não depende apenas de suas funcionalidades, mas também de aspectos como desempenho, segurança, confiabilidade e facilidade de utilização.

Para orientar a definição dos requisitos de qualidade da Clínica Vida + Saúde, utilizamos como referência o modelo **ISO/IEC 25010:2023**, que apresenta características para avaliar a qualidade de produtos de software.

A documentação utilizada como base foi disponibilizada no repositório [Sistema de Gestão de Projetos Ágil — ISO/IEC 25010](https://github.com/gabrielmarciano-dev/sistema-de-gestao-de-projetos-agil/blob/main/Documentacao/ISO_IEC%2025010.md).

### 📋 Aplicação ao Projeto

| Característica de qualidade | Aplicação na Clínica Vida + Saúde |
| :--- | :--- |
| **Eficiência de desempenho** | Consultar horários disponíveis em até 2 segundos para 95% das requisições. |
| **Segurança** | Proteger os dados dos pacientes e restringir o acesso a usuários autorizados. |
| **Capacidade de interação** | Permitir que o paciente conclua um agendamento em no máximo 4 cliques, a partir da tela inicial. |
| **Confiabilidade** | Manter disponibilidade mínima de 99% durante o horário comercial. |
| **Flexibilidade e compatibilidade** | Oferecer uma interface responsiva e compatibilidade com os navegadores previstos para uso em computadores e dispositivos móveis. |

### 🎯 Importância para o Projeto

A aplicação dessas características ajuda a transformar necessidades gerais, como ter um sistema rápido e seguro, em requisitos que podem ser testados e avaliados.

No contexto da clínica, isso contribui para proteger as informações dos pacientes, reduzir dificuldades durante os agendamentos e manter o sistema disponível para os usuários.

**Fonte de apoio:** [Documentação sobre a ISO/IEC 25010:2023 — GitHub](https://github.com/gabrielmarciano-dev/sistema-de-gestao-de-projetos-agil/blob/main/Documentacao/ISO_IEC%2025010.md).

---

## 📌 Restrições

As restrições representam limitações tecnológicas, legais e de prazo que devem ser consideradas no desenvolvimento.

| ID | Restrição | Categoria |
| :--- | :--- | :--- |
| RES01 | O sistema deve ser desenvolvido utilizando tecnologias de código aberto (Open Source). | Tecnologia |
| RES02 | O sistema deve ser finalizado e entregue para testes dentro do prazo estabelecido no cronograma. | Prazo |
| RES03 | O tratamento e armazenamento dos dados pessoais e de saúde devem estar em conformidade com a LGPD. | Legal |

---

## 📊 Indicadores de Desempenho

Os indicadores permitem acompanhar se as melhorias propostas estão produzindo os resultados esperados.

| ID | Indicador | Objetivo |
| :--- | :--- | :--- |
| IND01 | Tempo médio de agendamento | Acompanhar o tempo necessário para concluir um agendamento. |
| IND02 | Taxa de absenteísmo | Monitorar a quantidade de pacientes que não comparecem às consultas. |
| IND03 | Taxa de conflitos de agendamento | Identificar ocorrências de duplicidade ou sobreposição de horários. |
| IND04 | Quantidade de consultas agendadas | Acompanhar o volume de agendamentos realizados. |
| IND05 | Taxa de cancelamentos | Monitorar a quantidade de consultas canceladas em determinado período. |
| IND06 | Disponibilidade do sistema | Acompanhar o percentual de tempo em que o sistema permanece disponível. |

**Exemplo de acompanhamento:**

- **Tempo de agendamento:** objetivo de concluir uma marcação em menos de 2 minutos.
- **Taxa de absenteísmo:** acompanhar a redução das faltas após a implantação dos lembretes.
- **Conflitos de agendamento:** buscar eliminar as duplicidades por meio da verificação automática de disponibilidade.

---

## ⭐ Priorização dos Requisitos

A priorização define quais funcionalidades devem receber maior atenção durante o desenvolvimento, considerando sua importância para os usuários e para o funcionamento do sistema.

| Prioridade | Requisitos | Justificativa |
| :--- | :--- | :--- |
| **Alta — Must Have** | RF01, RF02, RF03, RF04, RF06, RQ01, RQ02, RQ03, RQ04 e RQ05 | São essenciais para o funcionamento, segurança e utilização do sistema. |
| **Média — Should Have** | RF05 e RF07 | Melhoram a comunicação com os pacientes e o gerenciamento das agendas. |
| **Baixa — Could Have** | RF08 | Complementa a gestão administrativa por meio de relatórios e estatísticas. |

**Critério utilizado:** Os requisitos de alta prioridade representam as funcionalidades e características essenciais para que o sistema consiga cumprir seu objetivo principal. Os de média prioridade agregam melhorias operacionais, enquanto os de baixa prioridade complementam a solução.

---

## 🧠 Justificativa Técnica

> **Por que a análise do processo de negócio é essencial?**
>
> A análise do processo de negócio permite compreender como as atividades são realizadas atualmente, identificar dificuldades e reconhecer as necessidades dos envolvidos.
>
> Por meio da modelagem AS-IS, foi possível observar problemas como demora nos agendamentos, falhas de comunicação e conflitos de horários. A partir dessas informações, a proposta TO-BE apresenta melhorias que orientam o levantamento e a especificação dos requisitos do sistema.
>
> Dessa forma, a Engenharia de Requisitos contribui para que a solução desenvolvida esteja alinhada às necessidades dos stakeholders, evitando funcionalidades desnecessárias e reduzindo possíveis falhas durante o desenvolvimento.

---

## 💭 Reflexão Final do Grupo

**1. Qual requisito gerou mais discussão durante o levantamento e por quê?**

O requisito RF05, referente ao envio de notificações automáticas por WhatsApp ou e-mail. A equipe discutiu se essa funcionalidade deveria ser indispensável na primeira versão ou considerada secundária, levando em consideração os custos de integração e a infraestrutura necessária.

**2. Qual necessidade do usuário inicialmente parecia simples, mas gerou vários requisitos?**

A necessidade do paciente de agendar uma consulta. Essa atividade envolve diversas funcionalidades, como cadastro de dados pessoais, consulta de médicos e especialidades, verificação de horários disponíveis e aplicação de regras para evitar sobreposições.

**3. O grupo identificou algum requisito implícito que somente apareceu durante a discussão? Qual?**

Sim. A possibilidade de a recepcionista bloquear manualmente horários na agenda dos médicos (RF07). Essa funcionalidade demonstrou ser importante para lidar com emergências e ausências médicas não planejadas.

---

## 📚 Referências

- GABRIELMARCIANO-DEV. **Sistema de Gestão de Projetos Ágil: Documentação ISO/IEC 25010**. GitHub. Disponível em: [Documentação ISO/IEC 25010](https://github.com/gabrielmarciano-dev/sistema-de-gestao-de-projetos-agil/blob/main/Documentacao/ISO_IEC%2025010.md). Acesso em: 11 nov. 2026.

- INTERNATIONAL ORGANIZATION FOR STANDARDIZATION. **ISO/IEC 25010:2023 — Systems and software engineering — Systems and software Quality Requirements and Evaluation (SQuaRE) — Product quality model**. 2. ed. Genebra: ISO, 2023. Disponível em: [ISO](https://www.iso.org/standard/78176.html).

---

<div align="center">
  <sub>Augusto Alejandro e equipe • 2026</sub>
  <p><sub>Engenharia de Requisitos — Clínica Vida + Saúde</sub></p>
</div>
