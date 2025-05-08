# Fluxograma - Renovação de Contrato

```mermaid
graph TD
    subgraph Areas
        GESTAO_CONTRATOS[DAT – Gestão de Contratos]
        DIRETORIA_DEMANDANTE[Diretoria Demandante]
        FORNECEDOR[Fornecedor]
        COORD_SUPRIMENTOS[Coordenação de Suprimentos]
    end

    A[Início] -->|I| B[GESTAO_CONTRATOS \ Imprimir relatório de renovações e verificar prazos]
    B -->|II| C[GESTAO_CONTRATOS Elabora aviso de vencimento e Enviar à DIRETORIA_DEMANDANTE]
    C -->|III| D[GESTAO_CONTRATOS Inseri o protocolo SEI no relatório]
    D -->|IV| E{DIRETORIA_DEMANDANTE quer renovar?}
    E -->|Sim| F[GESTAO_CONTRATOS \ Solicita manifestação do FORNECEDOR]
    E -->|Não| G[GESTAO_CONTRATOS \ Concluir processo]
    F -->|V| H{FORNECEDOR quer renovar?}
    H -->|Sim| I[GESTAO_CONTRATOS \ Adicionar documentos \ Encaminhar para COORD_SUPRIMENTOS]
    H -->|Não| J[GESTAO_CONTRATOS \ Adicionar manifestação negativa \ Encaminhar para DIRETORIA_DEMANDANTE]
    G -->|VI| K[Fim]
    I -->|VI| K
    J -->|VI| K

    

    class GESTAO_CONTRATOS,DIRETORIA_DEMANDANTE,FORNECEDOR,COORD_SUPRIMENTOS area;
    class A,B,C,D,E,F,G,H,I,J,K tarefa;
