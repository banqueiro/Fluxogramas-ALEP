```mermaid
flowchart TD
    A["Início: Demanda do Diretor"] --> B["Receber solicitação de assessoria"]
    B --> C["Organizar materiais necessários (documentos, relatórios, dados)"]
    C --> D["Preparar resumo / briefing para o Diretor"]
    D --> E["Apresentar materiais ao Diretor"]
    E --> F{"Aprovado / Necessita ajustes?"}
    F -->|Sim| C
    F -->|Não| G["Final: Material entregue e considerado"]
