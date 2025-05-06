# Fluxograma - Solicitação/Autorização da Despesa - Publicidade

```mermaid
graph TD
    %% Áreas à esquerda (conforme o modelo da imagem)
    subgraph Áreas
        REQUERIMENTO[REQUERIMENTO]
        DC_MARKETING[DC / MARKETING]
        DAT_CCONT[DAT / C. CONT]
        DC_DIR_COM[DC / DIRETORIA DE COMUNICAÇÃO]
        DG[DG / DIRETORIA-GERAL]
        PROCURADORIA[PROCURADORIA-GERAL]
        COMISSAO_EXEC[COMISSÃO EXECUTIVA]
        DAT_PUB[DAT / PUBLICIDADE]
    end

    %% Título do Processo
    A[Solicitação/Autorização da Despesa - Publicidade] -->|I| B

    %% Fluxo Principal
    B[DC - Marketing<br>Abertura processo SEI<br>Elaborar Solicitação<br>5 dias] -->|II| C
    C[DAT - Coord. de Contabilidade<br>Emitir Informação do saldo disponível<br>Inserir no Controle<br>Encaminhar ao DC<br>1 dia] -->|III| D
    D[DC - Diretoria de Comunicação<br>Aprovação da Despesa<br>Verificar requisitos<br>Emitir Despacho de aprovação<br>Encaminhar à DG<br>1 dia] -->|IV| E
    E[DG - Diretoria Geral<br>Manifestação/Despacho<br>Verificar requisitos<br>Encaminhar à Procuradoria-Geral<br>1 dia] -->|V| F
    F[Procuradoria-Geral<br>Parecer Jurídico<br>Verificar requisitos<br>Emitir parecer jurídico<br>Encaminhar à DG<br>3 dias] -->|VI| G
    G[DG - Diretoria Geral<br>Manifestação/Despacho<br>Verificar requisitos<br>Encaminhar à Comissão Executiva<br>1 dia] -->|VII| H
    H[Comissão Executiva<br>Autorização da Despesa<br>Verificar requisitos<br>Emitir Autorização da Despesa<br>Assinatura da Comissão<br>1 dia] -->|VIII| I
    I[DAT - Coord. de Contabilidade<br>Realização do Empenho<br>Elaborar Nota de Empenho<br>Encaminhar ao DAT/Publicidade<br>1 dia] -->|IX| J
    J[DAT - Publicidade<br>OS/Ordem de Serviços<br>Elaborar Ordem de Serviços<br>Enviar à Agência<br>Incluir no SEI<br>1 dia] -->|X| K
    K[DC - Marketing<br>Plano de Mídia<br>Incluir Plano de Mídia atualizado<br>1 dia] -->|XI| L[PAGAMENTO E VALIDAÇÃO DOS COMPROVANTES ATENDENDO REQUISITOS<br>Transparência]

    %% Estilização para seguir o modelo da imagem
    classDef area fill:#003087,stroke:#fff,stroke-width:2px,color:#fff;
    classDef tarefa fill:#B0C4DE,stroke:#333,stroke-width:2px;
    classDef transparencia fill:#90EE90,stroke:#333,stroke-width:2px;

    class REQUERIMENTO,DC_MARKETING,DAT_CCONT,DC_DIR_COM,DG,PROCURADORIA,COMISSAO_EXEC,DAT_PUB area;
    class A,B,C,D,E,F,G,H,I,J,K tarefa;
    class L transparencia;
