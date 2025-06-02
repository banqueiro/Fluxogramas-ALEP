# Fluxograma - Transferências de Recursos para o Tesouro Estadual

```mermaid
flowchart TD
    SGP[SGP – Secretaria Geral da Presidência<br/>Inicia o processo SEI e elabora ofício solicitando providências administrativas]
    DG[DG – Diretoria Geral<br/>Encaminha o processo para DAT e DF]
    DAT[DAT/CCONT – Diretoria de Apoio Técnico<br/>Verifica as dotações e elabora a minuta<br/>Prazo: 1 dia útil]
    DF1[DF – Diretoria Financeira<br/>Elabora e programa a ordem de pagamento]
    DP[DP – Diretoria de Pessoal<br/>Faz a gestão numérica do Ato de Publicação da comissão executiva]
    DL[DL – Diretoria Legislativa<br/>Publica o Ato da comissão executiva]
    DF2[DF – Diretoria Financeira<br/>Executa a transferência financeira]
    DAT2[DAT/CCONT – Diretoria de Apoio Técnico<br/>Executa a transferência Orçamentária]

    SGP --> DG
    DG --> DAT
    DG --> DF1
    DAT --> DP
    DF1 --> DP
    DP --> DL
    DL --> DF2
    DF2 --> DAT2
