# Fluxograma de Dispensa de Licitação - DAT

```mermaid
flowchart TD
    %% Início do Processo - Diretoria Demandante
    A["Início do Processo"] --> B["Diretoria Demandante:<br>Elaboração dos documentos essenciais"]
    B --> B1["1. Despacho de Solicitação<br>2. Documento de Formalização da Demanda (DFD)<br>3. Estudo Técnico Preliminar (ETP)<br>4. Termo de Referência (TR)<br>5. Pelo menos 3 orçamentos<br>6. Aceite Fiscal<br>7. Análise de Risco"]
    B1 --> B2["Encaminhar para DG"]
    
    %% Fluxo inicial entre departamentos
    B2 --> C["Diretoria Geral (DG):<br>Verificar solicitação"]
    C --> D["Encaminhar para DAT"]
    C --> E["Encaminhar para DA<br>para abertura do GMS"]
    
    %% Verificação DAT
    D --> F["DAT:<br>Verificar documentação no check list"]
    F --> G{"Documentação<br>completa?"}
    G -->|Não| H["Devolver processo<br>para Diretoria Demandante"]
    H --> B
    G -->|Sim| I["Distribuir para<br>orçamentista"]
    
    %% Orçamentação
    I --> J["DAT - Coord. de Suprimentos/Orçamento:<br>Elaboração do Mapa de Preços"]
    J --> K["Fazer pesquisa de Banco de Preços<br>e Nota Paraná"]
    K --> L["Elaborar despacho"]
    L --> M["Encaminhar para Agente de<br>Contratação para correção"]
    M --> N["Assinar despacho e<br>colocar no Bloco 37"]
    N --> O["Encaminhar para DAT"]
    
    %% Dotação Orçamentária
    O --> P["DAT:<br>Encaminhar para Coord. de Contabilidade"]
    P --> Q["DAT - Coord. de Contabilidade:<br>Incluir dotação orçamentária"]
    Q --> R["Incluir tabela com saldo<br>da dispensa de licitação"]
    R --> S["Solicitar aprovação da declaração<br>de disponibilidade financeira"]
    S --> T["Encaminhar para DAT"]
    
    %% Elaboração da Dispensa
    T --> U["DAT:<br>Encaminhar para Agente de Contratação"]
    U --> V["DAT - Coord. de Suprimentos/Gestão de Contratos:<br>Incluir documentação"]
    V --> V1["1. Certidões (Cadastral, FGTS, Federal,<br>Estadual, Trabalhista, Municipal)<br>2. Sanções Empresa e Sócios<br>3. Documentos da Empresa<br>4. Declaração de Nepotismo<br>5. Minuta do Contrato (se necessário)<br>6. Justificativa e Extrato da Dispensa"]
    V1 --> W["Elaborar despacho de dispensa"]
    W --> X["DAT:<br>Encaminhar para DG, Controladoria e Procuradoria"]
    
    %% Análise Jurídica e de Controle
    X --> Y["Procuradoria Geral (PG):<br>Emitir parecer jurídico"]
    Y --> Z["Encaminhar para Controladoria"]
    Z --> AA["Controladoria:<br>Incluir informação"]
    AA --> AB["Encaminhar para DG"]
    
    %% Autorização
    AB --> AC["DG:<br>Encaminhar para autorização<br>da Comissão Executiva"]
    AC --> AD{"Autorizado?"}
    AD -->|Não| AE["Encaminhar para DAT/Contabilidade<br>cancelar dotação"]
    AD -->|Sim| AF["Comissão Executiva:<br>Autorizar prévia o processo<br>para aquisição"]
    AF --> AG["Encaminhar para DAT"]
    
    %% Publicação e Empenho
    AG --> AH["DAT - Coord. de Suprimentos:<br>Publicar extrato da dispensa"]
    AH --> AI["Localizar publicação,<br>salvar em PDF e incluir no SEI"]
    AI --> AJ["DAT - Coord. de Suprimentos:<br>Solicitar empenho"]
    AJ --> AK["DAT - Coord. de Contabilidade:<br>Realizar empenho"]
    AK --> AL["Incluir número do empenho<br>no processo"]
    
    %% Contratação
    AL --> AM{"Há contrato?"}
    AM -->|Não| AN["DAT - Coord. de Suprimentos:<br>Encaminhar OS e nota de empenho<br>para empresa"]
    AM -->|Sim| AO["DAT - Coord. de Suprimentos:<br>Solicitar assinatura do contrato<br>pela empresa"]
    AO --> AP["Encaminhar para assinatura<br>do 1º Secretário"]
    AP --> AQ{"Presidente<br>assina?"}
    AQ -->|Sim| AR["Encaminhar para<br>assinatura do Presidente"]
    AQ -->|Não| AS["Solicitar assinatura<br>das testemunhas"]
    AR --> AS
    
    %% Publicação do Contrato
    AS --> AT["DAT - Coord. de Suprimentos:<br>Verificar se todos assinaram o contrato"]
    AT --> AU["Digitalizar e lançar no SEI"]
    AU --> AV["Elaborar Extrato do Contrato"]
    AV --> AW["Solicitar aprovação da<br>Coord. de Suprimentos"]
    AW --> AX["Enviar para publicação"]
    AX --> AY["Verificar Diário Oficial"]
    AY --> AZ["Localizar publicação,<br>salvar em PDF e incluir no SEI"]
    
    %% Finalização
    AN --> BA["DAT - Coord. de Suprimentos/Administrativo:<br>Incluir no Portal da Transparência e Legix"]
    AZ --> BA
    BA --> BB["Encaminhar processo para<br>Gestão de Contratos"]
    BB --> BC["Informar fiscal do contrato"]
    BC --> BD["Fim do Processo"]
    
    %% Subgráficos
    subgraph "Check List Inicial"
    CL1["1. Despacho da diretoria solicitante"]
    CL2["2. Termo de referência completo (mínimo 1 orçamento)"]
    CL3["3. DFD - Documento de Formalização da Demanda"]
    CL4["4. ETP - Estudo Técnico Preliminar"]
    CL5["5. Análise de Risco"]
    CL6["6. Aceite Fiscal"]
    end
    
    subgraph "Certidões Necessárias"
    CN1["1. Certidão Registro Cadastral na Alep"]
    CN2["2. Certificado de regularidade FGTS"]
    CN3["3. Certidão Negativa da União Federal"]
    CN4["4. Certidão Negativa Estadual"]
    CN5["5. Certidão Negativa de Débito Trabalhistas"]
    CN6["6. Certidão Municipal da cidade sede da empresa e/ou GMS"]
    end
    
    subgraph "Prazos Médios"
    PM1["Procuradoria: 1 dia útil"]
    PM2["Controladoria: 2 dias úteis"]
    PM3["Contabilidade (empenho): 1 dia útil"]
    PM4["Total do processo: 5 dias úteis"]
    end
