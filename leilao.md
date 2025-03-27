# Fluxograma de Leilão - Lei 14.133/2021

```mermaid
flowchart TD
    %% Início e Diretoria Demandante
    A["Início"] --> B["Diretoria Demandante"]
    B --> C["Elaboração dos documentos essenciais:<br>Justificativa da alienação<br>Relação dos bens a serem leiloados<br>Avaliação prévia<br>Valor mínimo de arrematação<br>Indicação da dotação orçamentária (se houver custos)"]
    
    %% Fluxo entre departamentos iniciais
    C --> D["DG - Diretoria Geral<br>Recebe o processo"]
    D --> E["Verifica a solicitação<br>Encaminha para DAT"]
    
    %% DAT - Diretoria de Apoio Técnico
    E --> F["DAT - Diretoria de Apoio Técnico<br>Recebe e processa"]
    F --> G["Verifica natureza dos bens<br>Confirma aplicabilidade do Leilão<br>Verifica avaliação prévia<br>Elabora estimativa de custos do leilão"]
    
    %% Verificação de documentação
    G --> H["Analisa documentação dos bens<br>Verifica situação patrimonial<br>Verifica completude do processo"]
    H --> I["Verifica documentos essenciais:<br>Justificativa da alienação<br>Laudo de avaliação dos bens<br>Documentação de propriedade<br>Declaração de desafetação (se bem público)<br>Autorização legislativa (se imóvel)"]
    
    %% Elaboração de documentos técnicos
    I --> J["Elabora documentos do Leilão:<br>Relação detalhada dos bens<br>Valor mínimo de arrematação<br>Condições de pagamento<br>Verifica disponibilidade orçamentária para custos<br>Elabora minuta do edital<br>Define condições de visitação"]
    
    %% Verificação de modalidade
    J --> K["Confirma modalidade Leilão:<br>Verifica se objeto é alienação de bens móveis ou imóveis<br>Define critério de julgamento (maior lance)<br>Estabelece regras para leiloeiro"]
    
    %% Encaminhamento para 1ª SEC
    K --> L["Encaminha processo para 1ª SEC"]
    
    %% 1ª SEC
    L --> M["1ª SEC<br>Recebe e processa"]
    M --> N["Verifica documentação<br>Encaminha para Procuradoria<br>Se necessário, solicita complementação"]
    
    %% Procuradoria
    N --> O["Procuradoria<br>Recebe o processo"]
    O --> P["Analisa parecer jurídico<br>Verifica legalidade do procedimento<br>Analisa documentação de propriedade<br>Encaminha para Controladoria"]
    
    %% Controladoria
    P --> Q["Controladoria<br>Recebe o processo"]
    Q --> R["Analisa legalidade<br>Verifica baixa patrimonial<br>Encaminha para o DG"]
    
    %% Retorno ao DG e Continuidade
    R --> S["DG recebe processo com pareceres"]
    S --> T["Verifica autorização:<br>Analisa pareceres<br>Solicita autorização do Presidente<br>Encaminha para DAT"]
    
    %% Preparação do Edital e Publicação
    T --> U["DAT prepara edital de Leilão:<br>Finaliza o edital<br>Realiza publicação no PNCP e Diário Oficial<br>Designa leiloeiro<br>Estabelece data, horário e local do leilão<br>Organiza visitação dos bens"]
    
    %% Realização do Leilão
    U --> V["Realização do Leilão:<br>Credenciamento dos interessados<br>Apresentação dos bens<br>Lances sucessivos<br>Arrematação pelo maior lance<br>Lavratura da ata"]
    
    %% Homologação e Pagamento
    V --> W["Homologação do resultado:<br>Leiloeiro apresenta resultado<br>Autoridade homologa resultado"]
    W --> X["Pagamento e transferência:<br>Arrematante efetua pagamento<br>Emissão de recibo/nota de venda<br>Transferência da propriedade<br>Baixa patrimonial"]
    
    %% Prestação de Contas
    X --> Y["Prestação de contas:<br>Leiloeiro apresenta prestação de contas<br>Verificação dos valores arrecadados<br>Pagamento de custas e comissão do leiloeiro<br>Recolhimento dos valores aos cofres públicos"]
    
    %% Finalização
    Y --> Z["Encerramento:<br>Verifica conclusão<br>Emite relatório final<br>Arquiva processo"]
    
    %% Check List Leilão - Lateral
    subgraph "Check List Leilão"
    CL1["Documentos para iniciar processo:<br>Justificativa da alienação<br>Relação dos bens<br>Laudo de avaliação<br>Documentação de propriedade<br>Autorização legislativa (se imóvel)<br>Declaração de desafetação (se necessário)"]
    
    CL2["Documentos do Edital:<br>Minuta do Edital<br>Relação e descrição dos bens<br>Valor mínimo de arrematação<br>Condições de pagamento<br>Designação do leiloeiro<br>Parecer Jurídico<br>Publicações"]
    
    CL3["Documentos da Realização:<br>Credenciamento dos participantes<br>Ata do leilão<br>Termo de arrematação<br>Comprovante de pagamento<br>Recibo/nota de venda<br>Homologação"]
    
    CL4["Documentos para encerramento:<br>Termo de transferência de propriedade<br>Baixa patrimonial<br>Prestação de contas do leiloeiro<br>Comprovante de recolhimento dos valores<br>Relatório final"]
    end
    
    %% Características do Leilão
    subgraph "Características do Leilão"
    CP1["Aplicabilidade:<br>Alienação de bens móveis inservíveis<br>Alienação de bens imóveis<br>Produtos legalmente apreendidos<br>Bens penhorados<br>Semoventes"]
    
    CP2["Particularidades:<br>Julgamento por maior lance<br>Lances sucessivos<br>Possibilidade de leilão eletrônico<br>Pagamento à vista ou parcelado"]
    
    CP3["Prazos:<br>Publicação: mínimo 15 dias úteis<br>Visitação: conforme edital<br>Pagamento: conforme edital"]
    end
    
    %% Leiloeiro
    subgraph "Leiloeiro"
    LE1["Tipos de leiloeiro:<br>Servidor designado pela Administração<br>Leiloeiro oficial contratado<br>Leiloeiro administrativo"]
    
    LE2["Remuneração:<br>Comissão paga pelo arrematante<br>Percentual conforme legislação<br>Reembolso de despesas (se previsto)"]
    end
