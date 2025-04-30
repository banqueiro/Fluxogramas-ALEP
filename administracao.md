```mermaid
graph TD
    A[DAT Administração] -->|Férias| B1[Solicitação: Recebimento do pedido de férias do servidor]
    A -->|Folha de Ponto| C1[Recebimento: Envio da folha de ponto pela DP à DAT]
    A -->|Plano de Contratação| D1[Elaboração: Criação inicial do Plano de Contratação Anual pela DAT]

    subgraph Pedido de Férias
        B1 --> B2[Abertura do Processo: Criação do processo no SEI pela DAT]
        B2 --> B3[Encaminhamento: Envio do processo à Diretoria de Pessoal]
        B3 --> B4[Análise: Avaliação do pedido pela Diretoria de Pessoal]
        B4 --> B5[Resposta: Retorno do resultado ao processo]
        B5 --> B6[Comunicação: Notificação do servidor pela DAT]
    end

    subgraph Folha de Ponto
        C1 --> C2[Justificativa: Elaboração das justificativas de faltas pela DAT]
        C2 --> C3[Anexação: Inclusão de atestados e declarações no processo]
        C3 --> C4[Relatório: Elaboração do relatório de horas pela DAT]
        C4 --> C5[Encaminhamento: Envio do relatório à Diretoria de Pessoal]
        C5 --> C6[Análise: Verificação e execução de descontos pela Diretoria de Pessoal]
        C6 --> C7[Conclusão: Finalização do processo com confirmação da DP]
    end

    subgraph Plano de Contratação Anual
        D1 --> D2[Atualização: Revisão e ajuste do plano pela DAT]
        D2 --> D3[Envio: Distribuição do plano às diretorias e áreas demandantes]
        D3 --> D4[Análise: Revisão do plano pelas áreas demandantes]
        D4 --> D5[Ajustes: Incorporação de atualizações, se necessário]
        D5 --> D6[Finalização: Consolidação do plano pela DAT]
    end
