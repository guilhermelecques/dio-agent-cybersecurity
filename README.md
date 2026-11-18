# dio-agent-cybersecurity

# DIO Agent — Especialista em Análise de Vulnerabilidades

## 1. Sobre o projeto

Este projeto consiste na evolução do DIO Agent, transformando-o em um agente especializado em análise de vulnerabilidades e segurança de aplicações (AppSec).

O objetivo é fazer com que o agente não apenas identifique falhas de segurança, mas também compreenda o contexto do ambiente, avalie os riscos, explique os possíveis impactos e apresente recomendações para corrigir as vulnerabilidades encontradas.

A especialização foi desenvolvida por meio de arquivos de instruções, conhecimento e habilidades (skills), sem realizar treinamento de um novo modelo de inteligência artificial.

## 2. Especialização desenvolvida

A especialização escolhida foi a análise de vulnerabilidades.

O agente foi orientado para:

- Identificar vulnerabilidades em aplicações e sistemas.
- Analisar possíveis formas de exploração em ambientes autorizados.
- Avaliar impacto, probabilidade e severidade.
- Relacionar vulnerabilidades com referências como OWASP e MITRE ATT&CK, quando aplicável.
- Recomendar medidas de correção.
- Validar se as vulnerabilidades foram mitigadas.

Escolhi essa especialização porque considero a identificação e a correção de vulnerabilidades etapas fundamentais da segurança da informação.

## 3. Arquivos criados e modificados

### Skill — vulnerability-analysis

Foi criada uma nova skill chamada `vulnerability-analysis`, responsável por orientar o agente durante o processo de análise de vulnerabilidades.

Arquivo:
- `skills/vulnerability-analysis/SKILL.md`
- `skills/vulnerability-analysis/README.md`

### Base de conhecimento — security-basics.md

Foi criado um arquivo de conhecimento com conceitos fundamentais de segurança da informação, incluindo:

- Vulnerabilidade, ameaça e risco.
- Tríade CIA: confidencialidade, integridade e disponibilidade.
- Boas práticas de segurança.

Arquivo:
- `agent/knowledge/security-basics.md`

### Persona do agente

O arquivo `agent/persona.md` foi atualizado para orientar o comportamento do agente durante análises de segurança.

Foram adicionadas orientações para que ele seja investigativo, cuidadoso, didático e priorize a segurança antes de recomendar procedimentos.

### AGENTS.md

O arquivo `AGENTS.md` foi atualizado para incluir a nova skill na tabela de habilidades disponíveis e orientar o agente sobre quando utilizá-la.

## 4. Laboratório prático — SQL Injection

Foi desenvolvido um laboratório local em Python para demonstrar uma vulnerabilidade SQL Injection.

Inicialmente, foi criada uma aplicação de login que utilizava concatenação de strings para montar consultas SQL, permitindo uma tentativa de contorno da autenticação.

Em seguida, o DIO Agent foi utilizado para identificar e explicar a vulnerabilidade.

A correção foi realizada utilizando consultas parametrizadas do SQLite, impedindo que os dados fornecidos pelo usuário fossem interpretados como parte do comando SQL.

Por fim, foi realizada uma nova análise para verificar a mitigação da vulnerabilidade.

## 5. Melhoria implementada

Foi implementada uma padronização na análise de vulnerabilidades.

O agente foi orientado a apresentar suas avaliações considerando:

- Vulnerabilidade identificada.
- Ativo afetado.
- Evidências.
- Impacto.
- Probabilidade.
- Severidade.
- Recomendação de correção.
- Validação da correção.

Essa melhoria permite organizar as análises e facilitar a comparação entre diferentes problemas de segurança.

## 6. Tecnologias utilizadas

- Python
- SQLite
- DIO Agent
- Hermes
- Git
- GitHub
- Markdown

## 7. Como executar o projeto

### Pré-requisitos

- Python instalado.
- Git instalado.
- Hermes instalado e configurado.
- Repositório DIO Agent baixado.

### Execução

Clone o repositório:

```bash
git clone https://github.com/SEU-USUARIO/dio-agent-cybersecurity.git
```

Entre na pasta:

```bash
cd dio-agent-cybersecurity
```

Execute o Hermes na raiz do projeto:

```bash
hermes
```

O agente poderá utilizar as instruções, conhecimentos e skills do projeto conforme a configuração do ambiente.

Para executar o laboratório Python:

```bash
python app.py
```

## 8. Evidências do projeto

Nesta seção serão apresentados registros da execução e dos testes realizados:

- Análise inicial da vulnerabilidade SQL Injection.
- Código corrigido utilizando consultas parametrizadas.
- Nova análise de segurança após a correção.
- Teste do agente utilizando a skill de análise de vulnerabilidades.
- Perguntas de contexto realizadas pelo agente antes de recomendar procedimentos.

## 9. Considerações finais

O desenvolvimento deste projeto permitiu aprofundar conhecimentos sobre análise de vulnerabilidades, segurança de aplicações, SQL Injection, documentação técnica e utilização de agentes de inteligência artificial.

Além disso, foi possível compreender como instruções, arquivos de conhecimento e skills podem modificar o comportamento de um agente sem a necessidade de treinar um novo modelo.

O projeto foi desenvolvido com finalidade educacional, utilizando exclusivamente um ambiente de laboratório controlado.
