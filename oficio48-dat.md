```mermaid
flowchart LR

    %% Diretoria
    A[Diretoria de Apoio Técnico] --> B[Diretor de Apoio Técnico]

    %% Setores subordinados
    B --> C[Chefia de Gabinete]
    B --> D[Coordenadoria de Compras Públicas]
    B --> E[Coordenadoria de Gestão de Contratos]
    B --> F[Coordenadoria de Contratos de Publicidade Institucional]


    %% Chefia de Gabinete
    subgraph CG[Chefia de Gabinete]
        C --> C1[Assessorar diretor]
        C --> C2[Elaborar atos e correspondencias]
        C --> C3[Gerenciar processos]
        C --> C4[Administrar sistemas]
        C --> C5[Plano de Contratacao Anual]
        C --> C6[Atividades correlatas]
    end


    %% Compras Públicas
    subgraph CP[Compras Publicas]
        D --> D1[Organizar solicitacoes de compras]
        D --> D2[Acompanhar licitacoes]
        D --> D3[Dispensa e inexigibilidade]
        D --> D4[Aditivos contratuais]
        D --> D5[Informacoes de licitacoes]
    end


    %% Gestão de Contratos
    subgraph GC[Gestao de Contratos]
        E --> E1[Controlar saldos e vigencias]
        E --> E2[Emitir ordens e empenhos]
        E --> E3[Notificacoes e multas]
        E --> E4[Regularidade fiscal]
        E --> E5[Repactuacao e reequilibrio]
        E --> E6[Pagamentos]
        E --> E7[Vencimentos contratuais]
    end


    %% Publicidade
    subgraph PI[Publicidade Institucional]
        F --> F1[Padronizar procedimentos]
        F --> F2[Ordens e atestados]
        F --> F3[Pagamentos publicidade]
        F --> F4[Aditivos publicidade]
        F --> F5[Relatorios transparencia]
        F --> F6[Demandas administrativas]
    end


    %% Relacoes operacionais
    D -->|gera contrato| E
    E -->|servicos publicidade| F
    F -->|relatorios| G[Portal da Transparencia]
