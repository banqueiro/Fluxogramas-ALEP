# Fluxograma de Pregão Eletrônico - Lei 14.133/2021

```mermaid
flowchart TD
    %% Início e Diretoria Demandante
    A["Início"] --> B["Diretoria Demandante"]
    B --> C["Elaboração dos documentos essenciais:<br>Justificativa da contratação<br>Objeto claro e preciso<br>Valor estimado<br>Prazo para a execução<br>Indicação da dotação orçamentária"]
    
    %% Fluxo entre departamentos iniciais
    C --> D["DG - Diretoria Geral<br>Recebe o processo"]
    D --> E["Verifica a solicitação<br>Encaminha para DAT"]
    
    %% DAT - Diretoria de Apoio Técnico
    E --> F["DAT - Diretoria de Apoio Técnico<br>Recebe e processa"]
    F --> G["Confere se o objeto é comum<br>Verifica aplicabilidade do Pregão<br>Complementa pesquisa de preços<br>Elabora mapa comparativo"]
    
    %% Verificação de documentação e pesquisa de preços
    G --> H["Realiza pesquisa complementar<br>Compara valores<br>Verifica completude do processo"]
    H --> I["Verifica documentos essenciais:<br>Justificativa da contratação<br>Objeto claro e preciso<br>Valor estimado com pesquisa<br>Prazo para execução<br>Dotação orçamentária"]
    
    %% Elaboração de documentos técnicos
    I --> J["Elabora documentos do Pregão:<br>Termo de Referência detalhado<br>Elabora mapa comparativo<br>Calcula valor médio<br>Verifica disponibilidade orçamentária<br>Elabora minuta do edital<br>Define critérios de julgamento"]
    
    %% Verificação de modalidade
    J --> K["Confirma modalidade Pregão:<br>Verifica se objeto é bem/serviço comum<br>Define modo de disputa (aberto/fechado)<br>Estabelece intervalo mínimo de lances"]
    
    %% Encaminhamento para 1ª SEC
    K --> L["Encaminha processo para 1ª SEC"]
    
    %% 1ª SEC
    L --> M["1ª SEC<br>Recebe e processa"]
    M --> N["Verifica documentação<br>Encaminha para Procuradoria<br>Se necessário, solicita complementação"]
    
    %% Procuradoria
    N --> O["Procuradoria<br>Recebe o processo"]
    O --> P["Analisa parecer jurídico<br>Verifica legalidade do procedimento<br>Encaminha para Controladoria"]
    
    %% Controladoria
    P --> Q["Controladoria<br>Recebe o processo"]
    Q --> R["Analisa legalidade<br>Encaminha para o DG"]
    
    %% Retorno ao DG e Continuidade
    R --> S["DG recebe processo com pareceres"]
    S --> T["Verifica autorização:<br>Analisa pareceres<br>Solicita autorização do Presidente<br>Encaminha para DAT"]
    
    %% Preparação do Edital e Publicação
    T --> U["DAT prepara edital de Pregão:<br>Finaliza o edital<br>Realiza publicação no PNCP e Diário Oficial<br>Marca data da sessão<br>Designa pregoeiro e equipe de apoio"]
    
    %% Sessão Pública do Pregão
    U --> V["Sessão pública do Pregão:<br>Credenciamento no sistema eletrônico<br>Envio de propostas<br>Fase de lances<br>Julgamento<br>Negociação<br>Habilitação"]
    
    %% Adjudicação e Homologação
    V --> W["Adjudicação:<br>Pregoeiro declara vencedor<br>Abre prazo recursal<br>Adjudica objeto (se não houver recurso)"]
    W --> X["Homologação:<br>Autoridade superior analisa processo<br>Solicita homologação do Presidente"]
    
    %% Contratação
    X --> Y["Contrato e empenho:<br>Elabora contrato<br>Convoca para assinatura<br>Emite nota de empenho<br>Publica extrato no PNCP"]
    
    %% Gestão Contratual
    Y --> Z["Gestão do contrato:<br>Designa fiscal e gestor<br>Acompanha execução<br>Realiza pagamentos<br>Verifica cumprimento"]
    
    %% Finalização
    Z --> ZA["Encerramento:<br>Verifica conclusão<br>Emite termo de recebimento<br>Arquiva processo"]
    
    %% Check List Pregão - Lateral
    subgraph "Check List Pregão Eletrônico"
    CL1["Documentos para iniciar processo:<br>Justificativa da contratação<br>Termo de Referência detalhado<br>Pesquisa de preços (mínimo 3 orçamentos)<br>Estudo Técnico Preliminar (ETP)<br>Análise de Riscos"]
    
    CL2["Documentos do Edital:<br>Minuta do Edital<br>Termo de Referência<br>Minuta do Contrato<br>Parecer Jurídico<br>Designação do Pregoeiro<br>Publicações"]
    
    CL3["Documentos da Sessão:<br>Propostas dos licitantes<br>Ata da sessão<br>Documentos de habilitação<br>Recursos e contrarrazões<br>Adjudicação<br>Homologação"]
    
    CL4["Documentos para contratação:<br>Contrato assinado<br>Publicação do extrato<br>Designação de fiscal/gestor<br>Garantia contratual (se exigida)"]
    end
    
    %% Características do Pregão
    subgraph "Características do Pregão Eletrônico"
    CP1["Aplicabilidade:<br>Aquisição de bens e serviços comuns<br>Independente do valor estimado"]
    
    CP2["Procedimentos específicos:<br>Inversão de fases (julgamento antes da habilitação)<br>Fase de lances<br>Modos de disputa: aberto ou aberto e fechado<br>Intervalo mínimo entre lances"]
    
    CP3["Prazos:<br>Publicação: mínimo 8 dias úteis<br>Recursal: 3 dias úteis<br>Validade das propostas: 60 dias (prorrogável)"]
    end
    
    %% Sistemas
    subgraph "Sistemas Eletrônicos"
    SE1["Plataformas:<br>Compras.gov.br<br>BEC<br>Licitações-e (Banco do Brasil)<br>Compras Paraná<br>Outros sistemas homologados"]
    end
