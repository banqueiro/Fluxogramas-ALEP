```mermaid
flowchart TD
    A["Início: Demanda de sistema (ex.: GMS, SIAFIC, SEI, CONTRATOSGOV, PORTAL TRANSPARENCIA, PUBLICADOR PCA, IA COMPRASGOV, etc.)"] --> B["Receber solicitação (usuário / setor)"]
    B --> C["Verificar tipo: Acesso novo / Adequação / Erro / Treinamento"]
    C --> D["Administrar acesso (cadastro, perfil, permissões)"]
    D --> E["Adequar configuração (parâmetros, fluxos customizados)"]
    E --> F["Gerir demandas: Monitorar uso, resolver incidentes"]
    F --> G["Treinar / Orientar usuários se necessário"]
    G --> H["Registrar logs / Relatório de gestão"]
    H --> I["Final: Demanda atendida / Sistema atualizado"]
