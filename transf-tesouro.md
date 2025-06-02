# Fluxograma - Transferências de Recursos para o Tesouro Estadual

```mermaid
flowchart TD
    SGP[SGP – Secretaria Geral da Presidência<br/>Inicia o processo SEI e elabora ofício solicitando providências administrativas]
    DG[DG – Diretoria Geral<br/>Encaminha o processo para DAT e DF]
    DAT[DAT/CCONT – Diretoria de Apoio Técnico<br/>Verifica as dotações e elabora a minuta<br/>Prazo: 1 dia útil]
    DF1[DF – Diretoria Financeira<br/>Elabora e programa a ordem de pagamento]
    DP[DP – Diretoria de Pessoal<br/>Publica o Ato da comissão executiva]
    DF2[DF – Diretoria Financeira<br/>Executa a transferência financeira]

    SGP --> DG
    DG --> DAT
    DG --> DF1
    DAT --> DP
    DF1 --> DP
    DP --> DF2
