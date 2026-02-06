```mermaid
flowchart TD
    A["Início: Início do ciclo anual (ex.: junho/outubro)"] --> B["Solicitar demandas às Diretorias"]
    B --> C["Receber via sistema planejamento de contratações e renovações previstas (objetos, valores, justificativas)"]
    C --> D["Consolidar informações no modelo PCA"]
    D --> E["Analisar compatibilidade com PPA / LDO / Orçamento"]
    E --> F["Elaborar o Plano de Contratações Anual"]
    F --> G["Submeter ao Diretor"]
    G --> H{"Aprovado?"}
    H -->|Não| D
    H -->|Sim| I["Publicar no DIOE ALEP / Portal da Transparência"]
    I --> J["Acompanhar execução / Atualizações mensais se necessário"]
    J --> K["Final: PCA publicado e monitorado"]
