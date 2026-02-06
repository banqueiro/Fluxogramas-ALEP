```mermaid
flowchart TB
    A[Diretoria de Apoio Técnico] --> Z{{ }}
    A[Diretoria de Apoio Técnico] --> 
    F[Chefia de Gabinete] --> Z{{ }}

    Z --> B[Coordenadoria de Contratos]
    Z --> C[Coordenadoria de Suprimentos]
    Z --> D[Coordenadoria de Publicidade]
    
    %% Organiza as coordenadorias em linha
    subgraph Coordenadorias
        direction LR
        B
        C
        D
        
    end
