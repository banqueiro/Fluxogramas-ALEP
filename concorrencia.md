
### 2. concorrencia.md

```markdown
# Fluxograma de Concorrência - Lei 14.133/2021

```mermaid
flowchart TD
    %% Início e Diretoria Demandante
    A["Início"] --> B["Diretoria Demandante"]
    B --> C["Elaboração dos documentos essenciais:<br>Justificativa da contratação<br>Objeto detalhado<br>Valor estimado<br>Prazo para a execução<br>Indicação da dotação orçamentária<br>Projeto Básico/Executivo (se obra)"]
    
    %% Fluxo entre departamentos iniciais
    C --> D["DG - Diretoria Geral<br>Recebe o processo"]
    D --> E["Verifica a solicitação<br>Encaminha para DAT"]
    
    %% DAT - Diretoria de Apoio Técnico
    E --> F["DAT - Diretoria de Apoio Técnico<br>Recebe e processa"]
    F --> G["Verifica complexidade do objeto<br>Confirma aplicabilidade da Concorrência<br>Complementa pesquisa de preços<br>Elabora mapa comparativo"]
    
    %% Verificação de documentação e pesquisa de preços
    G --> H["Realiza pesquisa complementar<br>Compara valores<br>Verifica completude do processo"]
    H --> I["Verifica documentos essenciais:<br>Justificativa da contratação<br>Projeto Básico/Executivo<br>Valor estimado com orçamento detalhado<br>Cronograma físico-financeiro<br>Dotação orçamentária"]
    
    %% Elaboração de documentos técnicos
    I --> J["Elabora documentos da Concorrência:<br>Projeto Básico/Executivo detalhado<br>Planilha orçamentária<br>Cronograma físico-financeiro<br>Verifica disponibilidade orçamentária<br>Elabora minuta do edital<br>Define critérios de julgamento e habilitação"]
    
    %% Verificação de modalidade
    J --> K["Confirma modalidade Concorrência:<br>Verifica valor (acima dos limites de outras modalidades)<br>Verifica complexidade técnica<br>Define critério de julgamento<br>(menor preço, técnica e preço, melhor técnica)"]
    
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
    T --> U["DAT prepara edital de Concorrência:<br>Finaliza o edital<br>Realiza publicação no PNCP e Diário Oficial<br>Define Comissão de Licitação<br>Estabelece data para recebimento dos envelopes"]
    
    %% Sessão Pública da Concorrência
    U --> V["Sessão pública da Concorrência:<br>Recebimento dos envelopes<br>Habilitação dos licitantes<br>Julgamento das propostas<br>Classificação<br>Declaração do vencedor"]
    
    %% Adjudicação e Homologação
    V --> W["Adjudicação:<br>Comissão declara vencedor<br>Abre prazo recursal<br>Adjudica objeto após recursos"]
    W --> X["Homologação:<br>Autoridade superior analisa processo<br>Solicita homologação do Presidente"]
    
    %% Contratação
    X --> Y["Contrato e empenho:<br>Elabora contrato<br>Convoca para assinatura<br>Emite nota de empenho<br>Publica extrato no PNCP<br>Exige garantia contratual"]
    
    %% Gestão Contratual
    Y --> Z["Gestão do contrato:<br>Designa fiscal e gestor<br>Acompanha execução<br>Realiza medições e pagamentos<br>Verifica cumprimento<br>Gerencia aditivos (se necessário)"]
    
    %% Finalização
    Z --> ZA["Encerramento:<br>Verifica conclusão<br>Emite termo de recebimento provisório<br>Emite termo de recebimento definitivo<br>Libera garantia<br>Arquiva processo"]
    
    %% Check List Concorrência - Lateral
    subgraph "Check List Concorrência"
    CL1["Documentos para iniciar processo:<br>Justificativa da contratação<br>Projeto Básico/Executivo<br>Orçamento detalhado<br>Cronograma físico-financeiro<br>Estudo Técnico Preliminar (ETP)<br>Análise de Riscos<br>ART/RRT (se obra)"]
    
    CL2["Documentos do Edital:<br>Minuta do Edital<br>Projeto Básico/Executivo<br>Planilhas orçamentárias<br>Minuta do Contrato<br>Parecer Jurídico<br>Publicações"]
    
    CL3["Documentos da Sessão:<br>Documentos de habilitação<br>Propostas técnicas (se aplicável)<br>Propostas de preços<br>Atas das sessões<br>Recursos e contrarrazões<br>Adjudicação<br>Homologação"]
    
    CL4["Documentos para contratação:<br>Contrato assinado<br>Publicação do extrato<br>Designação de fiscal/gestor<br>Garantia contratual<br>Ordem de serviço/fornecimento"]
    end
    
    %% Características da Concorrência
    subgraph "Características da Concorrência"
    CP1["Aplicabilidade:<br>Obras e serviços especiais de engenharia<br>Concessões e PPPs<br>Bens e serviços especiais<br>Licitações internacionais<br>Alienação de bens imóveis"]
    
    CP2["Critérios de julgamento:<br>Menor preço<br>Melhor técnica<br>Técnica e preço<br>Maior retorno econômico<br>Maior desconto"]
    
    CP3["Prazos:<br>Publicação: mínimo 15 dias úteis (regra geral)<br>Publicação: mínimo 25 dias úteis (técnica e preço)<br>Recursal: 3 dias úteis<br>Validade das propostas: 60 dias (prorrogável)"]
    end
    
    %% Limites
    subgraph "Limites de Aplicação"
    LA1["Obras e Serviços Especiais de Engenharia:<br>Acima de R$ 1.500.000,00"]
    
    LA2["Compras e Serviços:<br>Acima de R$ 1.000.000,00"]
    
    LA3["Obrigatória para:<br>Concessões e PPPs<br>Compra e alienação de bens imóveis<br>Licitações internacionais"]
    end
