# Fluxograma de Acordo de Cooperação - Lei 14.133/2021

```mermaid
flowchart TD
    %% Início e Diretoria Demandante
    A["Início"] --> B["Diretoria Demandante"]
    B --> C["Elaboração dos documentos essenciais:<br>Justificativa do interesse público<br>Objeto da cooperação<br>Plano de trabalho<br>Identificação dos partícipes<br>Prazo de vigência"]
    
    %% Fluxo entre departamentos iniciais
    C --> D["DG - Diretoria Geral<br>Recebe o processo"]
    D --> E["Verifica a solicitação<br>Encaminha para DAT"]
    
    %% DAT - Diretoria de Apoio Técnico
    E --> F["DAT - Diretoria de Apoio Técnico<br>Recebe e processa"]
    F --> G["Verifica natureza da cooperação:<br>Confirma ausência de transferência de recursos<br>Analisa interesse recíproco<br>Verifica capacidade técnica dos partícipes"]
    
    %% Verificação de documentação
    G --> H["Analisa documentação:<br>Verifica plano de trabalho<br>Analisa capacidade técnica<br>Verifica completude do processo"]
    H --> I["Verifica documentos essenciais:<br>Justificativa do interesse público<br>Plano de trabalho detalhado<br>Documentação dos partícipes<br>Comprovação de capacidade técnica"]
    
    %% Elaboração de documentos técnicos
    I --> J["Elabora documentos do Acordo:<br>Minuta do Acordo de Cooperação<br>Plano de trabalho detalhado<br>Cronograma de execução<br>Definição de responsabilidades<br>Estabelece mecanismos de acompanhamento"]
    
    %% Encaminhamento para 1ª SEC
    J --> K["Encaminha processo para 1ª SEC"]
    
    %% 1ª SEC
    K --> L["1ª SEC<br>Recebe e processa"]
    L --> M["Verifica documentação<br>Encaminha para Procuradoria<br>Se necessário, solicita complementação"]
    
    %% Procuradoria
    M --> N["Procuradoria<br>Recebe o processo"]
    N --> O["Analisa parecer jurídico:<br>Verifica legalidade do procedimento<br>Analisa minuta do Acordo<br>Verifica adequação do plano de trabalho<br>Encaminha para Controladoria"]
    
    %% Controladoria
    O --> P["Controladoria<br>Recebe o processo"]
    P --> Q["Analisa legalidade<br>Verifica mecanismos de controle<br>Encaminha para o DG"]
    
    %% Retorno ao DG e Continuidade
    Q --> R["DG recebe processo com pareceres"]
    R --> S["Verifica autorização:<br>Analisa pareceres<br>Solicita autorização do Presidente<br>Encaminha para DAT"]
    
    %% Assinatura do Acordo
    S --> T["DAT prepara Acordo de Cooperação:<br>Finaliza a minuta<br>Agenda assinatura com partícipes<br>Coleta assinaturas<br>Publica extrato no Diário Oficial"]
    
    %% Execução do Acordo
    T --> U["Execução do Acordo:<br>Designa gestor do Acordo<br>Inicia execução do plano de trabalho<br>Realiza reuniões periódicas<br>Monitora cronograma<br>Elabora relatórios de acompanhamento"]
    
    %% Avaliação e Monitoramento
    U --> V["Avaliação e Monitoramento:<br>Verifica cumprimento de metas<br>Analisa resultados parciais<br>Propõe ajustes (se necessário)<br>Elabora relatórios periódicos"]
    
    %% Prorrogação ou Encerramento
    V --> W{"Necessidade de prorrogação?"}
    W -->|"Sim"| X["Prorrogação:<br>Justifica necessidade<br>Elabora termo aditivo<br>Atualiza plano de trabalho<br>Coleta assinaturas<br>Publica extrato"]
    W -->|"Não"| Y["Encerramento:<br>Verifica cumprimento do objeto<br>Elabora relatório final<br>Avalia resultados<br>Formaliza encerramento"]
    
    %% Retorno ao ciclo ou Finalização
    X --> U
    Y --> Z["Prestação de contas final:<br>Elabora relatório de cumprimento<br>Documenta resultados alcançados<br>Avalia efetividade da cooperação<br>Arquiva processo"]
    
    %% Check List Acordo de Cooperação - Lateral
    subgraph "Check List Acordo de Cooperação"
    CL1["Documentos para iniciar processo:<br>Justificativa do interesse público<br>Plano de trabalho<br>Documentação dos partícipes<br>Comprovação de capacidade técnica"]
    
    CL2["Documentos do Acordo:<br>Minuta do Acordo de Cooperação<br>Plano de trabalho detalhado<br>Cronograma de execução<br>Definição de responsabilidades<br>Parecer Jurídico<br>Publicações"]
    
    CL3["Documentos de execução:<br>Designação de gestor<br>Relatórios de acompanhamento<br>Atas de reuniões<br>Registros de atividades<br>Produtos/resultados parciais"]
    
    CL4["Documentos de encerramento:<br>Relatório final<br>Avaliação de resultados<br>Termo de encerramento<br>Comprovação de cumprimento do objeto"]
    end
    
    %% Características do Acordo de Cooperação
    subgraph "Características do Acordo de Cooperação"
    CP1["Aplicabilidade:<br>Interesse recíproco<br>Ausência de transferência de recursos<br>Compartilhamento de conhecimentos<br>Ações conjuntas<br>Intercâmbio de experiências"]
    
    CP2["Particularidades:<br>Não envolve repasse financeiro<br>Baseado em cooperação mútua<br>Foco em resultados comuns<br>Compartilhamento de recursos não financeiros"]
    
    CP3["Prazos:<br>Vigência: conforme plano de trabalho<br>Prorrogação: mediante termo aditivo<br>Publicação: até 20 dias após assinatura"]
    end
    
    %% Diferenças para Convênios
    subgraph "Diferenças para Convênios"
    DC1["Acordo de Cooperação:<br>Sem transferência de recursos<br>Compartilhamento de recursos não financeiros<br>Menor complexidade documental"]
    
    DC2["Convênio:<br>Com transferência de recursos<br>Prestação de contas financeira<br>Maior complexidade documental<br>Regras específicas de execução financeira"]
    end
