# Fluxograma da Coordenadoria de Contratos - DAT

```mermaid
flowchart TD
    A["Recebimento do Processo Licitatório Concluído"] --> B["Elaboração da Minuta do Contrato"]
    B --> C["Análise Jurídica da Minuta"]
    C --> D{"Parecer Favorável?"}
    D -->|Não| E["Ajustes na Minuta"]
    E --> C
    D -->|Sim| F["Convocação do Fornecedor"]
    F --> G["Assinatura do Contrato"]
    G --> H["Publicação do Extrato do Contrato"]
    H --> I["Designação de Fiscal e Gestor do Contrato"]
    I --> J["Reunião Inicial com Contratada"]
    J --> K["Início da Execução Contratual"]
    
    K --> L["Acompanhamento da Execução"]
    L --> M["Verificação de Conformidade"]
    M --> N{"Execução Conforme?"}
    N -->|Não| O["Notificação à Contratada"]
    O --> P{"Problema Resolvido?"}
    P -->|Não| Q["Aplicação de Penalidades"]
    Q --> R["Registro no Cadastro de Fornecedores"]
    P -->|Sim| S["Registro da Ocorrência"]
    N -->|Sim| T["Ateste de Serviços/Produtos"]
    S --> T
    R --> T
    
    T --> U["Encaminhamento para Pagamento"]
    U --> V["Controle de Saldos Contratuais"]
    V --> W{"Contrato Próximo do Fim?"}
    W -->|Sim| X["Análise de Necessidade de Prorrogação"]
    X --> Y{"Prorrogação Necessária?"}
    Y -->|Sim| Z["Pesquisa de Preços para Comparação"]
    Z --> AA{"Preços Vantajosos?"}
    AA -->|Sim| AB["Elaboração de Termo Aditivo"]
    AB --> AC["Análise Jurídica do Aditivo"]
    AC --> AD["Assinatura do Termo Aditivo"]
    AD --> AE["Publicação do Extrato do Aditivo"]
    AE --> L
    AA -->|Não| AF["Preparação de Nova Licitação"]
    Y -->|Não| AF
    W -->|Não| L
    
    AF --> AG["Encerramento do Contrato"]
    AG --> AH["Verificação Final de Pendências"]
    AH --> AI["Emissão de Termo de Recebimento Definitivo"]
    AI --> AJ["Liberação de Garantia Contratual"]
    AJ --> AK["Arquivamento do Processo"]
    AK --> AL["Fim do Processo de Gestão Contratual"]
