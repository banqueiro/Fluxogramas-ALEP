```mermaid
flowchart TD
    A["Início: Necessidade de ato / correspondência"] --> B["Receber minuta ou solicitação"]
    B --> C["Pesquisar base legal / modelo padrão"]
    C --> D["Elaborar o ato normativo ou correspondência (redação)"]
    D --> E["Revisar gramática, formatação e conformidade legal"]
    E --> F["Submeter ao Diretor para assinatura / aprovação"]
    F --> G{"Aprovado?"}
    G -->|Sim| H["Registrar no SEI / Protocolizar / Publicar (se necessário)"]
    G -->|Não| D
    H --> I["Final: Ato / Correspondência emitido"]
