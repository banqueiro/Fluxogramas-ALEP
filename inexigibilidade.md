# Fluxograma de Inexigibilidade de Licitação - Lei 14.133/2021

```mermaid
flowchart TD
    %% Início e Diretoria Demandante
    A["Início"] --> B["Diretoria Demandante"]
    B --> C["Elaboração dos documentos essenciais:<br>Justificativa da contratação<br>Objeto claro e preciso<br>Justificativa da inviabilidade de competição<br>Valor estimado<br>Indicação da dotação orçamentária"]
    
    %% Fluxo entre departamentos iniciais
    C --> D["DG - Diretoria Geral<br>Recebe o processo"]
    D --> E["Verifica a solicitação<br>Encaminha para DAT"]
    
    %% DAT - Diretoria de Apoio Técnico
    E --> F["DAT - Diretoria de Apoio Técnico<br>Recebe e processa"]
    F --> G["Verifica enquadramento na Inexigibilidade:<br>Analisa inviabilidade de competição<br>Verifica documentação comprobatória<br>Analisa justificativa de preço"]
    
    %% Verificação de hipóteses legais
    G --> H{"Enquadramento legal?"}
    H -->|"Fornecedor exclusivo"| I1["Verifica documentação:<br>Atestado de exclusividade<br>Justificativa de preço<br>Comprovação de notória especialização"]
    H -->|"Serviços técnicos com notória especialização"| I2["Verifica documentação:<br>Comprovação de notória especialização<br>Natureza singular do serviço<br>Justificativa de preço<br>Razão da escolha do fornecedor"]
    H -->|"Artista consagrado"| I3["Verifica documentação:<br>Comprovação de consagração<br>Justificativa de preço<br>Contratação direta ou por empresário exclusivo"]
    H -->|"Credenciamento"| I4["Verifica documentação:<br>Justificativa do credenciamento<br>Critérios objetivos<br>Tabela de preços<br>Regulamento do credenciamento"]
    
    %% Consolidação da verificação
    I1 --> J["Consolida verificação"]
    I2 --> J
    I3 --> J
    I4 --> J
    
    %% Verificação de documentação
    J --> K["Verifica documentos essenciais:<br>Justificativa da inviabilidade de competição<br>Documentação comprobatória<br>Justificativa de preço<br>Documentação de habilitação<br>Dotação orçamentária"]
    
    %% Elaboração de documentos técnicos
    K --> L["Elabora documentos da Inexigibilidade:<br>Termo de Referência<br>Justificativa de preço<br>Minuta do contrato<br>Parecer técnico<br>Declaração de inexigibilidade"]
    
    %% Encaminhamento para 1ª SEC
    L --> M["Encaminha processo para 1ª SEC"]
    
    %% 1ª SEC
    M --> N["1ª SEC<br>Recebe e processa"]
    N --> O["Verifica documentação<br>Encaminha para Procuradoria<br>Se necessário, solicita complementação"]
    
    %% Procuradoria
    O --> P["Procuradoria<br>Recebe o processo"]
    P --> Q["Analisa parecer jurídico:<br>Verifica legalidade do procedimento<br>Analisa enquadramento legal<br>Verifica justificativa de preço<br>Encaminha para Controladoria"]
    
    %% Controladoria
    Q --> R["Controladoria<br>Recebe o processo"]
    R --> S["Analisa legalidade<br>Verifica justificativa de preço<br>Encaminha para o DG"]
    
    %% Retorno ao DG e Continuidade
    S --> T["DG recebe processo com pareceres"]
    T --> U["Verifica autorização:<br>Analisa pareceres<br>Solicita autorização do Presidente<br>Encaminha para DAT"]
    
    %% Ratificação e Publicação
    U --> V["DAT prepara Inexigibilidade:<br>Elabora termo de ratificação<br>Realiza publicação no PNCP e Diário Oficial<br>Emite nota de empenho"]
    
    %% Contratação
    V --> W["Contratação:<br>Elabora contrato<br>Convoca para assinatura<br>Publica extrato no PNCP<br>Designa fiscal e gestor"]
    
    %% Gestão Contratual
    W --> X["Gestão do contrato:<br>Acompanha execução<br>Realiza pagamentos<br>Verifica cumprimento<br>Gerencia eventuais alterações"]
    
    %% Finalização
    X --> Y["Encerramento:<br>Verifica conclusão<br>Emite termo de recebimento<br>Arquiva processo"]
    
    %% Check List Inexigibilidade - Lateral
    subgraph "Check List Inexigibilidade"
    CL1["Documentos para iniciar processo:<br>Justificativa da contratação<br>Termo de Referência<br>Justificativa da inviabilidade de competição<br>Documentação comprobatória<br>Justificativa de preço"]
    
    CL2["Documentos específicos por hipótese:<br>Fornecedor exclusivo: atestado de exclusividade<br>Notória especialização: comprovação da especialização<br>Artista: comprovação de consagração<br>Credenciamento: regulamento e critérios objetivos"]
    
    CL3["Documentos da contratação:<br>Termo de Ratificação<br>Publicação no PNCP<br>Contrato assinado<br>Publicação do extrato<br>Nota de empenho<br>Designação de fiscal/gestor"]
    
    CL4["Documentos de habilitação:<br>Regularidade fiscal e trabalhista<br>Qualificação técnica<br>Qualificação econômico-financeira<br>Documentação jurídica"]
    end
    
    %% Características da Inexigibilidade
    subgraph "Características da Inexigibilidade"
    CP1["Hipóteses legais:<br>Fornecedor exclusivo<br>Serviços técnicos com notória especialização<br>Contratação de artista consagrado<br>Credenciamento"]
    
    CP2["Requisitos essenciais:<br>Inviabilidade de competição<br>Justificativa de preço<br>Razão da escolha do fornecedor<br>Documentação comprobatória"]
    
    CP3["Prazos:<br>Publicação: até 10 dias úteis<br>Contrato: conforme necessidade<br>Vigência: conforme objeto"]
    end
    
    %% Justificativa de Preço
    subgraph "Justificativa de Preço"
    JP1["Métodos de comprovação:<br>Contratos similares com outros órgãos<br>Contratos anteriores do mesmo fornecedor<br>Pesquisa de mercado (quando possível)<br>Tabelas oficiais<br>Notas fiscais de outros clientes"]
    end
