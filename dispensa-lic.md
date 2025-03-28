# Fluxograma de Dispensa de Licitação - DAT

```mermaid
flowchart TD
    %% Início do Processo - Diretoria Demandante
    A["Início do Processo"] --> B["Diretoria Demandante: Elaboração dos documentos essenciais"]
    B --> B1["Documentos: Despacho de Solicitação, DFD, ETP, TR, Orçamentos, Aceite Fiscal, Análise de Risco"]
    B1 --> B2["Encaminhar para DG"]
    
    %% Fluxo inicial entre departamentos
    B2 --> C["Diretoria Geral (DG): Verificar solicitação"]
    C --> D["Encaminhar para DAT"]
    C --> E["Encaminhar para DA para abertura do GMS"]
    
    %% Verificação DAT
    D --> F["DAT: Verificar documentação no check list"]
    F --> G{"Documentação completa?"}
    G -->|Não| H["Devolver processo para Diretoria Demandante"]
    H --> B
    G -->|Sim| I["Distribuir para orçamentista"]
    
    %% Orçamentação
    I --> J["DAT - Coord. de Suprimentos/Orçamento: Elaboração do Mapa de Preços"]
    J --> K["Fazer pesquisa de Banco de Preços e Nota Paraná"]
    K --> L["Elaborar despacho"]
    L --> M["Encaminhar para Agente de Contratação para correção"]
    M --> N["Assinar despacho e colocar no Bloco 37"]
    N --> O["Encaminhar para DAT"]
    
    %% Dotação Orçamentária
    O --> P["DAT: Encaminhar para Coord. de Contabilidade"]
    P --> Q["DAT - Coord. de Contabilidade: Incluir dotação orçamentária"]
    Q --> R["Incluir tabela com saldo da dispensa de licitação"]
    R --> S["Solicitar aprovação da declaração de disponibilidade financeira"]
    S --> T["Encaminhar para DAT"]
    
    %% Elaboração da Dispensa
    T --> U["DAT: Encaminhar para Agente de Contratação"]
    U --> V["DAT - Coord. de Suprimentos/Gestão de Contratos: Incluir documentação"]
    V --> V1["Documentos: Certidões, Sanções, Documentos da Empresa, Declaração, Minuta, Justificativa"]
    V1 --> W["Elaborar despacho de dispensa"]
    W --> X["DAT: Encaminhar para DG, Controladoria e Procuradoria"]
    
    %% Análise Jurídica e de Controle
    X --> Y["Procuradoria Geral (PG): Emitir parecer jurídico"]
    Y --> Z["Encaminhar para Controladoria"]
    Z --> AA["Controladoria: Incluir informação"]
    AA --> AB["Encaminhar para DG"]
    
    %% Autorização
    AB --> AC["DG: Encaminhar para autorização da Comissão Executiva"]
    AC --> AD{"Autorizado?"}
    AD -->|Não| AE["Encaminhar para DAT/Contabilidade cancelar dotação"]
    AD -->|Sim| AF["Comissão Executiva: Autorizar prévia o processo para aquisição"]
    AF --> AG["Encaminhar para DAT"]
    
    %% Publicação e Empenho
    AG --> AH["DAT - Coord. de Suprimentos: Publicar extrato da dispensa"]
    AH --> AI["Localizar publicação, salvar em PDF e incluir no SEI"]
    AI --> AJ["DAT - Coord. de Suprimentos: Solicitar empenho"]
    AJ --> AK["DAT - Coord. de Contabilidade: Realizar empenho"]
    AK --> AL["Incluir número do empenho no processo"]
    
    %% Contratação
    AL --> AM{"Há contrato?"}
    AM -->|Não| AN["DAT - Coord. de Suprimentos: Encaminhar OS e nota de empenho para empresa"]
    AM -->|Sim| AO["DAT - Coord. de Suprimentos: Solicitar assinatura do contrato pela empresa"]
    AO --> AP["Encaminhar para assinatura do 1º Secretário"]
    AP --> AQ{"Presidente assina?"}
    AQ -->|Sim| AR["Encaminhar para assinatura do Presidente"]
    AQ -->|Não| AS["Solicitar assinatura das testemunhas"]
    AR --> AS
    
    %% Publicação do Contrato
    AS --> AT["DAT - Coord. de Suprimentos: Verificar se todos assinaram o contrato"]
    AT --> AU["Digitalizar e lançar no SEI"]
    AU --> AV["Elaborar Extrato do Contrato"]
    AV --> AW["Solicitar aprovação da Coord. de Suprimentos"]
    AW --> AX["Enviar para publicação"]
    AX --> AY["Verificar Diário Oficial"]
    AY --> AZ["Localizar publicação, salvar em PDF e incluir no SEI"]
    
    %% Finalização
    AN --> BA["DAT - Coord. de Suprimentos/Administrativo: Incluir no Portal da Transparência e Legix"]
    AZ --> BA
    BA --> BB["Encaminhar processo para Gestão de Contratos"]
    BB --> BC["Informar fiscal do contrato"]
    BC --> BD["Fim do Processo"]
    
    %% Subgráficos simplificados
    subgraph "Check List Inicial"
    CL1["Despacho da diretoria solicitante"]
    CL2["Termo de referência completo"]
    CL3["DFD - Documento de Formalização da Demanda"]
    CL4["ETP - Estudo Técnico Preliminar"]
    CL5["Análise de Risco"]
    CL6["Aceite Fiscal"]
    end
    
    subgraph "Certidões Necessárias"
    CN1["Certidão Registro Cadastral na Alep"]
    CN2["Certificado de regularidade FGTS"]
    CN3["Certidão Negativa da União Federal"]
    CN4["Certidão Negativa Estadual"]
    CN5["Certidão Negativa de Débito Trabalhistas"]
    CN6["Certidão Municipal da cidade sede da empresa"]
    end
    
    subgraph "Prazos Médios"
    PM1["Procuradoria: 1 dia útil"]
    PM2["Controladoria: 2 dias úteis"]
    PM3["Contabilidade (empenho): 1 dia útil"]
    PM4["Total do processo: 5 dias úteis"]
    end
