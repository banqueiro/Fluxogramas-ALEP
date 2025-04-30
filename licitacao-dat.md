# Fluxograma da Coordenadoria de Licitação - DAT

```mermaid
flowchart TD
    %% Fase Preliminar - Diretoria Administrativa
    A["Diretoria Administrativa: Elaboração do DFD - Documento de Formalização de Demanda"] --> B["Diretoria Administrativa: Elaboração do ETP - Estudo Técnico Preliminar"]
    B --> C["Diretoria Administrativa: Elaboração do TR - Termo de Referência"]
    C --> D["Diretoria Administrativa: Coleta de até 3 orçamentos iniciais"]
    D --> E["Envio do processo para DAT"]
    
    %% Fase de Planejamento da Contratação - DAT
    E --> F["DAT: Recebimento e análise inicial do processo"]
    F --> G["DAT: Complementação da pesquisa de preços"]
    G --> H["DAT: Elaboração do Mapa Comparativo de Preços"]
    H --> I["DAT: Cálculo do Valor Estimado da Contratação"]
    I --> J["DAT: Verificação de Disponibilidade Orçamentária"]
    J --> K{"Há Disponibilidade Orçamentária?"}
    K -->|Não| L["Solicitação de Suplementação Orçamentária"]
    L --> M{"Suplementação Aprovada?"}
    M -->|Não| N["Devolução do Processo à Diretoria Administrativa"]
    M -->|Sim| O["DAT: Elaboração da Solicitação de Autorização para Licitar"]
    K -->|Sim| O
    
    %% Fase de Autorização
    O --> P["Encaminhamento para Autorização da Presidência"]
    P --> Q{"Autorizado?"}
    Q -->|Não| N
    Q -->|Sim| R["DAT: Escolha da Modalidade Licitatória"]
    
    %% Fase de Seleção da Modalidade
    R --> S{"Qual Modalidade?"}
    S -->|"Pregão Eletrônico"| T1["Elaboração do Edital de Pregão"]
    S -->|"Concorrência"| T2["Elaboração do Edital de Concorrência"]
    S -->|"Concurso"| T3["Elaboração do Edital de Concurso"]
    S -->|"Leilão"| T4["Elaboração do Edital de Leilão"]
    S -->|"Diálogo Competitivo"| T5["Elaboração do Edital de Diálogo Competitivo"]
    S -->|"Contratação Direta"| T6["Elaboração do Processo de Contratação Direta"]
    
    %% Unificação após escolha da modalidade
    T1 & T2 & T3 & T4 & T5 --> U["DAT: Elaboração da Minuta do Edital e Anexos"]
    T6 --> U1["DAT: Elaboração da Justificativa de Contratação Direta"]
    U1 --> V
    
    %% Fase de Análise Jurídica
    U --> V["Encaminhamento para Procuradoria Análise Jurídica"]
    V --> W{"Parecer Jurídico Favorável?"}
    W -->|Não| X["Ajustes na Minuta do Edital"]
    X --> V
    W -->|Sim| Y["DAT: Publicação do Edital ou Aviso de Dispensa Eletrônica"]
    
    %% Fase de Publicação e Divulgação
    Y --> Z["Publicação no Diário Oficial"]
    Z --> AA["Publicação no Portal Nacional de Contratações Públicas - PNCP"]
    AA --> AB["Publicação no Site da Assembleia Legislativa"]
    AB --> AC["Período para Impugnações e Pedidos de Esclarecimentos"]
    AC --> AD{"Houve Impugnações/Esclarecimentos?"}
    AD -->|Sim| AE["Análise e Resposta às Impugnações/Esclarecimentos"]
    AE --> AF{"Necessita Alterar Edital?"}
    AF -->|Sim| AG["Alteração do Edital"]
    AG --> AH["Republicação do Edital"]
    AH --> AI["Reabertura de Prazos"]
    AI --> AJ["Sessão Pública"]
    AF -->|Não| AJ
    AD -->|Não| AJ
    
    %% Fase de Sessão Pública
    AJ --> AK["Credenciamento dos Licitantes"]
    AK --> AL["Abertura das Propostas"]
    AL --> AM["Verificação de Conformidade das Propostas"]
    AM --> AN["Fase de Lances (se Pregão)"]
    AN --> AO["Julgamento das Propostas"]
    AO --> AP["Verificação de Efetividade da Proposta"]
    AP --> AQ["Negociação com o Primeiro Colocado"]
    AQ --> AR["Habilitação do Licitante"]
    AR --> AS{"Licitante Habilitado?"}
    AS -->|Não| AT["Convocação do Próximo Licitante"]
    AT --> AQ
    AS -->|Sim| AU["Declaração do Vencedor"]
    
    %% Fase Recursal
    AU --> AV["Abertura de Prazo Recursal"]
    AV --> AW{"Houve Recursos?"}
    AW -->|Sim| AX["Análise dos Recursos"]
    AX --> AY{"Recurso Procedente?"}
    AY -->|Sim| AZ["Retorno à Fase Apropriada"]
    AZ --> BA["Continuidade do Processo"]
    BA --> AU
    AY -->|Não| BB["Manutenção da Decisão"]
    BB --> BC["Adjudicação do Objeto"]
    AW -->|Não| BC
    
    %% Fase de Homologação e Contratação
    BC --> BD["Elaboração do Relatório Final"]
    BD --> BE["Encaminhamento para Homologação"]
    BE --> BF{"Homologado?"}
    BF -->|Não| BG["Revogação ou Anulação da Licitação"]
    BF -->|Sim| BH["Publicação do Resultado"]
    BH --> BI["Convocação do Licitante para Assinatura do Contrato"]
    BI --> BJ["Assinatura do Contrato"]
    BJ --> BK["Publicação do Extrato do Contrato"]
    BK --> BL["Emissão de Nota de Empenho"]
    BL --> BM["Designação de Gestor e Fiscal do Contrato"]
    BM --> BN["Encaminhamento para Gestão de Contratos"]
    BN --> BO["Fim do Processo Licitatório"]
    
    %% Subgráfico para Modalidades Específicas
    subgraph "Modalidades da Lei 14.133/2021"
    CA["Pregão Eletrônico: Bens e Serviços Comuns"]
    CB["Concorrência: Obras, Serviços de Engenharia Especiais, Bens e Serviços Especiais"]
    CC["Concurso: Serviços Técnicos, Científicos ou Artísticos"]
    CD["Leilão: Alienação de Bens"]
    CE["Diálogo Competitivo: Inovação, Adaptação ou Complexidade Técnica"]
    CF["Contratação Direta: Dispensa ou Inexigibilidade"]
    end
    
    %% Subgráfico para Processos Específicos
    subgraph "Processos Específicos"
    DA["Gestão de Riscos"] --> DB["Análise de Conformidade"]
    DB --> DC["Portal Nacional de Contratações Públicas"]
    DC --> DD["Gestão por Competências"]
    end
