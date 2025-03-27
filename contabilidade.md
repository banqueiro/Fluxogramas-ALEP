# Fluxograma da Coordenadoria de Contabilidade - DAT

```mermaid

flowchart TD
    A["Início do Processo Contábil: Recebimento da documentação necessária para os registros contábeis, como notas fiscais e comprovantes."] --> B["Recebimento e conferência da documentação fiscal entregue pelos setores responsáveis, garantindo a conformidade com as normas."] 
    B --> C["Análise e classificação dos documentos recebidos, categorizando-os corretamente de acordo com os princípios contábeis vigentes."]
    C --> D["Registro das informações no sistema contábil oficial, garantindo o correto lançamento de cada item conforme a legislação aplicável."]
    D --> E{"Verificação da integridade da documentação e do correto preenchimento dos dados informados para evitar inconsistências contábeis."}
    E -->|Não| F["Caso faltem documentos ou haja informações incorretas, será solicitada a complementação da documentação junto ao setor responsável."]
    F --> B
    E -->|Sim| G["Com toda a documentação correta, são elaborados os relatórios contábeis, como balancetes e demonstrações financeiras."]
    G --> H["Realização da conciliação bancária para garantir que os lançamentos contábeis estejam compatíveis com os extratos das contas da instituição."]
    H --> I["Fechamento mensal das contas contábeis, consolidando as informações financeiras e contábeis de cada período."]
    I --> J["Elaboração de demonstrativos contábeis obrigatórios, como balanço patrimonial, demonstração do resultado e fluxo de caixa."]
    J --> K["Análise de conformidade dos lançamentos contábeis, garantindo que todas as informações estejam corretas e atendam às normas vigentes."]
    K --> L{"A documentação contábil e os lançamentos estão em conformidade com as exigências legais?"}
    L -->|Não| M["Caso haja erros ou inconsistências, são feitos os ajustes contábeis necessários para regularizar os registros."]
    M --> K
    L -->|Sim| N["Após a conferência final, os documentos são enviados ao Tribunal de Contas para prestação de contas e auditorias."]
    N --> O["Os documentos são arquivados digitalmente para garantir a rastreabilidade e facilitar futuras consultas."]
    O --> P["Elaboração de relatórios gerenciais para apoio à tomada de decisão e transparência da gestão financeira."]
    P --> Q["Realização da prestação de contas anual, consolidando os dados contábeis do exercício."]
    Q --> R["Encerramento do processo contábil após a devida prestação de contas."]
