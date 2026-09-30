# Universidade Estadual da Paraíba — UEPB
**Curso:** Tecnologia em Ciência de Dados / Computação  
**Disciplina:** Projeto Integrador na Prática Educacional  
**Docente:** [Nome do Professor]  
**Equipe:**
- Inacia Kelly Gonçalves de Souza Santos — [@kellyantunes](https://github.com/kellyantunes)
- Pietra — [@usuario-pietra](https://github.com/)
- Manuela — [@usuario-manuela](https://github.com/)

---

## 1. O Projeto
Este projeto tem como objetivo analisar o perfil de carga e esforço de trabalho dos professores da Educação Básica no Brasil, investigando disparidades estruturais entre redes de ensino (municipal, estadual, federal e privada), regiões do país e localização escolar (urbana vs. rural).

## 2. A Base de Dados Escolhida
- **Nome da base:** Indicador de Esforço Docente (IED) — Municípios[cite: 1]
- **Arquivo de origem:** `IED_MUNICIPIOS_2025.ods` / `IED_MUNICIPIOS_2025.xlsx`[cite: 1]
- **Órgão emissor / Fonte:** INEP / MEC (Diretoria de Estatísticas Educacionais - DEED)[cite: 1]
- **Ano censitário coberto:** 2025[cite: 1]
- **Cada linha representa:** A distribuição percentual dos docentes em cada nível de esforço de trabalho para uma combinação específica de Município, Dependência Administrativa, Localização Escolar e Etapa de Ensino.
- **Dimensões da base:**
  - **Total de linhas:** *~170.000 a 230.000 linhas* (o valor exato apurado no Colab via `df.shape[0]`)
  - **Total de colunas:** *14 colunas principais* (`df.shape[1] = 14`)
- **Licença / Termos:** Dados Abertos Governamentais (Domínio Público / Governo Federal do Brasil).

## 3. Nossas Perguntas de Análise
1. **Disparidade por Dependência:** Qual rede de ensino (Estadual, Municipal ou Privada) concentra a maior proporção de docentes nos níveis de esforço mais críticos (Níveis 5 e 6)?
2. **Abismo Urbano vs. Rural:** Existe diferença significativa no percentual de professores com sobrecarga de turnos e escolas entre áreas urbanas e rurais nos municípios brasileiros?
3. **Desigualdade Regional:** Como se distribuem os docentes do Nível 6 (mais de 400 alunos e 3 turnos/escolas) entre as cinco Grandes Regiões do Brasil?

## 4. Estrutura do Repositório
```text
├── README.md               # Apresentação do projeto, base e perguntas
├── .gitignore              # Arquivos e extensões ignorados pelo Git
├── dados/
│   ├── bruto/              # Amostra da base bruta (.csv) e .gitkeep
│   └── tratado/            # Dados limpos após tratamento e .gitkeep
├── notebooks/              # Jupyter Notebooks com a exploração dos dados
├── docs/                   # Documentação auxiliar e dicionário de dados
│   ├── dicionario.md       # Dicionário de dados formal
│   └── plano-de-analise.md # Plano de análise (Entrega 1)
└── equipe/                 # Contrato da equipe e diários de bordo
