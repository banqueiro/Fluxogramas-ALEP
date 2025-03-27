
# Fluxograma de Pregão Presencial - Lei 14.133/2021

```mermaid
flowchart TD
    %% Início e Diretoria Demandante
    A["Início"] --> B["Diretoria Demandante"]
    B --> C["Elaboração dos documentos essenciais:<br>Justificativa da contratação<br>Objeto claro e preciso<br>Valor estimado<br>Prazo para a execução<br>Indicação da dotação orçamentária"]
    
    %% Fluxo entre departamentos iniciais
    C --> D["DG - Diretoria Geral<br>Recebe o processo"]
    D --> E["Verifica a solicitação<br>Encaminha para DAT"]
    
    %% DAT - Diretoria de Apoio Técnico
    E --> F["DAT - Diretoria de Apoio Técnico<br>Recebe e processa"]
    F --> G["Verifica se o objeto é comum<br>Justifica a adoção do Pregão Presencial<br>Complementa pesquisa de preços<br>Elabora mapa comparativo"]
    
    %% Verificação de documentação e pesquisa de preços
    G --> H["Realiza pesquisa complementar<br>Compara valores<br>Verifica completude do processo"]
    H --> I["Verifica documentos essenciais:<br>Justificativa da contratação<br>Objeto claro e preciso<br>Valor estimado com pesquisa<br>Prazo para execução<br>Dotação orçamentária"]
    
    %% Elaboração de documentos técnicos
    I --> J["Elabora documentos do Pregão:<br>Termo de Referência detalhado<br>Elabora mapa comparativo<br>Calcula valor médio<br>Verifica disponibilidade orçamentária<br>Elabora minuta do edital<br>Define critérios de julgamento"]
    
    %% Verificação de modalidade
    J --> K["Confirma modalidade Pregão Presencial:<br>Verifica se objeto é bem/serviço comum<br>Justifica a não adoção do Pregão Eletrônico<br>Define modo de disputa<br>Estabelece intervalo mínimo de lances"]
    
    %% Encaminhamento para 1ª SEC
    K --> L["Encaminha processo para 1ª SEC"]
    
    %% 1ª SEC
    L --> M["1ª SEC<br>Recebe e processa"]
    M --> N["Verifica documentação<br>Encaminha para Procuradoria<br>Se necessário, solicita complementação"]
    
    %% Procuradoria
    N --> O["Procuradoria<br>Recebe o processo"]
    O --> P["Analisa parecer jurídico<br>Verifica legalidade do procedimento<br>Verifica justificativa para Pregão Presencial<br>Encaminha para Controladoria"]
    
    %% Controladoria
    P --> Q["Controladoria<br>Recebe o processo"]
    Q --> R["Analisa legalidade<br>Encaminha para o DG"]
    
    %% Retorno ao DG e Continuidade
    R --> S["DG recebe processo com pareceres"]
    S --> T["Verifica autorização:<br>Analisa pareceres<br>Solicita autorização do Presidente<br>Encaminha para DAT"]
    
    %% Preparação do Edital e Publicação
    T --> U["DAT prepara edital de Pregão:<br>Finaliza o edital<br>Realiza publicação no PNCP e Diário Oficial<br>Marca data da sessão presencial<br>Designa pregoeiro e equipe de apoio"]
    
    %% Sessão Pública do Pregão
    U --> V["Sessão pública do Pregão Presencial:<br>Credenciamento dos licitantes<br>Entrega dos envelopes<br>Abertura das propostas<br>Classificação para lances<br>Fase de lances verbais<br>Negociação<br>Habilitação"]
    
    %% Adjudicação e Homologação
    V --> W["Adjudicação:<br>Pregoeiro declara vencedor<br>Abre prazo recursal<br>Adjudica objeto (se não houver recurso)"]
    W --> X["Homologação:<br>Autoridade superior analisa processo<br>Solicita homologação do Presidente"]
    
    %% Contratação
    X --> Y["Contrato e empenho:<br>Elabora contrato<br>Convoca para assinatura<br>Emite nota de empenho<br>Publica extrato no PNCP"]
    
    %% Gestão Contratual
    Y --> Z["Gestão do contrato:<br>Designa fiscal e gestor<br>Acompanha execução<br>Realiza pagamentos<br>Verifica cumprimento"]
    
    %% Finalização
    Z --> ZA["Encerramento:<br>Verifica conclusão<br>Emite termo de recebimento<br>Arquiva processo"]
    
    %% Check List Pregão Presencial - Lateral
    subgraph "Check List Pregão Presencial"
    CL1["Documentos para iniciar processo:<br>Justificativa da contratação<br>Termo de Referência detalhado<br>Pesquisa de preços (mínimo 3 orçamentos)<br>Estudo Técnico Preliminar (ETP)<br>Análise de Riscos<br>Justificativa para adoção do Pregão Presencial"]
    
    CL2["Documentos do Edital:<br>Minuta do Edital<br>Termo de Referência<br>Minuta do Contrato<br>Parecer Jurídico<br>Designação do Pregoeiro<br>Publicações"]
    
    CL3["Documentos da Sessão:<br>Lista de credenciamento<br>Propostas dos licitantes<br>Ata da sessão<br>Mapa de lances<br>Documentos de habilitação<br>Recursos e contrarrazões<br>Adjudicação<br>Homologação"]
    
    CL4["Documentos para contratação:<br>Contrato assinado<br>Publicação do extrato<br>Designação de fiscal/gestor<br>Garantia contratual (se exigida)"]
    end
    
    %% Características do Pregão Presencial
    subgraph "Características do Pregão Presencial"
    CP1["Aplicabilidade:<br>Aquisição de bens e serviços comuns<br>Independente do valor estimado<br>Quando justificada a inviabilidade do Pregão Eletrônico"]
    
    CP2["Procedimentos específicos:<br>Inversão de fases (julgamento antes da habilitação)<br>Fase de lances verbais<br>Credenciamento presencial<br>Envelopes físicos de proposta e habilitação"]
    
    CP3["Prazos:<br>Publicação: mínimo 8 dias úteis<br>Recursal: 3 dias úteis<br>Validade das propostas: 60 dias (prorrogável)"]
    end
    
    %% Justificativa para Pregão Presencial
    subgraph "Justificativa para Pregão Presencial"
    JP1["Hipóteses de justificativa:<br>Comprovada inviabilidade técnica<br>Desvantagem para a administração<br>Limitações de mercado local<br>Complexidade do objeto que exija interação presencial"]
    
    JP2["Observação:<br>A Lei 14.133/2021 prioriza o Pregão Eletrônico<br>Pregão Presencial é exceção que deve ser justificada"]
    end
