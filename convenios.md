# Fluxograma de Convênios - Lei 14.133/2021

```mermaid
flowchart TD
    %% Início e Diretoria Demandante
    A["Início"] --> B["Diretoria Demandante"]
    B --> C["Elaboração dos documentos essenciais:<br>Justificativa do interesse público<br>Objeto do convênio<br>Plano de trabalho detalhado<br>Identificação dos partícipes<br>Valor e cronograma de desembolso<br>Contrapartida (se houver)"]
    
    %% Fluxo entre departamentos iniciais
    C --> D["DG - Diretoria Geral<br>Recebe o processo"]
    D --> E["Verifica a solicitação<br>Encaminha para DAT"]
    
    %% DAT - Diretoria de Apoio Técnico
    E --> F["DAT - Diretoria de Apoio Técnico<br>Recebe e processa"]
    F --> G["Verifica natureza do convênio:<br>Confirma transferência de recursos<br>Analisa interesse recíproco<br>Verifica capacidade técnica e operacional<br>Analisa viabilidade do plano de trabalho"]
    
    %% Verificação de documentação
    G --> H["Analisa documentação:<br>Verifica plano de trabalho<br>Analisa capacidade técnica e operacional<br>Verifica completude do processo<br>Analisa cronograma de desembolso"]
    H --> I["Verifica documentos essenciais:<br>Justificativa do interesse público<br>Plano de trabalho detalhado<br>Documentação dos partícipes<br>Comprovação de capacidade técnica<br>Comprovação de regularidade fiscal"]
    
    %% Elaboração de documentos técnicos
    I --> J["Elabora documentos do Convênio:<br>Minuta do Termo de Convênio<br>Plano de trabalho detalhado<br>Cronograma de execução<br>Cronograma de desembolso<br>Definição de responsabilidades<br>Estabelece mecanismos de prestação de contas"]
    
    %% Verificação orçamentária
    J --> K["Verifica disponibilidade orçamentária:<br>Confirma dotação orçamentária<br>Verifica programação financeira<br>Analisa cronograma de desembolso"]
    
    %% Encaminhamento para 1ª SEC
    K --> L["Encaminha processo para 1ª SEC"]
    
    %% 1ª SEC
    L --> M["1ª SEC<br>Recebe e processa"]
    M --> N["Verifica documentação<br>Encaminha para Procuradoria<br>Se necessário, solicita complementação"]
    
    %% Procuradoria
    N --> O["Procuradoria<br>Recebe o processo"]
    O --> P["Analisa parecer jurídico:<br>Verifica legalidade do procedimento<br>Analisa minuta do Convênio<br>Verifica adequação do plano de trabalho<br>Analisa mecanismos de controle<br>Encaminha para Controladoria"]
    
    %% Controladoria
    P --> Q["Controladoria<br>Recebe o processo"]
    Q --> R["Analisa legalidade<br>Verifica mecanismos de controle<br>Analisa prestação de contas<br>Encaminha para o DG"]
    
    %% Retorno ao DG e Continuidade
    R --> S["DG recebe processo com pareceres"]
    S --> T["Verifica autorização:<br>Analisa pareceres<br>Solicita autorização do Presidente<br>Encaminha para DAT"]
    
    %% Assinatura do Convênio
    T --> U["DAT prepara Termo de Convênio:<br>Finaliza a minuta<br>Agenda assinatura com partícipes<br>Coleta assinaturas<br>Publica extrato no Diário Oficial<br>Emite nota de empenho"]
    
    %% Execução do Convênio
    U --> V["Execução do Convênio:<br>Designa gestor do Convênio<br>Realiza transferência de recursos<br>Inicia execução do plano de trabalho<br>Monitora cronograma<br>Elabora relatórios de acompanhamento"]
    
    %% Monitoramento e Fiscalização
    V --> W["Monitoramento e Fiscalização:<br>Verifica cumprimento de metas<br>Analisa execução financeira<br>Realiza visitas técnicas<br>Analisa relatórios parciais<br>Propõe ajustes (se necessário)"]
    
    %% Prestação de Contas Parcial
    W --> X["Prestação de Contas Parcial:<br>Recebe relatórios parciais<br>Analisa execução física e financeira<br>Verifica documentação comprobatória<br>Emite parecer sobre continuidade"]
    
    %% Decisão sobre continuidade
    X --> Y{"Continuidade do Convênio?"}
    Y -->|"Sim"| Z["Continuidade:<br>Libera parcelas subsequentes<br>Atualiza cronograma (se necessário)<br>Continua monitoramento"]
    Y -->|"Não"| ZA["Interrupção:<br>Suspende repasses<br>Notifica convenente<br>Solicita devolução de recursos<br>Instaura tomada de contas especial (se necessário)"]
    
    %% Retorno ao ciclo ou Encerramento
    Z --> W
    ZA --> ZC["Encerramento antecipado:<br>Formaliza rescisão<br>Exige prestação de contas final<br>Analisa devolução de recursos<br>Registra inadimplência (se for o caso)"]
    
    %% Encerramento normal
    Y -->|"Término da vigência"| ZB["Encerramento normal:<br>Verifica cumprimento do objeto<br>Solicita prestação de contas final<br>Avalia resultados<br>Formaliza encerramento"]
    
    %% Prestação de Contas Final
    ZB --> ZD["Prestação de Contas Final:<br>Recebe relatório final<br>Analisa execução física e financeira<br>Verifica documentação comprobatória<br>Emite parecer conclusivo"]
    ZC --> ZD
    
    %% Aprovação das Contas
    ZD --> ZE{"Aprovação das contas?"}
    ZE -->|"Sim"| ZF["Aprovação:<br>Emite parecer de aprovação<br>Registra aprovação<br>Arquiva processo"]
    ZE -->|"Não"| ZG["Rejeição:<br>Notifica convenente<br>Estabelece prazo para regularização<br>Instaura tomada de contas especial (se não regularizado)<br>Registra inadimplência"]
    
    %% Finalização
    ZF --> ZH["Finalização:<br>Emite certificado de cumprimento<br>Libera garantias (se houver)<br>Arquiva processo"]
    ZG --> ZI["Medidas administrativas/judiciais:<br>Inscrição em dívida ativa<br>Processo administrativo<br>Ação judicial<br>Arquiva processo"]
    
    %% Check List Convênios - Lateral
    subgraph "Check List Convênios"
    CL1["Documentos para iniciar processo:<br>Justificativa do interesse público<br>Plano de trabalho detalhado<br>Documentação dos partícipes<br>Comprovação de capacidade técnica<br>Comprovação de regularidade fiscal<br>Declaração de contrapartida (se houver)"]
    
    CL2["Documentos do Convênio:<br>Minuta do Termo de Convênio<br>Plano de trabalho detalhado<br>Cronograma de execução<br>Cronograma de desembolso<br>Parecer Jurídico<br>Nota de empenho<br>Publicações"]
    
    CL3["Documentos de execução:<br>Designação de gestor<br>Comprovantes de transferência<br>Relatórios de acompanhamento<br>Relatórios de visitas técnicas<br>Prestações de contas parciais"]
    
    CL4["Documentos de prestação de contas:<br>Relatório de cumprimento do objeto<br>Relatório de execução físico-financeira<br>Demonstrativo de receitas e despesas<br>Relação de pagamentos<br>Extratos bancários<br>Comprovantes de despesas<br>Termo de aceitação definitiva"]
    end
    
    %% Características dos Convênios
    subgraph "Características dos Convênios"
    CP1["Aplicabilidade:<br>Interesse recíproco<br>Transferência de recursos<br>Execução descentralizada<br>Regime de mútua cooperação"]
    
    CP2["Particularidades:<br>Envolve repasse financeiro<br>Exige prestação de contas<br>Contrapartida (financeira ou não)<br>Conta bancária específica<br>Aplicação financeira obrigatória"]
    
    CP3["Prazos:<br>Vigência: conforme plano de trabalho<br>Prestação de contas: até 60 dias após término<br>Publicação: até 20 dias após assinatura<br>Análise das contas: até 150 dias"]
    end
    
    %% Vedações
    subgraph "Vedações"
    VD1["É vedado:<br>Realização de despesas fora da vigência<br>Utilização dos recursos em finalidade diversa<br>Realização de despesas com taxas bancárias<br>Pagamento de gratificação a servidor público<br>Transferência de recursos para clubes e associações de servidores"]
    end
