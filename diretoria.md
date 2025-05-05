```mermaid

graph TD
    A[Diretoria de Apoio Técnico<br>Dirige e controla serviços técnicos, administrativos e licitatórios] --> B[Diretor de Apoio Técnico]

    subgraph DiretorFuncoes
        B --> B1[Acompanhar licitações e realizar compras]
        B --> B2[Acompanhar dispensa/inexigibilidade e realizar compras]
        B --> B3[Acompanhar saldos, aditivos e liquidar despesas]
    end

    B --> C[Coordenadoria-Geral]
    B --> D[Coordenadoria de Suprimentos]
    B --> E[Coordenadoria Administrativa de Contratos]
    B --> F[Coordenadoria Administrativa de Publicidade]
    B --> G[Coordenadoria de Contabilidade]

    subgraph CoordGeral
        C --> C1[Assessorar Diretor<br>Organizar materiais]
        C --> C2[Coordenar servidores]
        C --> C3[Elaborar atos normativos]
        C --> C4[Gerir fluxo de processos]
    end

    subgraph CoordSuprimentos
        D --> D1[Organizar compras e aquisições]
        D --> D2[Acompanhar licitações e compras]
        D --> D3[Acompanhar dispensa/inexigibilidade]
        D --> D4[Elaborar aditivos contratuais]
        D --> D5[Manter cadastro de fornecedores]
        D --> D6[Atender processos de licitações]
    end

    subgraph CoordContratos
        E --> E1[Controlar saldos e vigências]
        E --> E2[Emitir ordens e empenhos]
        E --> E3[Enviar notificações e sanções]
        E --> E4[Verificar regularidade fiscal]
        E --> E5[Analisar repactuação/reequilíbrio]
        E --> E6[Controlar avisos de vencimento]
    end

    subgraph CoordPublicidade
        F --> F1[Mapear gestão de publicidade]
        F --> F2[Providenciar ordens via sistema]
        F --> F3[Controlar pagamentos]
        F --> F4[Encaminhar aditivos à Diretoria de Comunicação]
        F --> F5[Relatórios para Portal da Transparência]
    end

    subgraph CoordContabilidade
        G --> G1[Registrar operações contábeis]
        G --> G2[Elaborar prestação de contas]
        G --> G3[Confeccionar remanejamento orçamentário]
        G --> G4[Registrar empenhos e liquidações]
        G --> G5[Controlar execução orçamentária]
    end

    D -->|Aditivos| E
    E -->|Empenhos| G
    F -->|Pagamentos| G
    F -->|Aditivos/Relatórios| H[Diretoria de Comunicação]

    classDef default fill:#e6f3ff,stroke:#333,stroke-width:1px;
    classDef diretor fill:#b3d9ff,stroke:#333,stroke-width:1px;
    classDef coord fill:#99ccff,stroke:#333,stroke-width:1px;

    class A,B diretor
    class C,D,E,F,G coord
