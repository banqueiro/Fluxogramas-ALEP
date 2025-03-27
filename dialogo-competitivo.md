# Fluxograma de Diálogo Competitivo - Lei 14.133/2021

```mermaid
flowchart TD
    %% Início e Diretoria Demandante
    A["Início"] --> B["Diretoria Demandante"]
    B --> C["Elaboração dos documentos essenciais:<br>Justificativa da necessidade<br>Descrição da necessidade<br>Demonstração da inovação/complexidade<br>Indicação da dotação orçamentária"]
    
    %% Fluxo entre departamentos iniciais
    C --> D["DG - Diretoria Geral<br>Recebe o processo"]
    D --> E["Verifica a solicitação<br>Encaminha para DAT"]
    
    %% DAT - Diretoria de Apoio Técnico
    E --> F["DAT - Diretoria de Apoio Técnico<br>Recebe e processa"]
    F --> G["Verifica complexidade do objeto<br>Confirma aplicabilidade do Diálogo Competitivo<br>Verifica impossibilidade de especificação prévia<br>Elabora justificativa técnica"]
    
    %% Verificação de documentação
    G --> H["Analisa requisitos técnicos<br>Verifica justificativa de inovação/complexidade<br>Verifica completude do processo"]
    H --> I["Verifica documentos essenciais:<br>Justificativa da contratação<br>Demonstração da inovação/complexidade<br>Impossibilidade de especificação prévia<br>Dotação orçamentária"]
    
    %% Elaboração de documentos técnicos
    I --> J["Elabora documentos do Diálogo Competitivo:<br>Documento de necessidades<br>Requisitos mínimos de qualificação<br>Critérios de pré-seleção<br>Verifica disponibilidade orçamentária<br>Elabora minuta do edital<br>Define comissão de contratação"]
    
    %% Verificação de modalidade
    J --> K["Confirma modalidade Diálogo Competitivo:<br>Verifica inovação/adaptação/complexidade técnica<br>Confirma impossibilidade de especificação prévia<br>Define critérios de pré-seleção<br>Estabelece regras para a fase de diálogo"]
    
    %% Encaminhamento para 1ª SEC
    K --> L["Encaminha processo para 1ª SEC"]
    
    %% 1ª SEC
    L --> M["1ª SEC<br>Recebe e processa"]
    M --> N["Verifica documentação<br>Encaminha para Procuradoria<br>Se necessário, solicita complementação"]
    
    %% Procuradoria
    N --> O["Procuradoria<br>Recebe o processo"]
    O --> P["Analisa parecer jurídico<br>Verifica legalidade do procedimento<br>Analisa justificativa da modalidade<br>Encaminha para Controladoria"]
    
    %% Controladoria
    P --> Q["Controladoria<br>Recebe o processo"]
    Q --> R["Analisa legalidade<br>Encaminha para o DG"]
    
    %% Retorno ao DG e Continuidade
    R --> S["DG recebe processo com pareceres"]
    S --> T["Verifica autorização:<br>Analisa pareceres<br>Solicita autorização do Presidente<br>Encaminha para DAT"]
    
    %% Preparação do Edital e Publicação
    T --> U["DAT prepara edital de Diálogo Competitivo:<br>Finaliza o edital de pré-seleção<br>Realiza publicação no PNCP e Diário Oficial<br>Define Comissão de Contratação<br>Estabelece cronograma do diálogo"]
    
    %% Fase de Pré-seleção
    U --> V["Fase de Pré-seleção:<br>Recebimento de documentação<br>Análise da qualificação técnica<br>Seleção dos participantes do diálogo<br>Convocação para fase de diálogo"]
    
    %% Fase de Diálogo
    V --> W["Fase de Diálogo:<br>Reuniões individuais com pré-selecionados<br>Discussão de soluções propostas<br>Registro das reuniões<br>Confidencialidade das informações<br>Encerramento do diálogo"]
    
    %% Fase Competitiva
    W --> X["Fase Competitiva:<br>Elaboração do termo de referência/projeto básico<br>Convocação para apresentação de propostas finais<br>Julgamento conforme critérios definidos<br>Seleção da proposta mais vantajosa"]
    
    %% Adjudicação e Homologação
    X --> Y["Adjudicação e Homologação:<br>Comissão declara vencedor<br>Abre prazo recursal<br>Adjudica objeto após recursos<br>Autoridade homologa resultado"]
    
    %% Contratação
    Y --> Z["Contrato e empenho:<br>Elabora contrato<br>Convoca para assinatura<br>Emite nota de empenho<br>Publica extrato no PNCP<br>Exige garantia contratual"]
    
    %% Gestão Contratual
    Z --> ZA["Gestão do contrato:<br>Designa fiscal e gestor<br>Acompanha execução<br>Realiza pagamentos<br>Verifica cumprimento"]
    
    %% Finalização
    ZA --> ZB["Encerramento:<br>Verifica conclusão<br>Emite termo de recebimento<br>Arquiva processo"]
    
    %% Check List Diálogo Competitivo - Lateral
    subgraph "Check List Diálogo Competitivo"
    CL1["Documentos para iniciar processo:<br>Justificativa da necessidade<br>Demonstração da inovação/complexidade<br>Impossibilidade de especificação prévia<br>Estudo Técnico Preliminar (ETP)<br>Análise de Riscos"]
    
    CL2["Documentos do Edital de Pré-seleção:<br>Minuta do Edital<br>Documento de necessidades<br>Requisitos de qualificação<br>Critérios de pré-seleção<br>Parecer Jurídico<br>Publicações"]
    
    CL3["Documentos da Fase de Diálogo:<br>Atas das reuniões<br>Registro das soluções propostas<br>Termos de confidencialidade<br>Documento de encerramento do diálogo<br>Termo de referência/projeto básico final"]
    
    CL4["Documentos da Fase Competitiva:<br>Propostas finais<br>Ata de julgamento<br>Recursos e contrarrazões<br>Adjudicação<br>Homologação"]
    
    CL5["Documentos para contratação:<br>Contrato assinado<br>Publicação do extrato<br>Designação de fiscal/gestor<br>Garantia contratual<br>Ordem de serviço/fornecimento"]
    end
    
    %% Características do Diálogo Competitivo
    subgraph "Características do Diálogo Competitivo"
    CP1["Aplicabilidade:<br>Inovação tecnológica ou técnica<br>Impossibilidade de especificação prévia<br>Necessidade de adaptação de soluções<br>Complexidade técnica ou jurídica<br>Soluções não disponíveis no mercado"]
    
    CP2["Fases do procedimento:<br>Pré-seleção de licitantes<br>Diálogo com os pré-selecionados<br>Fase competitiva com apresentação de propostas"]
    
    CP3["Prazos:<br>Publicação: mínimo 25 dias úteis<br>Diálogo: conforme edital<br>Fase competitiva: mínimo 60 dias<br>Recursal: 5 dias úteis"]
    end
    
    %% Comissão de Contratação
    subgraph "Comissão de Contratação"
    CC1["Composição:<br>Servidores efetivos ou empregados públicos<br>Pelo menos 3 membros<br>Especialistas na área do objeto"]
    
    CC2["Atribuições:<br>Condução do diálogo<br>Registro das reuniões<br>Elaboração do termo de referência/projeto básico<br>Julgamento das propostas"]
    end
