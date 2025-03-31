# Fluxograma de Solicitação/Autorização da Despesa - Publicidade

```mermaid
flowchart TD
    A["Início do Processo"] --> B["Diretoria de Comunicação (DC):<br>Elaboração da Solicitação"]
    B --> C["Elaborar Briefing da Campanha"]
    C --> D["Definir Objetivo da Campanha"]
    D --> E["Estimar Valor da Campanha"]
    E --> F["Encaminhar para DG"]
    
    F --> G["Diretoria Geral (DG):<br>Análise Inicial"]
    G --> H["Verificar Solicitação"]
    H --> I["Encaminhar para DAT"]
    
    I --> J["DAT:<br>Análise Técnica"]
    J --> K["Verificar Disponibilidade Orçamentária"]
    K --> L["Elaborar Despacho Técnico"]
    L --> M["Encaminhar para DG"]
    
    M --> N["DG:<br>Encaminhamento para Autorização"]
    N --> O["Encaminhar para Comissão Executiva"]
    
    O --> P["Comissão Executiva:<br>Análise e Autorização"]
    P --> Q{"Autorizado?"}
    Q -->|Não| R["Devolver com Justificativa"]
    R --> B
    Q -->|Sim| S["Autorizar Campanha"]
    
    S --> T["DG:<br>Encaminhamento para Execução"]
    T --> U["Encaminhar para DC"]
    
    U --> V["DC:<br>Solicitação para Agência"]
    V --> W["Elaborar Ordem de Serviço"]
    W --> X["Encaminhar Briefing para Agência"]
    
    X --> Y["Agência de Publicidade:<br>Desenvolvimento da Campanha"]
    Y --> Z["Elaborar Proposta Criativa"]
    Z --> AA["Elaborar Plano de Mídia"]
    AA --> AB["Apresentar para DC"]
    
    AB --> AC["DC:<br>Análise da Proposta"]
    AC --> AD{"Proposta Aprovada?"}
    AD -->|Não| AE["Solicitar Ajustes"]
    AE --> Y
    AD -->|Sim| AF["Aprovar Campanha"]
    
    AF --> AG["DC:<br>Autorização para Execução"]
    AG --> AH["Emitir Autorização de Veiculação"]
    AH --> AI["Encaminhar para DAT"]
    
    AI --> AJ["DAT:<br>Registro e Controle"]
    AJ --> AK["Registrar Campanha no Sistema"]
    AK --> AL["Atualizar Planilha de Controle"]
    AL --> AM["Fim do Processo de Solicitação"]
    
    subgraph "Observações Importantes"
    OBS1["Recomenda-se prévia confirmação de saldos orçamentário e financeiro"]
    OBS2["Dotação e disponibilidade devem ser confirmadas pela Coord. de Contabilidade"]
    OBS3["Incluir Plano de Mídia atualizado após finalização da Campanha"]
    end
