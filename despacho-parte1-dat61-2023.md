# Fluxograma de Atividades da Diretoria de Apoio Técnico

```mermaid
graph TD
    A[Diretoria de Apoio Técnico] -->|Diretor| B1[Planejar: Definir diretrizes para licitações e orçamento]
    A -->|Chefia de Gabinete| C1[Assessorar: Preparar materiais para o Diretor]
    A -->|Suprimentos| E1[Solicitar: Receber demandas de compras]
    A -->|Contratos| F1[Controlar: Monitorar saldos e vigências de contratos]
    A -->|Publicidade| G1[Solicitar: Receber demandas de publicidade no SEI]

    subgraph Diretor de Apoio Técnico
        B1 --> B2[Supervisionar: Acompanhar licitações e dispensa/inexigibilidade]
        B2 --> B3[Controlar: Monitorar saldos de contratos e aditivos]
        B3 --> B4[Registrar: Supervisionar atos orçamentários e financeiros]
        B4 --> B5[Elaborar: Coordenar proposta orçamentária]
        B5 --> B6[Executar: Aprovar balancetes e demonstrativos]
        B6 --> B7[Assegurar: Garantir conformidade legal]
    end

    subgraph Chefia de Gabinete
        C1 --> C2[Coordenar: Supervisionar servidores da DAT]
        C2 --> C3[Elaborar: Redigir atos normativos e correspondências]
        C3 --> C4[Receber: Gerenciar entrada de processos no SEI]
        C4 --> C5[Acompanhar: Monitorar fluxo de processos]
        C5 --> C6[Finalizar: Arquivar ou encaminhar processos]
   
    end

    subgraph Coordenadoria de Suprimentos
        E1 --> E2[Planejar: Elaborar termos de referência]
        E2 --> E3[Licitar: Conduzir licitações ou dispensa/inexigibilidade]
        E3 --> E4[Julgar: Avaliar propostas e habilitar fornecedores]
        E4 --> E5[Contratar: Formalizar contratos ou aditivos]
        E5 --> E6[Cadastrar: Atualizar cadastro de fornecedores]
        E6 --> E7[Acompanhar: Monitorar execução das aquisições]
    end

    subgraph Coordenadoria Administrativa de Contratos
        F1 --> F2[Emitir: Gerar ordens de serviço e empenhos]
        F2 --> F3[Notificar: Enviar sanções ou multas contratuais]
        F3 --> F4[Verificar: Conferir regularidade fiscal]
        F4 --> F5[Analisar: Avaliar pedidos de repactuação/reequilíbrio]
        F5 --> F6[Avisar: Notificar vencimentos de contratos]
    end

    subgraph Coordenadoria Administrativa de Publicidade
        G1 --> G2[Instruir: Abrir processo no sistema eletrônico]
        G2 --> G3[Emitir: Gerar ordens de serviço para Diretoria de Comunicação]
        G3 --> G4[Verificar: Analisar conformidade documental]
        G4 --> G5[Encaminhar: Enviar processo à Diretoria Financeira]
        G5 --> G6[Relatar: Elaborar e validar relatórios de gastos]
        G6 --> G7[Publicar: Disponibilizar relatórios no Portal da Transparência]
    end
