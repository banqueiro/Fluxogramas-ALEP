# Fluxograma de Processo de Pagamentos - Publicidade

```mermaid
flowchart TD
    A["Início do Processo"] --> B["DAT - Publicidade:<br>Verificação Inicial"]
    B --> C["Fazer Check List no Drive"]
    C --> D{"Documentação adequada?"}
    D -->|Não| E["Enviar para pasta de pendência"]
    E --> C
    D -->|Sim| F["Passar para pasta Notas Protocoladas"]
    
    F --> G["DAT - Publicidade:<br>Abertura do Processo"]
    G --> H["Abrir processo no SEI"]
    H --> I["Vincular ao processo do empenho"]
    I --> J["Alimentar planilha de controle"]
    J --> K["Fazer despacho de encaminhamento (Anexo I)"]
    K --> L["Fazer informação certificação (Anexo II)"]
    L --> M["Realizar conferência Administrativa"]
    M --> N["Assinar Despacho e inserir no Bloco"]
    N --> O["Encaminhar para DC/Marketing"]
    
    O --> P["DC - Marketing:<br>Conferência Técnica"]
    P --> Q["Realizar conferência técnica"]
    Q --> R["Assinar despacho de encaminhamento"]
    R --> S["DAT - Publicidade:<br>Continuação do Processo"]
    S --> T["Inserir certificação no bloco"]
    T --> U["Informar Fiscal para assinar o bloco"]
    U --> V["Informar DC/Comunicação para assinar certificação"]
    
    V --> W["DC:<br>Encaminhamento para Contabilidade"]
    W --> X["Inserir despacho para contabilidade (Anexo III)"]
    X --> Y["Diretor assina certificação e despacho"]
    Y --> Z["Enviar processo para DAT/Contabilidade"]
    
    Z --> AA["DAT - Coord. de Contabilidade:<br>Liquidação"]
    AA --> AB["Elaborar e inserir liquidação no processo"]
    AB --> AC["Enviar processo para DAT"]
    
    AC --> AD["DAT:<br>Encaminhamento para DG"]
    AD --> AE["Enviar processo para DG"]
    
    AE --> AF["DG:<br>Verificação e Encaminhamento"]
    AF --> AG["Verificar requisitos contratuais"]
    AG --> AH["Encaminhar para Diretoria Financeira"]
    
    AH --> AI["DF:<br>Emissão de Ordem de Pagamento"]
    AI --> AJ["Verificar requisitos contratuais"]
    AJ --> AK["Emitir Ordem de Pagamento"]
    AK --> AL["DG:<br>Encaminhamento para Autorização"]
    
    AL --> AM["1ª Secretaria / Presidência:<br>Autorização"]
    AM --> AN["Assinar Ordem de Pagamento"]
    
    AN --> AO["DF:<br>Pagamento"]
    AO --> AP["Realizar pagamento à agência"]
    AP --> AQ["Enviar Ordem de Pagamento por e-mail para DAT/Publicidade"]
    
    AQ --> AR["DAT - Publicidade:<br>Registro do Pagamento"]
    AR --> AS["Salvar Ordem de Pagamento no Drive"]
    
    AS --> AT["Fornecedor:<br>Comprovação de Pagamento"]
    AT --> AU["Salvar comprovante de pagamento no Drive (5 dias úteis)"]
    
    AU --> AV["DAT - Publicidade:<br>Finalização do Processo"]
    AV --> AW["Conferir comprovante de Pagamento"]
    AW --> AX["Subir documento no processo SEI"]
    AX --> AY["Atualizar planilha de Controle"]
    AY --> AZ["Finalizar processo no SEI"]
    AZ --> BA["Fim do Processo"]
    
    subgraph "Prazos Médios"
    PM1["Conferência técnica: 1 dia útil"]
    PM2["Liquidação: 1 dia útil"]
    PM3["Autorização: 2 dias úteis"]
    PM4["Pagamento: 1 dia útil"]
    PM5["Total do processo: 10 dias úteis"]
    end
