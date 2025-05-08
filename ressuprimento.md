# Fluxograma - Ressuprimento

```mermaid
graph TD
    subgraph Áreas
        DEMANDANTE[Diretoria Demandante]
        DG[DG]
        DAT[DAT]
        SUPRIMENTOS[DAT / SUPRIMENTOS]
        CONTABILIDADE[DAT / CONTABILIDADE]
        SECRETARIA[1&ordf; Secretaria]
        ALMOXARIFADO[DA / Almoxarifado]
        CONTRATADO[Contratado]
    end

    A[Início] -->|I| B[DEMANDANTE<br>Elabora solicitação<br>Encaminha para DG<br>1 dia]
    B -->|II| C[DG<br>Recebe e encaminha para DAT<br>0 dias]
    C -->|III| D[DAT<br>Verifica solicitação e condições<br>Encaminha para DG<br>0 dias]
    D -->|IV| E[DG<br>Analisa informações<br>Encaminha para 1&ordf; Secretaria<br>1 dia]
    E -->|V| F[SECRETARIA<br>Aprova solicitação<br>Encaminha para DG<br>1 dia]
    F -->|VI| G[DG<br>Recebe para conhecimento<br>Encaminha para SUPRIMENTOS<br>0 dias]
    G -->|VII| H[SUPRIMENTOS<br>Verifica documentos<br>Encaminhar para CONTABILIDADE<br>0 dias]
    H -->|VIII| I[CONTABILIDADE<br>Inclui empenho<br>Devolve para SUPRIMENTOS<br>0 dias]
    I -->|IX| J[SUPRIMENTOS<br>Elabora ordem de serviço<br>Informa fiscal<br>Encaminha para CONTRATADO<br>0 dias]
    J -->|X| K[DEMANDANTE<br>Fiscal acompanha entrega e nota fiscal<br>1 dia]
    K -->|XI| L[ALMOXARIFADO<br>Recebe itens<br>Inclui nota fiscal no SEI<br>Encaminha para SUPRIMENTOS<br>1 dia]
    L -->|XII| M[SUPRIMENTOS<br>Verifica documentos<br>Encaminha para certificação<br>0 dias]
    M -->|XIII| N[DEMANDANTE<br>Certifica nota fiscal<br>Encaminha para SUPRIMENTOS<br>1 dia]
    N -->|XIV| O[SUPRIMENTOS<br>Encaminha para DG para liquidação<br>1 dia]
    O -->|XV| P[DG<br>Encaminha para pagamento<br>1 dia]
    P --> Q[Fim]

    

    class DEMANDANTE,DG,DAT,SUPRIMENTOS,CONTABILIDADE,SECRETARIA,ALMOXARIFADO,CONTRATADO area;
    class A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q tarefa;
