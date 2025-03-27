
### 3. concurso.md

```markdown
# Fluxograma de Concurso - Lei 14.133/2021

```mermaid
flowchart TD
    %% Início e Diretoria Demandante
    A["Início"] --> B["Diretoria Demandante"]
    B --> C["Elaboração dos documentos essenciais:<br>Justificativa da necessidade<br>Objeto do concurso<br>Valor da premiação<br>Critérios de julgamento<br>Indicação da dotação orçamentária"]
    
    %% Fluxo entre departamentos iniciais
    C --> D["DG - Diretoria Geral<br>Recebe o processo"]
    D --> E["Verifica a solicitação<br>Encaminha para DAT"]
    
    %% DAT - Diretoria de Apoio Técnico
    E --> F["DAT - Diretoria de Apoio Técnico<br>Recebe e processa"]
    F --> G["Verifica natureza do objeto<br>Confirma aplicabilidade do Concurso<br>Verifica valor da premiação<br>Elabora estimativa de custos"]
    
    %% Verificação de documentação
    G --> H["Analisa requisitos técnicos<br>Verifica critérios de julgamento<br>Verifica completude do processo"]
    H --> I["Verifica documentos essenciais:<br>Justificativa da contratação<br>Definição clara do objeto<br>Critérios objetivos de julgamento<br>Valor da premiação<br>Dotação orçamentária"]
    
    %% Elaboração de documentos técnicos
    I --> J["Elabora documentos do Concurso:<br>Regulamento detalhado<br>Critérios de avaliação<br>Composição da comissão julgadora<br>Verifica disponibilidade orçamentária<br>Elabora minuta do edital<br>Define premiação e direitos autorais"]
    
    %% Verificação de modalidade
    J --> K["Confirma modalidade Concurso:<br>Verifica se objeto é trabalho técnico, científico ou artístico<br>Define critérios de julgamento<br>Estabelece regras para comissão julgadora"]
    
    %% Encaminhamento para 1ª SEC
    K --> L["Encaminha processo para 1ª SEC"]
    
    %% 1ª SEC
    L --> M["1ª SEC<br>Recebe e processa"]
    M --> N["Verifica documentação<br>Encaminha para Procuradoria<br>Se necessário, solicita complementação"]
    
    %% Procuradoria
    N --> O["Procuradoria<br>Recebe o processo"]
    O --> P["Analisa parecer jurídico<br>Verifica legalidade do procedimento<br>Analisa questões de direitos autorais<br>Encaminha para Controladoria"]
    
    %% Controladoria
    P --> Q["Controladoria<br>Recebe o processo"]
    Q --> R["Analisa legalidade<br>Encaminha para o DG"]
    
    %% Retorno ao DG e Continuidade
    R --> S["DG recebe processo com pareceres"]
    S --> T["Verifica autorização:<br>Analisa pareceres<br>Solicita autorização do Presidente<br>Encaminha para DAT"]
    
    %% Preparação do Edital e Publicação
    T --> U["DAT prepara edital de Concurso:<br>Finaliza o regulamento<br>Realiza publicação no PNCP e Diário Oficial<br>Define Comissão Julgadora<br>Estabelece cronograma do concurso"]
    
    %% Realização do Concurso
    U --> V["Realização do Concurso:<br>Inscrições dos participantes<br>Recebimento dos trabalhos<br>Avaliação pela Comissão Julgadora<br>Classificação<br>Declaração do(s) vencedor(es)"]
    
    %% Homologação e Premiação
    V --> W["Homologação do resultado:<br>Comissão apresenta resultado<br>Abre prazo recursal<br>Autoridade homologa resultado"]
    W --> X["Premiação:<br>Autoridade superior autoriza premiação<br>Solicita empenho dos valores<br>Realiza cerimônia de premiação (se aplicável)"]
    
    %% Contratação (se aplicável)
    X --> Y["Contratação (se aplicável):<br>Elabora contrato para desenvolvimento do trabalho<br>Convoca vencedor para assinatura<br>Emite nota de empenho<br>Publica extrato no PNCP"]
    
    %% Gestão Contratual (se aplicável)
    Y --> Z["Gestão do contrato (se aplicável):<br>Designa fiscal e gestor<br>Acompanha execução<br>Realiza pagamentos<br>Verifica cumprimento"]
    
    %% Finalização
    Z --> ZA["Encerramento:<br>Verifica conclusão<br>Emite termo de recebimento<br>Arquiva processo"]
    
    %% Check List Concurso - Lateral
    subgraph "Check List Concurso"
    CL1["Documentos para iniciar processo:<br>Justificativa da necessidade<br>Termo de Referência específico<br>Critérios de julgamento<br>Valor da premiação<br>Estudo Técnico Preliminar (ETP)"]
    
    CL2["Documentos do Edital:<br>Regulamento do Concurso<br>Critérios de avaliação<br>Composição da Comissão Julgadora<br>Premiação e direitos autorais<br>Parecer Jurídico<br>Publicações"]
    
    CL3["Documentos da Realização:<br>Inscrições dos participantes<br>Trabalhos apresentados<br>Atas de julgamento<br>Recursos e contrarrazões<br>Resultado final<br>Homologação"]
    
    CL4["Documentos para premiação/contratação:<br>Autorização de pagamento da premiação<br>Contrato (se desenvolvimento posterior)<br>Publicação do extrato<br>Termo de cessão de direitos autorais"]
    end
    
    %% Características do Concurso
    subgraph "Características do Concurso"
    CP1["Aplicabilidade:<br>Trabalhos técnicos, científicos ou artísticos<br>Projetos arquitetônicos ou urbanísticos<br>Criação de desenho industrial<br>Trabalhos intelectuais"]
    
    CP2["Particularidades:<br>Julgamento por comissão especializada<br>Anonimato dos participantes (quando possível)<br>Cessão de direitos autorais<br>Premiação ou remuneração"]
    
    CP3["Prazos:<br>Publicação: mínimo 35 dias<br>Recursal: 5 dias úteis<br>Desenvolvimento posterior: conforme edital"]
    end
    
    %% Direitos Autorais
    subgraph "Direitos Autorais"
    DA1["Cessão de Direitos:<br>Edital deve prever cessão de direitos patrimoniais<br>Possibilidade de uso pela Administração<br>Remuneração pela cessão"]
    
    DA2["Desenvolvimento posterior:<br>Possibilidade de contratação do vencedor<br>Condições estabelecidas no edital"]
    end
