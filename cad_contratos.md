# Fluxograma - Cadastro de Contratos

```mermaid
graph TD
    subgraph Áreas
        DAT[DAT]
        CONTABILIDADE[DAT / CONTABILIDADE]
        CONTRATOS[DAT / CONTRATOS]
        DG[DG Diretoria Geral]
        SECRETARIA[1&ordf; Secretaria]
        EMPRESA[Empresa]
    end

    A[Início] -->|I| B[DAT<br>Recebe processo homologado<br>Encaminha para DAT / CONTABILIDADE<br>1 dia]
    B -->|II| C[CONTABILIDADE<br>Inclui empenho no SEI<br>Passa para Gestão de Contratos<br>0 dias]
    C -->|III| D[DAT<br>Encaminha contrato/ata para assinatura da empresa - Empresa assina e devolve<br>5 dias]
    D -->|IV| E[DAT<br>Recebe contrato/ata assinado<br>Encaminha para Diretoria Geral<br>0 dias]
    E -->|V| F[DG<br>Assina contrato/ata<br>Encaminha para 1&ordf; Secretaria<br>1 dia]
    F -->|VI| G[SECRETARIA<br>Solicita assinatura do 1&ordf; Secretário<br>Devolve para DAT<br>0 dias]
    G -->|VII| H[DAT<br>Recebe contrato/ata<br>Envia via para empresa<br>Insere no SEI<br>Publica no Di&aacute;rio Oficial<br>Insere publicação no SEI<br>Encaminha para CONTABILIDADE<br>1 dia]
    H -->|VIII| I[CONTABILIDADE<br>Emite empenho<br>Encaminha à CONTRATOS<br>0 dias]
    I -->|IX| J[CONTRATOS<br>Insere dados na planilha e relatório<br>Confere Portal da Transparência<br>Envia ordem de serviço para empresa<br>Encerrar processo e avisar área demandante<br>0 dias]
    J --> K[Fim]

    classDef area fill:#003087,stroke:#fff,stroke-width:2px,color:#fff;
    classDef tarefa fill:#B0C4DE,stroke:#333,stroke-width:2px;

    class DAT,CONTABILIDADE,CONTRATOS,DG,SECRETARIA,EMPRESA area;
    class A,B,C,D,E,F,G,H,I,J,K tarefa;
