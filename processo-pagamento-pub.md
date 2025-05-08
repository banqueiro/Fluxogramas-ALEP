# Fluxograma - Processo de Pagamentos de Publicidade

```mermaid
graph TD
    %% Áreas à esquerda (conforme o modelo da imagem)
    subgraph Áreas
        DAT_PUB[DAT / PUBLICIDADE]
        DC_MARKETING[DC / MARKETING]
        DC_DIR_COM[DC / DIRETORIA DE COMUNICAÇÃO]
        DAT_CCONT[DAT / C. CONT]
        DAT_APOIO[DAT / DIRETORIA DE APOIO TÉCNICO]
        DG[DG / DIRETORIA-GERAL]
        DF[DF - DIRETORIA FINANCEIRA]
        SGP_1SEC[SGP E 1ª SECRETARIA]
        FORNECEDOR[FORNECEDOR]
    end

    %% Título do Processo
    A[Processo de Pagamentos - Publicidade] -->|I| B

    %% Fluxo Principal
    B[DAT - Publicidade<br>Conferir documentação no Drive<br>Check List Anexo I<br>Mover para Notas Protocoladas ou Pendência<br>Abrir Processo SEI<br>1 dia] -->|II| C
    C[DAT - Publicidade<br>Abertura Processo de Pagamento SEI<br>Vincular ao Empenho/Contrato<br>Preencher Controle Administrativo<br>Emitir Despacho e Certificação NF<br>Conferência Administrativa<br>Assinar e Encaminhar a DC/Marketing<br>15 dias] -->|III| D
    D[DC - Marketing<br>Conferência Técnica<br>Assinar Despacho no Bloco<br>9 dias] -->|IV| E
    E[DC/Diretoria de Comunicação<br>Emitir Despacho para Contabilidade<br>Assinar Certificação NF e Despacho<br>Encaminhar a DAT/Contabilidade<br>1 dia] -->|V| F
    F[DAT - Coord. de Contabilidade<br>Liquidação<br>Elaborar Liquidação<br>Encaminhar a DAT/Diretoria de Apoio Técnico<br>1 dia] -->|VI| G
    G[DAT - Diretoria de Apoio Técnico<br>Encaminhar a DG - Diretoria Geral<br>0 dias] -->|VII| H
    H[DG - Diretoria Geral<br>Manifestação<br>Verificar Requisitos Contratuais<br>Encaminhar a DF - Diretoria Financeira<br>0 dias] -->|VIII| I
    I[DF - Diretoria Financeira<br>Ordem de Pagamento<br>Verificar Requisitos Contratuais<br>Emitir Ordem de Pagamento<br>Devolver a DG<br>1 dia] -->|IX| J
    J[DG - Diretoria Geral<br>Manifestação<br>Encaminhar Ordem de Pagamento a Presidência/1ª Secretaria<br>0 dias] -->|X| K
    K[1ª Secretaria / Presidência<br>Autorização de Pagamento<br>Assinar Ordem de Pagamento<br>2 dias] -->|XI| L
    L[DF - Diretoria Financeira<br>Pagamento<br>Realizar Pagamento à Agência<br>Enviar Ordem de Pagamento a DAT/Publicidade<br>1 dia] -->|XII| M
    M[DAT - Publicidade<br>Salvar Ordem de Pagamento no Drive<br>2 dias] -->|XIII| N
    N[Fornecedor<br>Comprovante de Pagamento<br>Salvar no Drive<br>3 dias] -->|XIV| O
    O[DAT - Publicidade<br>Conferir Comprovante de Pagamento<br>Subir ao SEI<br>Atualizar Controle Administrativo<br>Finalizar Processo SEI<br>5 dias] -->|XV| P[PAGAMENTO E VALIDAÇÃO DOS COMPROVANTES ATENDENDO REQUISITOS<br>Transparência]

   

    class REQUERIMENTO,DAT_PUB,DC_MARKETING,DC_DIR_COM,DAT_CCONT,DAT_APOIO,DG,DF,SGP_1SEC,FORNECEDOR area;
    class A,B,C,D,E,F,G,H,I,J,K,L,M,N,O tarefa;
    class P transparencia;
