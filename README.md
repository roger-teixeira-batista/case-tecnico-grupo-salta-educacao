# Case Técnico – Célula de Operações e Pagamentos | ONC

## Sobre o projeto

Este repositório contém a resolução do **Case Técnico da Olimpíada Nacional de Ciências (ONC)**, desenvolvido para simular atividades relacionadas à **Célula de Operações e Pagamentos**.

O desafio envolve a análise e o tratamento de dados de produção e pagamentos de avaliadores freelancers responsáveis pela correção das provas da ONC, com foco na **acurácia dos repasses financeiros**, identificação de inconsistências, realização de ajustes retroativos e análise orçamentária.

A solução foi desenvolvida utilizando **Python e Google Colab**, com apoio de ferramentas de análise e tratamento de dados.

---

## Objetivos do Case

O projeto contempla as seguintes etapas:

### 1. Conferência e tratamento da base de avaliadores

* Padronização dos dados cadastrais dos avaliadores;
* Tratamento de nomes e informações textuais;
* Cruzamento entre a base de avaliadores e a base de produção/pagamentos;
* Identificação de inconsistências e dados faltantes;
* Organização da base final seguindo a ordenação por **Nome Completo (A-Z)** e **Regional (A-Z)**;
* Elaboração de uma comunicação para solicitar ao representante da marca as informações necessárias para solucionar eventuais inconsistências.

A base oficial de avaliadores contém informações como **ID Avaliador, Nome Avaliador, Regional, Valor por Prova e Salário Recorrente**, enquanto a base de produção apresenta informações referentes aos lotes corrigidos e aos respectivos bônus de complexidade.

---

### 2. Ajuste retroativo e análise de desconto

Foi realizada uma análise do erro de pagamento ocorrido no mês de abril envolvendo o avaliador **Marcos Oliveira (ID 12345)**.

A análise considera:

* Quantidade de lotes pagos indevidamente em abril;
* Quantidade efetivamente corrigida;
* Produção realizada em maio;
* Cálculo do valor pago indevidamente;
* Aplicação do desconto na folha de pagamento;
* Limite máximo de desconto de **30% do salário recorrente**;
* Definição da quantidade mínima de parcelas necessárias quando o valor do desconto ultrapassa o limite permitido;
* Cálculo da remuneração total referente ao mês de maio;
* Identificação de possíveis parcelas futuras.

A regra definida no case estabelece que nenhum desconto pode ultrapassar 30% do salário recorrente do avaliador. Caso o valor seja superior ao limite, o desconto deve ser parcelado no menor número de parcelas possível sem ultrapassar esse teto.

---

### 3. Comunicação ao colaborador

Foi elaborado um modelo de e-mail direcionado ao avaliador Marcos Oliveira, apresentando de forma clara e transparente:

* O erro identificado no pagamento de abril;
* O motivo do ajuste;
* O valor a ser descontado;
* A forma como o desconto será aplicado;
* A existência de parcelamento, quando aplicável;
* O impacto nos próximos pagamentos.

A comunicação busca apresentar as informações financeiras de maneira objetiva, mantendo clareza sobre o processo de ajuste e os próximos pagamentos.

---

### 4. Análise orçamentária

Foi realizada uma análise de **Real x Orçado** considerando exclusivamente os pagamentos referentes às correções realizadas em maio, sem incluir o salário recorrente dos avaliadores.

A análise tem como objetivos:

* Comparar os pagamentos realizados com o orçamento disponível para cada regional;
* Identificar quais regionais ultrapassaram o orçamento previsto;
* Avaliar os custos médios de correção por prova;
* Identificar as regionais com maiores custos;
* Apresentar os resultados por meio de visualizações gráficas;
* Elaborar uma comunicação para a diretoria da marca com os principais resultados e sugestões de planos de ação.

Os orçamentos definidos no case são:

| Regional   | Orçamento de Maio – Correções |
| ---------- | ----------------------------: |
| Regional A |                 R$ 126.438,09 |
| Regional B |                 R$ 108.338,70 |
| Regional C |                 R$ 141.529,82 |
| Regional D |                 R$ 132.443,15 |
| Regional E |                 R$ 100.172,62 |

A análise orçamentária considera exclusivamente os pagamentos de correção de maio, conforme definido nas instruções do case.

---

## Tecnologias e ferramentas utilizadas

* **Python**
* **Google Colab**
* **Pandas**
* **Matplotlib**
* **Excel**
* **Jupyter Notebook**

As principais etapas de tratamento e análise dos dados foram realizadas utilizando Python, com foco em manipulação de dados, cruzamento de bases, cálculos financeiros, análise orçamentária e visualização de informações.

---

## Estrutura do projeto

```text
📁 Case_Grupo_Salta_ONC
│
├── 📓 Case_Grupo_Salta_ONC.ipynb
│   └── Notebook desenvolvido no Google Colab contendo o tratamento,
│       análise dos dados, cálculos e visualizações do case.
│
├── 📄 Instruções do Case.pdf
│   └── Documento com as instruções e requisitos do desafio.
│
├── 📊 ONC_Base_Candidato (1) (1).xlsx
│   └── Base de dados bruta utilizada como fonte para o desenvolvimento
│       da solução.
│
├── 📊 ONC_base_final.xlsx
│   └── Base final após o tratamento, padronização e organização dos dados.
│
└── 📁 Arquivos em Texto
    ├── 📄 [arquivos textuais da solução]
    └── 📄 [comunicações e análises produzidas no case]
```

---

## Fluxo de desenvolvimento

O projeto seguiu, de forma geral, o seguinte fluxo:

```text
Dados Brutos
     │
     ▼
Tratamento e Padronização
     │
     ▼
Conferência e Cruzamento das Bases
     │
     ▼
Identificação de Inconsistências
     │
     ▼
Cálculos e Ajustes Financeiros
     │
     ▼
Análise Orçamentária
     │
     ▼
Visualização dos Resultados
     │
     ▼
Comunicações e Planos de Ação
     │
     ▼
Base Final Tratada
```

---

## Principais entregáveis

O repositório disponibiliza:

1. **Notebook de análise** com o desenvolvimento da solução;
2. **Base bruta** fornecida para o case;
3. **Base final tratada** após o processo de ETL e análise;
4. **Documento com as instruções originais** do desafio;
5. **Arquivos textuais** contendo as respostas e comunicações elaboradas durante a resolução.

As instruções do desafio solicitam o retorno das bases tratadas e dos arquivos eventualmente criados com as respostas e considerações da resolução.

---

## Considerações finais

Este projeto foi desenvolvido com o objetivo de demonstrar a aplicação prática de conceitos de **Análise de Dados, Tratamento de Dados, ETL, análise financeira e visualização de informações** em um contexto de Operações e Pagamentos.

Além da análise quantitativa, a solução também considera a importância da **comunicação dos resultados** para diferentes públicos, incluindo representantes de marca, colaboradores e diretoria, transformando os dados analisados em informações que podem apoiar a tomada de decisão.

---

## Autor

**Roger Teixeira Batista**

Projeto desenvolvido como resolução do **Case Técnico – Célula de Operações e Pagamentos da Olimpíada Nacional de Ciências (ONC)**.
