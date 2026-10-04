# FIAP - Faculdade de Informática e Administração Paulista

# CardioIA — Fase 2

## Diagnóstico Automatizado — IA no Estetoscópio Digital

Projeto acadêmico desenvolvido para a Fase 2 do curso de Inteligência Artificial da FIAP.

## 📜 Descrição

O CardioIA é um projeto acadêmico voltado à aplicação de Inteligência Artificial no contexto cardiovascular.

Nesta etapa, o projeto utiliza Processamento de Linguagem Natural (NLP) para analisar relatos textuais simulados de pacientes, identificar sintomas e características clínicas presentes no texto e relacioná-los a possíveis condições cadastradas em uma base de conhecimento.

O sistema não realiza diagnóstico médico. Os resultados representam associações educacionais baseadas nas regras e fontes cadastradas no projeto.

## 🧠 Funcionalidades implementadas

Nesta versão já foram implementados:

- Base de conhecimento de sintomas e manifestações cardiovasculares;
- Normalização de relatos textuais;
- Identificação de sintomas por expressões em linguagem natural;
- Identificação de atributos clínicos, como esforço, repouso, duração, irradiação e temporalidade;
- Associação dos conceitos encontrados com possíveis condições cardiovasculares;
- Pontuação explicativa baseada nas evidências encontradas;
- Exibição das fontes científicas relacionadas às associações;
- Testes utilizando 10 relatos simulados de pacientes.

A etapa de classificação de risco utilizando TF-IDF e Machine Learning será adicionada durante a continuidade da Fase 2.

## 📁 Estrutura do projeto

```text
CardioAI/
├── assets/
├── config/
├── data/
│   └── relatos_pacientes.txt
├── document/
├── knowledge_base/
│   ├── associacoes.csv
│   ├── atributos.csv
│   ├── conceitos.csv
│   ├── expressoes.csv
│   ├── fontes.csv
│   └── README.md
├── notebooks/
├── scripts/
├── src/
│   ├── analisador_clinico.py
│   ├── carregador_base.py
│   ├── extrator_sintomas.py
│   ├── main.py
│   └── README.md
└── tests/

```
## 🗃 Base de conhecimento

A pasta `knowledge_base` contém os arquivos utilizados pelo sistema para interpretar os relatos.

- `conceitos.csv`: conceitos clínicos normalizados;
- `expressoes.csv`: formas de expressão utilizadas pelos pacientes;
- `atributos.csv`: características contextuais dos sintomas;
- `associacoes.csv`: relações entre conceitos e condições;
- `fontes.csv`: referências utilizadas na construção da base.

As expressões simuladas representam formas possíveis de linguagem dos pacientes e não devem ser interpretadas como citações literais das fontes científicas.

## 🔧 Como executar

### Pré-requisitos

- Python 3

Na raiz do projeto, execute:

    python3 src/main.py

O programa carregará os relatos presentes em `data/relatos_pacientes.txt`, realizará a extração dos conceitos e atributos e exibirá as possíveis associações encontradas.

## ⚠️ Aviso

Este projeto possui finalidade exclusivamente acadêmica e educacional.

As associações apresentadas pelo sistema não representam diagnóstico médico e não substituem avaliação realizada por profissionais de saúde.

## 🚧 Status da Fase 2

### Parte 1 — NLP e base de conhecimento

**Implementada e testada.**

### Parte 2 — Classificação de risco com Machine Learning

**Em desenvolvimento.**

Está prevista a utilização de TF-IDF e um algoritmo de classificação supervisionada para classificar relatos simulados em categorias de risco.

## 📋 Histórico

### v0.1.0

- Criação da base de conhecimento da Fase 2;
- Implementação do extrator de sintomas;
- Implementação da análise de atributos e contexto;
- Implementação das associações explicáveis;
- Validação utilizando 10 relatos simulados.

## 📚 Contexto acadêmico

Projeto desenvolvido como parte das atividades acadêmicas da FIAP — Faculdade de Informática e Administração Paulista.
