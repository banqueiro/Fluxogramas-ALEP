```mermaid
flowchart TB
    A[Diretoria de Apoio Técnico] --> Z{{ }}
    A[Diretoria de Apoio Técnico] --> 
    F[Chefia de Gabinete] --> Z{{ }}

    Z --> B[Coordenadoria de Contabilidade]
    Z --> C[Coordenadoria de Contratos]
    Z --> D[Coordenadoria de Suprimentos]
    Z --> E[Coordenadoria de Publicidade]
    
    %% Organiza as coordenadorias em linha
    subgraph Coordenadorias
        direction LR
        B
        C
        D
        E
    end
