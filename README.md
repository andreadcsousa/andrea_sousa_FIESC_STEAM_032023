# 💼 Profissionais STEAM em Santa Catarina (Case FIESC)

Este repositório apresenta a resolução de um estudo de caso técnico real, desenvolvido para o processo seletivo do Observatório da FIESC (IEL), cujo resultado validou minhas competências e garantiu minha contratação. O objetivo do projeto foi utilizar dados oficiais do Novo CAGED para analisar o mercado de trabalho de profissionais das áreas de **STEAM** (Ciência, Tecnologia, Engenharia e Matemática) no estado de Santa Catarina.

## 🎯 O Problema de Negócio & Hipóteses

O Observatório da FIESC vinha recebendo relatos de empresários locais indicando extrema dificuldade em **contratar e reter** profissionais das áreas de tecnologia e engenharia. 

O desafio consistiu em agir como um analista consultivo para:
1. **Formular e testar hipóteses** baseadas nos dados brutos de movimentação do CAGED para validar se a dor dos empresários era real.
2. **Identificar gargalos:** Descobrir se o problema era a falta de contratações (baixa oferta), alta rotatividade (turnover agressivo) ou descompasso salarial.
3. **Mapear o cenário:** Agrupar ocupações usando filtros específicos de CBO (Famílias 20, 21 e 22) para isolar o ecossistema STEAM.

## 🛠️ Tecnologias Utilizadas

* **Python & Pandas:** Exploração ágil do dataset, aplicação de filtros específicos de CBOs, limpeza e agregações demográficas e regionais.
* **Seaborn & Matplotlib:** Geração de gráficos de distribuição para análise exploratória de tipos de movimentação (admissões vs. demissões).
* **Power BI:** Desenvolvimento de painel analítico voltado para apresentação executiva de resultados e indicadores de monitoramento (salário médio, saldo de vagas e principais setores empregadores).

## 📈 Insights e Conclusões da Análise

* **Validação da Dor:** Os dados confirmaram uma alta volatilidade nas contratações. Cargos como *Analista de Desenvolvimento de Sistemas* e *Enfermeiro* figuraram entre as principais movimentações, mostrando alta demanda, mas também um volume expressivo de desligamentos a pedido.
* **Comportamento Salarial:** A média salarial de admissão em SC foi mapeada por município e por CNAE (Setor Econômico), permitindo identificar se as empresas que reclamavam de retenção estavam praticando salários abaixo da média de mercado do estado.
* **Gargalo de Retenção:** Identificou-se que o saldo de movimentações (Admitidos - Desligados) em determinados períodos era estreito para funções de tecnologia, sinalizando que a dor principal do mercado não era a falta de contratação, mas sim a incapacidade de retenção (*turnover*).

## 🚀 Ideias de Evolução (Indo Além do Case)

Como este projeto reflete um cenário real de mercado, planejo expandir o escopo original com as seguintes implementações:

- [ ] **Análise de Input de Talentos (Oferta vs. Demanda):** Integrar os dados do Censo da Educação Superior (INEP) para mapear o volume de formandos em cursos STEAM por região. O objetivo é contrastar a formação de novos entrantes com a taxa de abertura de vagas do CAGED, identificando se o gargalo do mercado é a escassez de formação ou a retenção salarial.
- [ ] **Machine Learning (Previsão de Salários):** Construir um modelo de regressão para prever o salário médio de admissão com base na região, porte da empresa (CNAE) e nível de senioridade do CBO.
- [ ] **Análise de Cohort para Turnover:** Estruturar uma análise temporal para medir o tempo médio de permanência do profissional STEAM em cada cadeira antes do desligamento.
- [ ] **Automação do Pipeline (ETL):** Migrar a leitura dos arquivos locais para um pipeline dinâmico que consome diretamente os dados mensais disponibilizados pelo FTP do Ministério do Trabalho e Emprego.

<img src="./dashboard_steam.jpg" width="100%">  
