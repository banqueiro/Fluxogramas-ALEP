# Fluxograma da Coordenadoria de Contabilidade - DAT

```mermaid
flowchart LR
    A["Início do Processo Contábil"] --> B["Recebimento de Documentação Fiscal"]
    B --> C["Análise e Classificação Contábil"]
    C --> D["Registro no Sistema Contábil"]
    D --> E{"Documentação Completa?"}
    E -->|Não| F["Solicitar Documentação Complementar"]
    F --> B
    E -->|Sim| G["Elaboração de Relatórios Contábeis"]
    G --> H["Conciliação Bancária"]
    H --> I["Fechamento Mensal"]
    I --> J["Elaboração de Demonstrativos Contábeis"]
    J --> K["Análise de Conformidade"]
    K --> L{"Conformidade OK?"}
    L -->|Não| M["Ajustes Contábeis"]
    M --> K
    L -->|Sim| N["Envio ao Tribunal de Contas"]
    N --> O["Arquivamento Digital"]
    O --> P["Elaboração de Relatórios Gerenciais"]
    P --> Q["Prestação de Contas Anual"]
    Q --> R["Fim do Processo"]
    
    subgraph "Processos Periódicos"
    S["Elaboração da Proposta Orçamentária"] --> T["Acompanhamento da Execução Orçamentária"]
    T --> U["Remanejamentos Orçamentários"]
    U --> V["Suplementações Orçamentárias"]
    end
    
    subgraph "Processos Específicos"
    W["Registro Patrimonial"] --> X["Depreciação de Bens"]
    X --> Y["Inventário Anual"]
    Y --> Z["Baixa de Bens"]
    end

