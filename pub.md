# Fluxograma de Pagamentos da Publicidade - DAT

```mermaid
flowchart TD
    A["Início do Processo"] --> B["DAT - Publicidade:<br>Fazer Check List no Drive"]
    B --> C{"Documentação<br>adequada?"}
    C -->|Não| D["Enviar para pasta<br>de pendência"]
    D --> B
    C -->|Sim| E["Passar para pasta<br>Notas Protocoladas"]
    E --> F["Abrir processo no SEI<br>conforme Check List"]
    F --> G["Vincular processo de pagamento<br>ao processo do empenho"]
    G --> H["Alimentar planilha de controle"]
    H --> I["Fazer despacho de encaminhamento<br>(Anexo I)"]
    I --> J["Fazer informação certificação<br>(Anexo II)"]
    J --> K["Realizar conferência Administrativa"]
    K --> L["Assinar Despacho e inserir no Bloco"]
    L --> M["Encaminhar para DC/Marketing"]
    
    M --> N["DC - Marketing:<br>Realizar conferência técnica"]
    N --> O["DC - Marketing:<br>Assinar despacho de encaminhamento"]
    O --> P["DAT - Publicidade:<br>Inserir certificação no bloco"]
    P --> Q["Informar Fiscal para assinar o bloco"]
    Q --> R["Informar DC/Comunicação<br>para assinar certificação"]
    
    R --> S["DC:<br>Inserir despacho para contabilidade<br>(Anexo III) no Bloco"]
    S --> T["Diretor assina certificação e<br>despacho para contabilidade"]
    T --> U["Enviar processo para<br>DAT/Contabilidade"]
    
    U --> V["DAT - Coord. de Contabilidade:<br>Elaborar e inserir liquidação no processo"]
    V --> W["Enviar processo para DAT"]
    W --> X["DAT:<br>Enviar processo para DG"]
    
    X --> Y["DG - Diretoria Geral:<br>Verificar requisitos contratuais"]
    Y --> Z["Encaminhar para Diretoria Financeira"]
    
    Z --> AA["DF - Diretoria Financeira:<br>Verificar requisitos contratuais"]
    AA --> AB["Emitir Ordem de Pagamento"]
    AB --> AC["DG - Diretoria Geral:<br>Encaminhar Ordem de Pagamento<br>para autorização"]
    
    AC --> AD["1ª Secretaria / Presidência:<br>Assinar Ordem de Pagamento"]
    AD --> AE["DF - Diretoria Financeira:<br>Realizar pagamento à agência"]
    AE --> AF["Enviar Ordem de Pagamento<br>por e-mail para DAT/Publicidade"]
    
    AF --> AG["DAT - Publicidade:<br>Salvar Ordem de Pagamento<br>no Drive de cada Agência"]
    AG --> AH["Fornecedor:<br>Salvar comprovante de pagamento<br>no Drive (5 dias úteis)"]
    
    AH --> AI["DAT - Publicidade:<br>Conferir comprovante de Pagamento"]
    AI --> AJ["Subir documento no processo SEI"]
    AJ --> AK["Atualizar planilha de Controle"]
    AK --> AL["Finalizar processo no SEI"]
    AL --> AM["Fim do Processo"]
    
    subgraph "Legenda"
    Z1["DAT: Diretoria de Apoio Técnico"]
    Z2["DC: Diretoria de Comunicação"]
    Z3["DG: Diretoria Geral"]
    Z4["DF: Diretoria Financeira"]
    Z5["SEI: Sistema Eletrônico de Informações"]
    end
