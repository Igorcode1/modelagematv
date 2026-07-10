# 🗣️ Nossa Fala: Explicando os Desenhos do Mapa Falante

E aí, pessoal! Professor, comunidade, tudo bem? 

A gente desenhou uns mapas diferentes para mostrar como o nosso aplicativo vai funcionar. Não são mapas de terra, mas mapas de ideias, que mostram como as coisas se encaixam. Sabe aquela regra que diz que desenhar é bom, mas explicar o *porquê* é melhor ainda? É exatamente isso que vamos fazer aqui: trazer as nuances e os motivos por trás de cada linha.

---

## 1. O Mapa das Visitas (Diagrama de Contexto)

Imagine que o nosso aplicativo é uma casa nova no meio da comunidade. Esse primeiro desenho mostra quem vem visitar a casa e o que eles trazem ou levam.

* **Para quem é:** Para o **Líder Comunitário** e o **Pesquisador** (que vão alimentar o mapa com histórias) e para o **Visitante Geral** (que vem para aprender e consultar o acervo).
* **O que ele faz:** O aplicativo se conecta com a **API de Mapas** (OpenStreetMap / Leaflet, que mostra as coordenadas na tela) e com o **Cadastro da Fundação Palmares** (para validação de dados de certificação pública).
* **O Porquê Técnico (A Regra de Ouro):** A gente precisa desse desenho para enxergar o sistema de fora. Ele prova que o aplicativo não é isolado; ele depende de serviços externos de mapas e de bases oficiais para garantir a legitimidade dos dados e a navegação geográfica.

---

## 2. O Mapa do Fazer (Diagrama de Casos de Uso)

Esse desenho é como a divisão de tarefas de um mutirão. Ele mostra o que cada papel dentro da comunidade consegue acionar no aplicativo, organizado de um jeito limpo para ninguém se perder nas linhas.

* **As Nossas Pessoas (Atores):** Temos o **Ancião / Guardião**, o **Trabalhador da Terra**, o **Estudante Parceiro** e o **Jovem da Comunidade**.
* **O que cada um faz:**
    * O **Ancião** e o **Trabalhador** alimentam a memória viva: registram a **História Oral**, os **Pontos Culturais** (festas, lugares sagrados) e as **Áreas de Sustento** (roça, pesca).
    * O **Estudante** mapeia as **Zonas de Sinal** e o **Jovem** entra com o **Apoio Digital**, ajudando quem tem mais dificuldade com o celular.
* **O Coração do Sistema:** Reparou que quase tudo aponta para o **Visualizar com Áudio**? Isso é uma ligação técnica de inclusão. Significa que a história, a cultura e o sustento se completam de forma contínua com o som.
* **O Porquê Técnico (A Regra de Ouro):** O desenho mostra as ações, mas o texto explica a nuance: a comunidade é fortemente baseada na **tradição oral**. O aplicativo *precisa* do áudio e de uma interface visual simples porque o conhecimento é falado, e o sistema deve ser inclusivo para os mais velhos que dominam a história, mas não a tecnologia.

---

## 3. O Roteiro da Criação (Diagrama de Atividades)

Esse último desenho é o passo a passo do nosso processo de trabalho, desde a saída a campo até o resultado final.

* **O Início e a Escuta:** Começamos definindo os objetivos e preparando cadernos e gravadores. Depois, o fluxo se divide: se for com os **Anciãos**, colhemos histórias de fundação e lugares sagrados; se for com os **Trabalhadores e Jovens**, focamos na lida diária e no mapeamento das dificuldades com o celular.
* **O Desafio da Conectividade:** Aqui está uma regra de negócio crucial. O fluxo testa se a internet funciona no local. Se sim, marca o ponto com sinal bom; se não, marca onde o sinal some e ativa a configuração para o **funcionamento offline**.
* **A Entrega:** No fim, juntamos todas as peças para gerar o **Mapa Falante** (com botões grandes e áudios), protegendo essa história para as próximas gerações.
* **O Porquê Técnico (A Regra de Ouro):** A grande nuance que o desenho não explica sozinho é a **restrição de infraestrutura**. O aplicativo *não pode* depender de internet constante para salvar os dados. O armazenamento local e a sincronização posterior (modo offline) são requisitos técnicos obrigatórios devido à realidade geográfica do território quilombola.

---

É isso, gente! Esses desenhos são os nossos guias para garantir que o Mapa Falante seja feito com o rigor técnico que o professor exige e com o respeito e utilidade que a comunidade merece. Obrigado!