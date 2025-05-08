# Fluxograma - Processo de Liquidação

```mermaid
graph TD
    subgraph Áreas
        DAT[DAT]
        SUPRIMENTOS[DAT / SUPRIMENTOS]
        CONTABILIDADE[DAT / CONTABILIDADE]
        FISCAL[Fiscal de Contrato]
        DG[Diretoria Geral]
        DF[Diretoria Financeira]
        SECRETARIA[1&ordf; Secretaria]
    end

    A[Início] -->|I| B[E-mail DAT<br>Recebe nota fiscal<br>Inicia processo SEI<br>Encaminha para certificação<br>1 dia]
    B -->|II| C[SUPRIMENTOS<br>Verifica documentação<br>Assina despacho<br>0 dias]
    C -->|III| D[FISCAL<br>Verifica valor da nota<br>Certifica documento<br>2 dias]
    D -->|IV| E[DAT<br>Prepara despacho de liquidação<br>1 dia]
    E -->|V| F[SUPRIMENTOS<br>Verifica regularidade<br>Encaminha para CONTABILIDADE<br>0 dias]
    F -->|VI| G{Tem retenção?}
    G -->|No| H[CONTABILIDADE<br>Sem retenção: realiza liquidação<br>1 dia]
    G -->|Yes| I[CONTABILIDADE<br>Com retenção: prepara guias, realiza liquidação<br>0 dias]
    H -->|VII| J[DAT<br>Diretor assina<br>Encaminha para DG<br>1 dia]
    I -->|VII| J
    J -->|VIII| K[DG<br>Analisa<br>Encaminha para DF<br>1 dia]
    K -->|IX| L[DF<br>Analisa<br>Prepara ordem de pagamento<br>Encaminha para DG<br>0 dias]
    L -->|X| M[DG<br>Prepara autorização de pagamento<br>Encaminha para 1 SECRETARIA<br>1 dia]
    M -->|XI| N[1 SECRETARIA<br>Assina autorização de pagamento<br>Encaminha para DF<br>1 dia]
    N -->|XII| O[DF<br>Realiza depósito de pagamento<br>Anexa comprovação no SEI<br>Encaminha para DAT<br>1 dia]
    O -->|XIII| P[DAT<br>Finaliza processo<br>0 dias]
    P --> Q[Fim]

   
    class DAT,SUPRIMENTOS,CONTABILIDADE,FISCAL,DG,DF,SECRETARIA area;
    class A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q tarefa;
