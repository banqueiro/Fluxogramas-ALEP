```mermaid
flowchart TD
    A["Início: Recebimento de processo"] --> B["Receber processo digital (SEI)"]
    B --> C["Autuar / Numerar / Classificar"]
    C --> D["Verificar documentação completa"]
    D --> E{"Completo?"}
    E -->|Não| F["Solicitar complementação / Devolver"]
    E -->|Sim| G["Distribuir / Encaminhar para responsável (Coordenadorias)"]
    G --> H["Acompanhar tramitação (prazo, status no sistema)"]
    H --> I["Gerir fluxo: Alertas de prazo, despachos intermediários"]
    I --> J["Final: Arquivar / Enviar / Encerrar processo"]
