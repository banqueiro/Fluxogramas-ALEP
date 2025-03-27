# Fluxograma de Sistema de Registro de Preços - Lei 14.133/2021

```mermaid
flowchart TD
    %% Início e Diretoria Demandante
    A["Início"] --> B["Diretoria Demandante"]
    B --> C["Elaboração dos documentos essenciais:<br>Justificativa para adoção do SRP<br>Objeto claro e preciso<br>Estimativa de quantidades<br>Previsão de aquisições frequentes<br>Indicação da dotação orçamentária"]
    
    %% Fluxo entre departamentos iniciais
    C --> D["DG - Diretoria Geral<br>Recebe o processo"]
    D --> E["Verifica a solicitação<br>Encaminha para DAT"]
    
    %% DAT - Diretoria de Apoio Técnico
    E --> F["DAT - Diretoria de Apoio Técnico<br>Recebe e processa"]
    F --> G["Verifica adequação ao SRP:<br>Confirma aquisições frequentes<br>Verifica impossibilidade de definição prévia do quantitativo<br>Analisa vantajosidade do SRP"]
    
    %% Verificação de documentação e pesquisa de preços
    G --> H["Realiza pesquisa de preços<br>Elabora mapa comparativo<br>Verifica completude do processo"]
    H --> I["Verifica documentos essenciais:<br>Justificativa para adoção do SRP<br>Termo de Referência<br>Estimativa de quantidades<br>Pesquisa de preços<br>Dotação orçamentária"]
    
    %% Elaboração de documentos técnicos
    I --> J["Elabora documentos do SRP:<br>Intenção de Registro de Preços (IRP)<br>Termo de Referência detalhado<br>Minuta da Ata de Registro de Preços<br>Elabora minuta do edital<br>Define critérios de julgamento"]
    
    %% Divulgação da IRP
    J --> K["Divulga Intenção de Registro de Preços:<br>Publica IRP no PNCP<br>Estabelece prazo para manifestação<br>Recebe manifestações de interesse<br>Consolida demandas"]
    
    %% Encaminhamento para 1ª SEC
    K --> L["Encaminha processo para 1ª SEC"]
    
    %% 1ª SEC
    L --> M["1ª SEC<br>Recebe e processa"]
    M --> N["Verifica documentação<br>Encaminha para Procuradoria<br>Se necessário, solicita complementação"]
    
    %% Procuradoria
    N --> O["Procuradoria<br>Recebe o processo"]
    O --> P["Analisa parecer jurídico<br>Verifica legalidade do procedimento<br>Analisa minuta da Ata de RP<br>Encaminha para Controladoria"]
    
    %% Controladoria
    P --> Q["Controladoria<br>Recebe o processo"]
    Q --> R["Analisa legalidade<br>Encaminha para o DG"]
    
    %% Retorno ao DG e Continuidade
    R --> S["DG recebe processo com pareceres"]
    S --> T["Verifica autorização:<br>Analisa pareceres<br>Solicita autorização do Presidente<br>Encaminha para DAT"]
    
    %% Preparação do Edital e Publicação
    T --> U["DAT prepara edital do SRP:<br>Finaliza o edital<br>Realiza publicação no PNCP e Diário Oficial<br>Define modalidade (geralmente Pregão)<br>Designa pregoeiro/comissão"]
    
    %% Realização da Licitação
    U --> V["Realização da licitação para SRP:<br>Segue procedimento da modalidade escolhida<br>(geralmente Pregão Eletrônico)<br>Julgamento das propostas<br>Habilitação<br>Declaração do vencedor"]
    
    %% Adjudicação e Homologação
    V --> W["Adjudicação:<br>Pregoeiro/comissão declara vencedor<br>Abre prazo recursal<br>Adjudica objeto após recursos"]
    W --> X["Homologação:<br>Autoridade superior analisa processo<br>Solicita homologação do Presidente"]
    
    %% Assinatura da Ata de Registro de Preços
    X --> Y["Assinatura da Ata de RP:<br>Elabora Ata de Registro de Preços<br>Convoca fornecedores para assinatura<br>Publica extrato no PNCP<br>Cadastra preços registrados"]
    
    %% Gestão da Ata
    Y --> Z["Gestão da Ata de RP:<br>Designa gestor da Ata<br>Controla saldos e quantitativos<br>Gerencia adesões (se permitido)<br>Negocia eventuais reequilíbrios"]
    
    %% Contratações decorrentes
    Z --> ZA["Contratações decorrentes:<br>Verifica necessidade de contratação<br>Emite nota de empenho<br>Formaliza contrato (se necessário)<br>Designa fiscal e gestor"]
    
    %% Finalização
    ZA --> ZB["Encerramento da Ata:<br>Verifica vigência (máximo 1 ano)<br>Elabora relatório final<br>Arquiva processo"]
    
    %% Check List SRP - Lateral
    subgraph "Check List Sistema de Registro de Preços"
    CL1["Documentos para iniciar processo:<br>Justificativa para adoção do SRP<br>Termo de Referência<br>Estimativa de quantidades<br>Pesquisa de preços<br>Estudo Técnico Preliminar (ETP)"]
    
    CL2["Documentos da IRP:<br>Intenção de Registro de Preços<br>Manifestações de interesse<br>Consolidação das demandas<br>Termo de Referência atualizado"]
    
    CL3["Documentos do Edital:<br>Minuta do Edital<br>Termo de Referência<br>Minuta da Ata de Registro de Preços<br>Parecer Jurídico<br>Publicações"]
    
    CL4["Documentos da Ata de RP:<br>Ata de Registro de Preços assinada<br>Publicação do extrato<br>Designação de gestor<br>Cadastro de preços registrados"]
    
    CL5["Documentos para contratações:<br>Nota de empenho<br>Contrato (se necessário)<br>Designação de fiscal/gestor<br>Ordem de fornecimento"]
    end
    
    %% Características do SRP
    subgraph "Características do Sistema de Registro de Preços"
    CP1["Aplicabilidade:<br>Contratações frequentes<br>Entregas parceladas<br>Atendimento a mais de um órgão<br>Impossibilidade de definição prévia do quantitativo<br>Bens e serviços padronizados"]
    
    CP2["Vantagens:<br>Não obrigatoriedade de contratação<br>Redução de estoques<br>Redução do número de licitações<br>Economia de escala<br>Possibilidade de adesão por outros órgãos"]
    
    CP3["Prazos:<br>Vigência da Ata: máximo 1 ano<br>IRP: mínimo 8 dias úteis<br>Demais prazos: conforme modalidade adotada"]
    end
    
    %% Adesão à Ata (Carona)
    subgraph "Adesão à Ata (Carona)"
    AA1["Requisitos para adesão:<br>Previsão no edital<br>Vantajosidade comprovada<br>Anuência do órgão gerenciador<br>Aceitação do fornecedor<br>Limite de 50% do quantitativo registrado"]
    
    AA2["Procedimento:<br>Solicitação ao órgão gerenciador<br>Consulta ao fornecedor<br>Comprovação de vantajosidade<br>Emissão de nota de empenho<br>Formalização de contrato (se necessário)"]
    end
