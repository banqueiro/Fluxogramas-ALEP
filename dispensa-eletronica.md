# Fluxograma de Dispensa Eletrônica - Lei 14.133/2021

```mermaid
flowchart TD
    %% Início e Diretoria Demandante
    A["Início"] --> B["Diretoria Demandante"]
    B --> C["Elaboração dos documentos essenciais:<br>Justificativa da contratação<br>Objeto claro e preciso<br>Valor estimado<br>Enquadramento na hipótese de dispensa<br>Indicação da dotação orçamentária"]
    
    %% Fluxo entre departamentos iniciais
    C --> D["DG - Diretoria Geral<br>Recebe o processo"]
    D --> E["Verifica a solicitação<br>Encaminha para DAT"]
    
    %% DAT - Diretoria de Apoio Técnico
    E --> F["DAT - Diretoria de Apoio Técnico<br>Recebe e processa"]
    F --> G["Verifica enquadramento na Dispensa:<br>Analisa valor (dentro dos limites)<br>Verifica pesquisa de preços<br>Confirma possibilidade de dispensa eletrônica"]
    
    %% Verificação de hipóteses legais
    G --> H{"Enquadramento legal?"}
    H -->|"Dispensa por valor"| I1["Verifica limites:<br>Obras e serviços de engenharia: até R$ 100.000,00<br>Outros serviços e compras: até R$ 50.000,00"]
    H -->|"Outras hipóteses de dispensa"| I2["Verifica enquadramento:<br>Licitação deserta/fracassada<br>Emergência/calamidade<br>Outras hipóteses do art. 75"]
    
    %% Consolidação da verificação
    I1 --> J["Consolida verificação"]
    I2 --> J
    
    %% Verificação de documentação
    J --> K["Verifica documentos essenciais:<br>Justificativa da contratação<br>Termo de Referência simplificado<br>Pesquisa de preços<br>Enquadramento legal<br>Dotação orçamentária"]
    
    %% Elaboração de documentos técnicos
    K --> L["Elabora documentos da Dispensa Eletrônica:<br>Termo de Referência<br>Aviso de Dispensa Eletrônica<br>Minuta do contrato (se necessário)<br>Declaração de dispensa"]
    
    %% Encaminhamento para 1ª SEC
    L --> M["Encaminha processo para 1ª SEC"]
    
    %% 1ª SEC
    M --> N["1ª SEC<br>Recebe e processa"]
    N --> O["Verifica documentação<br>Encaminha para Procuradoria<br>Se necessário, solicita complementação"]
    
    %% Procuradoria
    O --> P["Procuradoria<br>Recebe o processo"]
    P --> Q["Analisa parecer jurídico:<br>Verifica legalidade do procedimento<br>Analisa enquadramento legal<br>Verifica minuta do contrato (se houver)<br>Encaminha para Controladoria"]
    
    %% Controladoria
    Q --> R["Controladoria<br>Recebe o processo"]
    R --> S["Analisa legalidade<br>Verifica pesquisa de preços<br>Encaminha para o DG"]
    
    %% Retorno ao DG e Continuidade
    S --> T["DG recebe processo com pareceres"]
    T --> U["Verifica autorização:<br>Analisa pareceres<br>Solicita autorização do Presidente<br>Encaminha para DAT"]
    
    %% Publicação do Aviso
    U --> V["DAT prepara Dispensa Eletrônica:<br>Finaliza o Aviso de Dispensa<br>Publica no PNCP<br>Cadastra no sistema eletrônico<br>Define data da sessão eletrônica"]
    
    %% Realização da Dispensa Eletrônica
    V --> W["Realização da Dispensa Eletrônica:<br>Abertura da sessão no sistema<br>Envio de lances pelos fornecedores<br>Julgamento automático (menor preço)<br>Verificação da proposta mais vantajosa"]
    
    %% Habilitação e Adjudicação
    W --> X["Habilitação e Adjudicação:<br>Verifica documentação do fornecedor<br>Analisa proposta final<br>Negocia condições (se necessário)<br>Adjudica objeto"]
    
    %% Homologação
    X --> Y["Homologação:<br>Autoridade superior analisa processo<br>Homologa resultado<br>Autoriza emissão de empenho"]
    
    %% Contratação
    Y --> Z["Contratação:<br>Emite nota de empenho<br>Elabora contrato (se necessário)<br>Convoca para assinatura<br>Publica extrato no PNCP"]
    
    %% Gestão Contratual
    Z --> ZA["Gestão do contrato:<br>Designa fiscal e gestor<br>Acompanha execução<br>Realiza pagamentos<br>Verifica cumprimento"]
    
    %% Finalização
    ZA --> ZB["Encerramento:<br>Verifica conclusão<br>Emite termo de recebimento<br>Arquiva processo"]
    
    %% Check List Dispensa Eletrônica - Lateral
    subgraph "Check List Dispensa Eletrônica"
    CL1["Documentos para iniciar processo:<br>Justificativa da contratação<br>Termo de Referência simplificado<br>Pesquisa de preços<br>Enquadramento legal<br>Dotação orçamentária"]
    
    CL2["Documentos da Dispensa:<br>Aviso de Dispensa Eletrônica<br>Termo de Referência<br>Minuta do contrato (se necessário)<br>Parecer Jurídico<br>Publicação no PNCP"]
    
    CL3["Documentos da sessão eletrônica:<br>Propostas dos fornecedores<br>Lances ofertados<br>Ata da sessão<br>Documentos de habilitação<br>Adjudicação<br>Homologação"]
    
    CL4["Documentos da contratação:<br>Nota de empenho<br>Contrato (se necessário)<br>Publicação do extrato<br>Designação de fiscal/gestor<br>Ordem de fornecimento"]
    end
    
    %% Características da Dispensa Eletrônica
    subgraph "Características da Dispensa Eletrônica"
    CP1["Aplicabilidade:<br>Dispensa por valor<br>Outras hipóteses de dispensa (quando possível)<br>Compras e serviços comuns"]
    
    CP2["Particularidades:<br>Realizada em sistema eletrônico<br>Disputa aberta entre fornecedores<br>Julgamento automático<br>Maior transparência e competitividade"]
    
    CP3["Prazos:<br>Publicação: mínimo 3 dias úteis<br>Sessão: conforme aviso<br>Contratação: imediata após homologação"]
    end
    
    %% Sistemas Eletrônicos
    subgraph "Sistemas Eletrônicos"
    SE1["Plataformas:<br>Compras.gov.br<br>BEC<br>Licitações-e (Banco do Brasil)<br>Compras Paraná<br>Outros sistemas homologados"]
    end
