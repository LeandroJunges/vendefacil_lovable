# VendeFácil

> Sua vitrine online. Seus pedidos. Seu negócio.

O **VendeFácil** é um MVP de uma ferramenta digital criada para pequenos negócios que vendem produtos artesanais, personalizados ou sob encomenda.

A proposta é simples: permitir que o empreendedor tenha uma **página própria para divulgar seus produtos e receber solicitações de pedidos**, enquanto utiliza um painel para organizar leads, clientes e pedidos.

O projeto foi desenvolvido como parte do desafio de construção de um MVP, utilizando **ChatGPT como apoio na validação e definição do produto** e **Lovable para construção da aplicação**.

---

## 📌 A dor

Pequenos negócios artesanais frequentemente começam suas vendas utilizando ferramentas que já possuem:

* Instagram;
* WhatsApp;
* Shopee;
* planilhas;
* cadernos;
* anotações;
* mensagens espalhadas em diferentes conversas.

Isso funciona enquanto o volume de pedidos é pequeno, mas pode dificultar a organização conforme o negócio cresce.

Um cliente pode descobrir um produto pelo Instagram, tirar dúvidas pelo WhatsApp e depois ter seu pedido acompanhado manualmente pelo empreendedor.

A hipótese que deu origem ao VendeFácil foi:

> **Pequenos empreendedores precisam de uma maneira simples de divulgar seus produtos e organizar os contatos, clientes e pedidos que hoje ficam espalhados entre diferentes canais.**

### Por que essa dor chamou minha atenção?

A ideia surgiu observando um cenário próximo: pequenos negócios que produzem seus próprios produtos e utilizam redes sociais e marketplaces para alcançar clientes, mas ainda dependem muito de conversas manuais pelo WhatsApp para concluir e acompanhar as vendas.

Em vez de tentar criar outro marketplace ou um e-commerce completo, a proposta foi criar uma camada simples entre **divulgação, geração do pedido e organização da venda**.

---

# 💡 A ideia

O VendeFácil combina duas experiências:

### Para o cliente

Uma página pública do negócio que funciona como uma pequena vitrine digital.

O empreendedor pode divulgar o link:

```text
Instagram
    ↓
Página do VendeFácil
    ↓
Produtos
    ↓
Solicitação de pedido/orçamento
    ↓
WhatsApp
```

### Para o empreendedor

Um painel para acompanhar o que acontece depois:

```text
Lead
 ↓
Contato
 ↓
Negociação
 ↓
Cliente
 ↓
Pedido
 ↓
Produção
 ↓
Entrega
```

A proposta não é substituir plataformas como Shopee nem criar um ERP completo.

O foco é oferecer uma ferramenta simples para pequenos negócios que querem ter uma **presença digital própria e organizar suas vendas**.

---

# 🎯 Tese do MVP

A principal tese que o MVP busca testar é:

> **Pequenos empreendedores podem perceber valor em ter uma página própria para divulgar seus produtos e receber pedidos, combinada com uma ferramenta simples para organizar leads, clientes e pedidos.**

O MVP não tenta provar que todos os pequenos negócios precisam de um CRM.

Ele busca validar principalmente se existe interesse em uma solução que una:

**Vitrine digital + geração de pedidos + organização comercial.**

---

# 🧪 Hipóteses que o MVP precisa testar

| Hipótese                                                                     | Como o MVP testa                                                             |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| Pequenos negócios precisam de uma página própria para divulgar seus produtos | Cada negócio possui uma página pública compartilhável                        |
| O empreendedor pode utilizar essa página como link de divulgação             | O sistema disponibiliza um link público para compartilhamento                |
| Clientes podem demonstrar interesse sem criar uma conta                      | O formulário público não exige cadastro                                      |
| WhatsApp continua sendo importante para concluir a venda                     | O formulário gera uma mensagem pré-preenchida para WhatsApp                  |
| O empreendedor precisa organizar os contatos recebidos                       | Leads ficam disponíveis no painel administrativo                             |
| Um lead pode evoluir para cliente                                            | O painel permite converter leads em clientes                                 |
| O empreendedor precisa acompanhar o pedido após a negociação                 | O sistema possui gestão de pedidos e status                                  |
| Uma solução simples pode ser suficiente inicialmente                         | O MVP evita checkout, pagamentos, estoque e outras funcionalidades complexas |

---

# 📊 Mercado

O mercado considerado inicialmente é formado por pequenos negócios que trabalham com produtos ou serviços artesanais, personalizados ou sob encomenda.

Exemplos:

* sabonetes artesanais;
* lembrancinhas;
* produtos personalizados;
* doces;
* produtos para festas;
* artesanato;
* brindes;
* pequenos produtores;
* negócios que recebem pedidos pelo WhatsApp e Instagram.

## TAM

**[Preencher com o cálculo realizado durante a etapa de validação.]**

O TAM representa o mercado total potencial relacionado à solução.

## SAM

**[Preencher com o recorte de mercado escolhido para o produto.]**

O SAM representa a parcela do mercado que pode ser atendida considerando o público e o posicionamento inicial do VendeFácil.

## SOM

**[Preencher com a estimativa inicial de clientes que poderia ser alcançada na fase inicial.]**

O SOM representa a parcela que poderia ser alcançada inicialmente considerando os recursos disponíveis e a estratégia de aquisição.

> Os valores acima devem ser substituídos pelos números obtidos durante a validação da ideia.

---

# 🧩 Business Model Canvas

| Bloco                           | VendeFácil                                                                                                                        |
| ------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Segmentos de clientes**       | Pequenos empreendedores, artesãos, produtores de itens personalizados, negócios caseiros e profissionais que vendem sob encomenda |
| **Proposta de valor**           | Criar uma vitrine digital própria e organizar leads, clientes e pedidos em um único lugar                                         |
| **Canais**                      | Instagram, WhatsApp, indicação, redes sociais e divulgação direta                                                                 |
| **Relacionamento com clientes** | Self-service, página pública, suporte e onboarding simples                                                                        |
| **Fontes de receita**           | Assinatura do SaaS                                                                                                                |
| **Recursos principais**         | Aplicação web, infraestrutura, banco de dados e plataforma de autenticação                                                        |
| **Atividades principais**       | Desenvolvimento, manutenção, aquisição de clientes e evolução do produto                                                          |
| **Parcerias principais**        | Serviços de infraestrutura, comunicação e ferramentas utilizadas pelos pequenos negócios                                          |
| **Estrutura de custos**         | Infraestrutura, banco de dados, serviços de terceiros, desenvolvimento e aquisição de clientes                                    |

---

# 🚀 O MVP

O MVP foi construído com foco em validar o fluxo comercial completo.

## Fluxo público

```text
Página pública
     ↓
Visualização dos produtos
     ↓
"Tenho interesse"
     ↓
Formulário
     ↓
Lead criado
     ↓
WhatsApp
```

## Fluxo administrativo

```text
Lead
 ↓
Contato realizado
 ↓
Negociação
 ↓
Conversão
 ↓
Cliente
 ↓
Pedido
 ↓
Acompanhamento
 ↓
Entrega
```

---

# ✨ Funcionalidades

## Página pública

Cada negócio pode possuir uma página própria com:

* nome do negócio;
* descrição;
* logo;
* redes sociais;
* WhatsApp;
* produtos;
* imagens;
* preços, quando aplicável;
* botão para solicitar pedido/orçamento.

A página foi pensada principalmente para acesso pelo celular e compartilhamento através de Instagram e WhatsApp.

---

## Catálogo

O empreendedor pode cadastrar produtos para exibição na página pública.

Cada produto pode possuir:

* nome;
* descrição;
* imagem;
* preço;
* categoria;
* disponibilidade;
* opção de trabalhar com orçamento.

---

## Solicitação de pedido

O visitante pode demonstrar interesse em um produto através de um formulário.

Informações coletadas:

* nome;
* WhatsApp;
* produto;
* quantidade;
* data desejada;
* observações.

Após o envio, o lead é registrado no painel administrativo.

Também é possível continuar a conversa pelo WhatsApp através de uma mensagem pré-preenchida.

---

# 📋 Gestão de Leads

O empreendedor pode acompanhar os leads recebidos através dos seguintes status:

* Novo;
* Contato realizado;
* Em negociação;
* Convertido;
* Perdido.

Também é possível:

* visualizar informações;
* editar o lead;
* alterar status;
* converter em cliente;
* criar pedido.

---

# 👥 Gestão de Clientes

Os clientes possuem:

* nome;
* WhatsApp;
* e-mail;
* observações;
* data de cadastro.

Também é possível visualizar o histórico básico relacionado ao cliente e seus pedidos.

---

# 📦 Gestão de Pedidos

Os pedidos possuem:

* cliente;
* produto/serviço;
* quantidade;
* valor;
* data desejada;
* observações;
* status.

Status disponíveis:

* Orçamento;
* Aguardando confirmação;
* Confirmado;
* Em produção;
* Pronto;
* Entregue;
* Cancelado.

---

# 📊 Dashboard

O painel administrativo apresenta uma visão resumida do negócio:

* novos leads;
* leads em negociação;
* pedidos em aberto;
* pedidos concluídos;
* valor estimado em vendas;
* leads recentes;
* pedidos recentes.

A intenção é permitir que o empreendedor tenha uma visão rápida do estado atual das vendas.

---

# 📱 Experiência mobile

O produto foi desenvolvido pensando especialmente no contexto de pequenos empreendedores que utilizam o celular como principal ferramenta de trabalho.

A página pública prioriza:

* produtos;
* imagens;
* informações essenciais;
* botão de interesse;
* WhatsApp.

A aplicação administrativa também possui layout responsivo para utilização em dispositivos móveis.

---

# 🛠️ Stack e construção

O MVP foi construído utilizando o **Lovable**, com o backend e banco disponibilizados pelo **Lovable Cloud**, conforme proposto no desafio.

O ChatGPT foi utilizado como apoio durante:

* definição da ideia;
* estruturação da proposta de valor;
* levantamento das hipóteses;
* definição do fluxo do MVP;
* elaboração do Business Model Canvas;
* criação do mega prompt;
* análise da experiência;
* criação dos prompts de correção e evolução.

O Lovable foi utilizado para transformar essa especificação em uma aplicação funcional.

---

# 🤖 O uso de IA como co-founder

O processo não consistiu apenas em pedir para uma IA "criar um sistema".

A IA foi utilizada como uma ferramenta para discutir a ideia antes da implementação.

O processo foi:

```text
Dor observada
     ↓
Discussão da ideia
     ↓
Definição da proposta
     ↓
Hipóteses
     ↓
Business Model Canvas
     ↓
Definição do MVP
     ↓
Mega Prompt
     ↓
Lovable
     ↓
Teste da aplicação
     ↓
Identificação de problemas
     ↓
Prompt de correção
     ↓
Nova validação
```

Esse processo ajudou a reduzir a quantidade de decisões tomadas diretamente durante a implementação.

---

# 📝 Mega Prompt

O mega prompt utilizado para construir o MVP foi estruturado em Markdown e definiu:

* contexto do negócio;
* objetivo do produto;
* landing page;
* formulário de leads;
* dashboard;
* gestão de leads;
* clientes;
* pedidos;
* configurações;
* autenticação;
* banco de dados;
* segurança;
* responsividade;
* critérios de aceitação.

O prompt completo pode ser encontrado em:

**[`docs/mega-prompt.md`](docs/mega-prompt.md)**

> Caso você ainda não tenha criado esse arquivo no repositório, salve o prompt utilizado no Lovable nesse caminho antes de publicar o projeto.

---

# 🔄 Evolução após os primeiros testes

Após analisar a primeira versão construída pelo Lovable, identifiquei que o produto estava sendo apresentado principalmente como um **CRM**.

Isso não representava completamente a ideia que eu queria testar.

A partir dessa análise, a proposta foi ajustada.

### Antes

```text
CRM para pequenos negócios
```

### Depois

```text
Vitrine digital
      +
Recebimento de pedidos
      +
Organização das vendas
```

Essa mudança levou à criação da página pública de cada negócio.

O objetivo passou a ser permitir que o empreendedor possa divulgar um único link no Instagram, WhatsApp ou outros canais e direcionar o cliente para seus produtos.

---

# 🎨 Identidade visual

A primeira versão apresentava uma estética mais próxima de um dashboard SaaS tradicional.

Durante a revisão, foi identificada a necessidade de diferenciar melhor:

### Área pública

Mais:

* visual;
* criativa;
* acolhedora;
* comercial;
* orientada a produtos.

### Área administrativa

Mais:

* objetiva;
* organizada;
* funcional;
* orientada à gestão.

A nova direção visual busca combinar tecnologia com a personalidade dos pequenos negócios artesanais, evitando a aparência de um ERP corporativo.

---

# 🧪 O que ficou manual de propósito

O objetivo do MVP é validar a tese antes de investir em funcionalidades mais complexas.

Por isso, algumas etapas permanecem manuais.

### WhatsApp

A aplicação não utiliza a API oficial do WhatsApp.

O sistema apenas gera um link `wa.me` com uma mensagem pré-preenchida.

A conversa e o fechamento da venda continuam acontecendo manualmente.

### Pagamento

Não existe checkout ou pagamento integrado.

O pagamento pode ser combinado diretamente entre empreendedor e cliente.

### Operação

Produção, estoque, entrega e logística continuam sendo responsabilidade do empreendedor.

### Marketplace

O VendeFácil não possui marketplace próprio.

A página pública pertence ao próprio negócio.

---

# 🚫 O que ficou fora do MVP

Para evitar transformar o projeto em uma plataforma grande demais, ficaram fora do escopo:

* emissão de nota fiscal;
* estoque;
* financeiro completo;
* integração bancária;
* gateway de pagamento;
* WhatsApp API;
* marketplace;
* cálculo de frete;
* logística;
* automações complexas;
* chatbot.

Essas funcionalidades podem ser avaliadas posteriormente caso a hipótese principal seja validada.

---

# 📸 Demonstração

## Landing Page

![Landing Page](docs/screenshots/landing-page.png)

## Página pública do negócio

![Página pública](docs/screenshots/pagina-publica.png)

## Dashboard

![Dashboard](docs/screenshots/dashboard.png)

## Gestão de Leads

![Leads](docs/screenshots/leads.png)

## Gestão de Pedidos

![Pedidos](docs/screenshots/pedidos.png)

> Substitua os caminhos acima pelos screenshots reais da aplicação antes de publicar o repositório.

---

# 🌐 Aplicação publicada

**URL:** [COLOCAR URL DA APLICAÇÃO PUBLICADA]

---

# 💻 Repositório

**GitHub:** [COLOCAR URL DO REPOSITÓRIO]

---

# 🔮 Próximos passos

Caso a hipótese seja validada com os primeiros usuários, algumas possibilidades de evolução são:

* alertas de novos leads por e-mail;
* integração com Resend;
* melhorias no compartilhamento;
* domínio personalizado para cada negócio;
* planos pagos;
* integração com Stripe;
* automações;
* integração com WhatsApp;
* chatbot;
* analytics da página pública;
* personalização visual da vitrine;
* integração com outros canais de venda.

A prioridade dessas funcionalidades dependeria do feedback obtido durante a validação com usuários reais.

---

# 📚 Aprendizados

O principal aprendizado deste projeto foi perceber que construir um MVP não significa simplesmente construir a maior quantidade possível de funcionalidades.

O objetivo é identificar:

> **Qual é a menor experiência capaz de testar a hipótese do negócio?**

No caso do VendeFácil, isso levou à decisão de manter o fechamento da venda pelo WhatsApp, evitar pagamentos integrados e concentrar o esforço na combinação entre **página pública + geração de leads + organização das vendas**.

A IA foi utilizada como ferramenta de apoio durante esse processo, mas as decisões sobre o produto foram tomadas a partir do problema escolhido e das hipóteses que precisavam ser testadas.

---

# 🚀 Conclusão

O VendeFácil nasceu de uma dor observada em pequenos negócios que precisam conciliar divulgação, atendimento e organização das vendas utilizando diversas ferramentas.

O MVP busca testar uma proposta simples:

> **Dar ao pequeno empreendedor uma página própria para divulgar seus produtos e uma ferramenta simples para transformar os contatos recebidos em vendas organizadas.**

O próximo passo não é adicionar dezenas de funcionalidades.

É colocar o produto nas mãos de pequenos empreendedores, observar como eles utilizam a solução e descobrir se essa proposta realmente resolve uma dor relevante.
