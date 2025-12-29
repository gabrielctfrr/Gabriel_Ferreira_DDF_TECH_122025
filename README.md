# Gabriel_Ferreira_DDF_TECH_122025

# Item 0: Planejamento e Gestão do Projeto

Este documento detalha o planejamento do projeto de implementação da Plataforma de Dados para E-commerce, seguindo as melhores práticas do PMBOK. O ciclo de vida do projeto foi dividido em 5 fases: Iniciação, Planejamento, Execução, Monitoramento e Encerramento.

## 1. Visão Geral do Cronograma (Gantt Chart)

O gráfico abaixo representa o fluxo temporal e as interdependências entre as tarefas.

```mermaid
gantt
    title Cronograma de Implementação - Data Platform Olist
    dateFormat  YYYY-MM-DD
    axisFormat  %d/%m
    
    section Iniciação
    Definição do Escopo e KPI      :done,    init1, 2025-12-27, 1d
    Seleção do Dataset (Olist)     :done,    init2, 2025-12-27, 1d

    section Planejamento
    Arquitetura da Solução         :active,  plan1, 2025-12-27, 1d
    Análise de Riscos e Recursos   :active,  plan2, 2025-12-27, 1d

    section Execução (Engenharia)
    Ingestão de Dados (Dadosfera)  :         exec1, after plan1, 2d
    Limpeza e Tratamento (SQL/Py)  :         exec2, after exec1, 2d

    section Execução (Data Science)
    Análise Exploratória (EDA)     :         ds1, after exec2, 2d
    Modelagem Preditiva (ML)       :         ds2, after ds1, 3d

    section Entrega de Valor
    Desenvolvimento Data App       :         app1, after ds2, 2d
    Gravação do Vídeo de Demo      :crit,    final1, after app1, 1d
    Documentação Final             :         final2, after final1, 1d****
