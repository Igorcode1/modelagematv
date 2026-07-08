# Engenharia de Requisitos - Cartografia Participativa Quilombola

Este documento apresenta a especificação de Requisitos Funcionais (RF) e Não Funcionais (RNF) para o sistema de Cartografia Participativa da comunidade quilombola de Itapecuru-Mirim, com foco na preservação da memória e alta usabilidade.

## Requisitos Funcionais

# Engenharia de Requisitos - Cartografia Participativa Quilombola
## Especificação de Requisitos Funcionais (RF)

A tabela abaixo descreve as funcionalidades do sistema, mapeadas com os seus respetivos identificadores formais, nomes descritivos, comportamentos esperados e criticidade para o negócio (Prioridade).

| Identificador | Nome | Descrição | Prioridade |
| :--- | :--- | :--- | :--- |
| **RF-001** | Marcação de Pontos Culturais e Históricos | O sistema deve permitir que os moradores/utilizadores marquem geograficamente no mapa os locais sagrados, áreas de festas tradicionais, pontos de plantio e caminhos antigos. | **Alta** |
| **RF-002** | Registo de Relatos Orais em Áudio | O sistema deve permitir a gravação direta ou o upload de ficheiros de áudio através de dispositivos móveis para associar as histórias contadas pelos anciãos aos pontos geográficos do mapa. | **Alta** |
| **RF-003** | Upload de Acervo Fotográfico e Histórico | O sistema deve disponibilizar uma funcionalidade para carregar fotografias e imagens de documentos antigos, vinculando-as ao ponto geográfico correspondente. | **Média** |
| **RF-004** | Linha do Tempo Integrada | O sistema deve oferecer uma visualização cronológica (linha do tempo) associada aos pontos mapeados para organizar e encadear os acontecimentos históricos da comunidade. | **Média** |
| **RF-005** | Consulta e Navegação Pública | O sistema deve permitir que qualquer membro da comunidade navegue pelo mapa interativo e aceda livremente aos áudios, fotos e textos cadastrados. | **Alta** |

---

### Critérios de Atribuição de Prioridade (Padrão de Engenharia)
* **Alta (Essencial):** Funcionalidades indispensáveis, sem as quais o sistema não cumpre o seu propósito core de Cartografia Participativa (Core MVP).
* **Média (Importante):** Funcionalidades que adicionam grande valor de contextualização histórica e documental, mas que podem ser implementadas numa segunda fase de desenvolvimento.
* **Baixa (Desejável):** Funcionalidades de melhoria estética ou otimizações secundárias (não aplicadas nesta tabela base).

## Requisitos Não-Funcionais

# Engenharia de Requisitos - Cartografia Participativa Quilombola
## Especificação de Requisitos Não Funcionais (RNF) com Critérios de Verificação

A tabela abaixo apresenta os requisitos não funcionais acrescidos dos **Critérios de Aceitação/Verificação**. Na Engenharia de Requisitos, estes critérios são fundamentais porque transformam descrições subjetivas (como "sistema leve" ou "interface simples") em metas numéricas e testáveis pela equipa de Controle de Qualidade (QA).

| Identificador | Categoria (ISO 25010) | Nome | Descrição | Prioridade | Critérios de Aceitação / Verificação |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **RNF-001** | Usabilidade (Operabilidade) | Interface de Alta Usabilidade (Foco em Idosos) | A interface do sistema deve ser extremamente simples e intuitiva, contendo botões grandes, ícones ilustrativos e poucos passos para a execução de tarefas, garantindo o uso por anciãos com baixa literacia digital. | **Alta** | • O fluxo principal de marcação de pontos não deve exceder **3 cliques/toques** desde a tela inicial.<br>• Todos os elementos interativos (botões) devem ter uma área de toque mínima de **48x48px**.<br>• 100% dos ícones de navegação devem possuir um rótulo de texto descritivo logo abaixo ou ao lado. |
| **RNF-002** | Usabilidade (Acessibilidade) | Mecanismos de Acessibilidade Visual | O sistema deve possuir suporte nativo para alto contraste e controlo de tamanho de fonte, garantindo que os elementos textuais sejam legíveis para pessoas com dificuldades visuais. | **Alta** | • O sistema deve atingir a conformidade nível **AA da WCAG 2.1**.<br>• No modo de alto contraste, a proporção de contraste entre texto e fundo deve ser de, no mínimo, **7:1**.<br>• O redimensionamento do texto deve permitir um aumento de até **200%** sem quebrar o layout ou sobrepor elementos. |
| **RNF-003** | Eficiência de Desempenho | Otimização para Conexões Lentas | O sistema deve ser leve e realizar a compressão automática de imagens e áudios no upload, além de utilizar carregamento sob demanda (*lazy loading*), para operar eficientemente em redes rurais 3G/4G instáveis. | **Alta** | • O tempo de carregamento da página inicial não deve passar de **5 segundos** em conexões simuladas de 3G (300 Kbps).<br>• Imagens carregadas devem ser compactadas automaticamente no cliente (browser/app) para um tamanho máximo de **200 KB** antes do envio ao servidor.<br>• O consumo de dados de áudio deve ser otimizado através da conversão para o formato `.ogg` ou `.aac` de baixa taxa de bits. |
| **RNF-004** | Portabilidade (Adaptabilidade) | Design Totalmente Responsivo | O sistema deve ser planeado e otimizado prioritariamente para ecrãs/telas de dispositivos móveis (smartphones), assegurando a fidelidade visual e facilidade de toque. | **Alta** | • O sistema não deve apresentar barras de rolagem horizontal em resoluções de tela a partir de **320px** de largura.<br>• Passar sem erros na ferramenta oficial *Lighthouse (Mobile)* da Google com nota de desempenho/acessibilidade superior a **90/100**. |

---

### Importância desta coluna para o projeto:
* **Testabilidade:** O programador sabe exatamente o limite técnico que deve atingir (ex: comprimir a imagem para menos de 200 KB).
* **Homologação com a Comunidade:** Facilita a criação de testes de usabilidade reais com os anciãos da comunidade de Itapecuru-Mirim, validando se eles conseguem fechar o fluxo em até 3 toques na tela do telemóvel.