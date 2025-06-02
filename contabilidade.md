# Fluxograma da Coordenadoria de Contabilidade - DAT

```mermaid
flowchart TD
    %% Processo Contábil Geral
    A["Início do Processo Contábil"] --> B["Recebimento de Documentação Fiscal"]
    B --> C["Análise e Classificação Contábil"]
    C --> D["Registro no Sistema Contábil"]
    D --> E{"Documentação Completa?"}
    E -->|Não| F["Solicitar Documentação Complementar"]
    F --> B
    E -->|Sim| G["Elaboração de Relatórios Contábeis"]
    G --> H["Conciliação Bancária"]
    H --> I["Fechamento Mensal"]
    I --> J["Elaboração de Demonstrativos Contábeis"]
    J --> K["Análise de Conformidade"]
    K --> L{"Conformidade OK?"}
    L -->|Não| M["Ajustes Contábeis"]
    M --> K
    L -->|Sim| N["Envio ao Tribunal de Contas"]
    N --> O["Arquivamento Digital"]
    O --> P["Elaboração de Relatórios Gerenciais"]
    P --> Q["Prestação de Contas Anual"]
    Q --> R["Fim do Processo"]

    %% Substituindo Processos Periódicos pelo novo bloco:
    subgraph "Recursos para o Tesouro"

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
    end

    %% Processos Específicos permanecem inalterados
    subgraph "Processos Específicos"
        W["Registro Patrimonial"] --> X["Depreciação de Bens"]
        X --> Y["Inventário Anual"]
        Y --> Z["Baixa de Bens"]
    end
