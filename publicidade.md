# Fluxograma da Coordenadoria de Publicidade - DAT

```mermaid
flowchart TD
    A["Recebimento da Solicitação de Campanha Publicitária"] --> B["Análise da Demanda"]
    B --> C{"Demanda Aprovada?"}
    C -->|Não| D["Devolução com Justificativa"]
    C -->|Sim| E["Verificação de Contrato Vigente"]
    E --> F{"Contrato Vigente?"}
    F -->|Não| G["Iniciar Processo Licitatório"]
    F -->|Sim| H["Emissão de Ordem de Serviço"]
    H --> I["Briefing com Agência"]
    I --> J["Apresentação de Proposta pela Agência"]
    J --> K["Análise da Proposta"]
    K --> L{"Proposta Aprovada?"}
    L -->|Não| M["Solicitação de Ajustes"]
    M --> J
    L -->|Sim| N["Autorização para Execução"]
    N --> O["Acompanhamento da Campanha"]
    O --> P["Entrega dos Serviços"]
    P --> Q["Conferência dos Serviços Entregues"]
    Q --> R{"Serviços Conformes?"}
    R -->|Não| S["Solicitação de Correções"]
    S --> P
    R -->|Sim| T["Recebimento da Nota Fiscal"]
    T --> U["Verificação de Documentação Fiscal"]
    U --> V["Verificação de Regularidade Fiscal"]
    V --> W{"Documentação OK?"}
    W -->|Não| X["Solicitação de Regularização"]
    X --> U
    W -->|Sim| Y["Ateste da Nota Fiscal"]
    Y --> Z["Verificação de Comprovantes de Veiculação"]
    Z --> AA["Análise de Relatórios de Mídia"]
    AA --> AB["Conferência de Valores"]
    AB --> AC["Elaboração de Processo de Pagamento"]
    AC --> AD["Emissão de Nota de Liquidação"]
    AD --> AE["Autorização de Pagamento"]
    AE --> AF["Emissão de Ordem Bancária"]
    AF --> AG["Registro Contábil"]
    AG --> AH["Arquivamento Digital"]
    AH --> AI["Relatório Mensal de Despesas com Publicidade"]
    AI --> AJ["Prestação de Contas Anual de Publicidade"]
    AJ --> AK["Fim do Processo"]
    
    subgraph "Processos Específicos"
    AL["Gestão de Cotas Publicitárias"] --> AM["Controle de Mídia por Veículo"]
    AM --> AN["Análise de Efetividade das Campanhas"]
    end
