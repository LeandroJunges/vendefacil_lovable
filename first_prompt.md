# Construção de MVP — CRM para pequenos negócios artesanais

## Contexto do projeto

Quero construir um MVP de um produto SaaS chamado provisoriamente **VendeFácil**.

O produto será uma ferramenta simples de gestão comercial para pequenos negócios que fabricam e vendem produtos artesanais, personalizados ou sob encomenda.

Exemplos de negócios que podem utilizar o produto:

* sabonetes artesanais;
* lembrancinhas;
* produtos personalizados;
* itens para festas;
* doces e produtos caseiros;
* artesanato;
* brindes;
* pequenos produtores que recebem pedidos principalmente pelo WhatsApp e Instagram.

O produto não deve tentar substituir um ERP ou uma plataforma completa de e-commerce.

O objetivo do MVP é testar a seguinte hipótese:

> Pequenos produtores precisam de uma maneira simples de organizar leads, clientes, orçamentos e pedidos que hoje ficam espalhados entre WhatsApp, Instagram, cadernos e planilhas.

O MVP deve priorizar simplicidade e facilidade de uso.

---

# 1. Objetivo do produto

Criar uma aplicação web responsiva que tenha duas experiências:

### Área pública

Uma landing page para apresentar o produto e permitir que um potencial cliente de um pequeno negócio entre em contato ou solicite um orçamento.

### Área administrativa

Um painel onde o empreendedor consiga:

* visualizar leads;
* acompanhar oportunidades;
* cadastrar clientes;
* transformar leads em clientes;
* criar e acompanhar pedidos;
* visualizar informações básicas do negócio.

O sistema deve ser simples o suficiente para uma pessoa sem conhecimento técnico utilizar.

---

# 2. Landing Page

Criar uma landing page moderna, limpa e profissional.

A comunicação deve ser voltada para pequenos empreendedores que vendem produtos artesanais ou personalizados.

Headline sugerida:

> Organize suas vendas sem deixar seus clientes perdidos no WhatsApp.

Subheadline:

> Centralize seus leads, clientes, orçamentos e pedidos em um único lugar e acompanhe suas vendas do primeiro contato até a entrega.

Criar uma chamada principal:

**"Começar agora"**

E uma segunda chamada:

**"Solicitar orçamento"**

A landing page deve conter:

1. Hero;
2. problema;
3. como funciona;
4. principais recursos;
5. exemplo visual do painel;
6. chamada para ação;
7. rodapé.

Evitar linguagem de grandes empresas ou funcionalidades exageradas.

A comunicação deve transmitir que o produto foi criado para pequenos negócios.

---

# 3. Cadastro de lead

Criar um formulário público de solicitação de orçamento.

Campos:

* Nome;
* WhatsApp;
* Produto ou serviço de interesse;
* Quantidade;
* Data desejada;
* Observações.

Após o envio:

1. salvar o lead;
2. mostrar uma mensagem de sucesso;
3. disponibilizar botão para continuar a conversa pelo WhatsApp.

O botão do WhatsApp deve montar uma mensagem contendo os dados enviados pelo formulário.

Exemplo:

"Olá! Meu nome é João. Tenho interesse em 30 unidades de sabonetes artesanais para o dia 15/10. Gostaria de receber um orçamento."

Não implementar integração oficial com a API do WhatsApp neste MVP.

Utilizar apenas um link `wa.me` com mensagem pré-preenchida.

---

# 4. Área administrativa

Criar uma área administrativa protegida por autenticação.

A navegação principal deve possuir:

* Dashboard;
* Leads;
* Clientes;
* Pedidos;
* Configurações.

---

# 5. Dashboard

Criar um dashboard simples.

Exibir cards:

* Novos leads;
* Leads em negociação;
* Pedidos em aberto;
* Pedidos concluídos;
* Valor estimado em vendas.

Adicionar uma visualização simples dos leads e pedidos recentes.

Não criar gráficos complexos neste MVP.

O objetivo é permitir que o empreendedor entenda rapidamente o estado atual das vendas.

---

# 6. Gestão de Leads

Criar uma tela de leads.

Cada lead deve possuir:

* nome;
* WhatsApp;
* produto de interesse;
* quantidade;
* data desejada;
* observações;
* data de criação;
* status.

Statuses:

* Novo;
* Contato realizado;
* Em negociação;
* Convertido;
* Perdido.

Permitir:

* visualizar lead;
* editar lead;
* alterar status;
* converter lead em cliente;
* criar pedido a partir do lead.

Ao converter um lead em cliente, reutilizar automaticamente os dados já cadastrados.

Não solicitar novamente as mesmas informações.

---

# 7. Gestão de Clientes

Criar uma tela de clientes.

Campos:

* Nome;
* WhatsApp;
* E-mail;
* Observações;
* Data de cadastro.

Cada cliente deve possuir uma página ou modal de detalhes.

Mostrar:

* informações do cliente;
* pedidos anteriores;
* pedidos em aberto;
* histórico básico de relacionamento.

Permitir criar um novo pedido diretamente a partir do cliente.

---

# 8. Gestão de pedidos

Criar uma tela de pedidos.

Cada pedido deve possuir:

* cliente;
* produto/serviço;
* quantidade;
* valor;
* data desejada;
* observações;
* status.

Statuses:

* Orçamento;
* Aguardando confirmação;
* Confirmado;
* Em produção;
* Pronto;
* Entregue;
* Cancelado.

Permitir alterar o status do pedido.

Criar uma visualização clara do fluxo do pedido.

Pode utilizar uma tabela com filtros ou uma visualização estilo Kanban, desde que a interface permaneça simples.

---

# 9. Configurações

Criar uma área simples para o empreendedor configurar:

* nome do negócio;
* descrição;
* WhatsApp;
* Instagram;
* endereço;
* logo;
* mensagem padrão do WhatsApp.

Essas informações podem ser utilizadas na landing page e nas mensagens geradas.

Não implementar ainda:

* emissão de nota fiscal;
* estoque;
* financeiro completo;
* integração bancária;
* gateway de pagamento;
* integração oficial com WhatsApp;
* marketplace;
* cálculo de frete;
* logística;
* automações complexas.

Esses recursos ficam fora do escopo do MVP.

---

# 10. Banco de dados

Utilizar exclusivamente o backend e banco de dados disponibilizados pelo Lovable Cloud.

Criar uma estrutura adequada para:

* usuários;
* configuração do negócio;
* leads;
* clientes;
* pedidos.

Relacionamentos:

User/Business → Leads

User/Business → Clients

Client → Orders

Lead → Client, quando convertido.

Lead → Order, quando houver pedido originado daquele lead.

Aplicar regras de segurança para impedir que um usuário consiga visualizar dados de outro negócio.

---

# 11. Autenticação

Implementar cadastro e login.

O usuário deve conseguir:

* criar uma conta;
* entrar;
* sair;
* recuperar acesso, caso suportado pela infraestrutura padrão.

Após o login, direcionar para o Dashboard.

---

# 12. Design

O produto deve transmitir simplicidade, organização e proximidade com pequenos empreendedores.

Evitar aparência excessivamente corporativa.

Utilizar:

* bastante espaço em branco;
* cards;
* bordas suaves;
* tipografia legível;
* boa hierarquia visual;
* componentes consistentes;
* responsividade.

A interface deve funcionar bem em:

* desktop;
* tablet;
* celular.

A experiência mobile é especialmente importante porque o público provavelmente utiliza o celular para acompanhar vendas e conversar com clientes.

---

# 13. Menu

Desktop:

Dashboard | Leads | Clientes | Pedidos | Configurações

Mobile:

utilizar menu inferior ou menu lateral responsivo.

Dar destaque visual para ações importantes como:

* Novo lead;
* Novo cliente;
* Novo pedido.

---

# 14. Dados demonstrativos

Criar dados de demonstração suficientes para que o painel não fique vazio após a primeira utilização.

Exemplos de clientes:

* Mariana Souza;
* Carlos Oliveira;
* Fernanda Lima.

Exemplos de produtos:

* Kit de sabonetes;
* Lembrancinhas personalizadas;
* Kit festa;
* Brindes personalizados.

Deixar claro visualmente quando os dados forem demonstrativos.

---

# 15. Regras importantes do MVP

Não construir funcionalidades que não foram solicitadas.

Priorizar:

1. funcionamento;
2. simplicidade;
3. boa experiência de usuário;
4. responsividade;
5. segurança básica;
6. clareza do fluxo comercial.

O MVP deve permitir demonstrar este fluxo completo:

Landing Page
→ Solicitação de orçamento
→ Lead
→ Contato pelo WhatsApp
→ Negociação
→ Conversão para cliente
→ Criação de pedido
→ Acompanhamento do pedido
→ Entrega.

---

# 16. Critérios de aceitação

Considerar o MVP funcional quando for possível:

1. criar uma conta;
2. acessar o dashboard;
3. receber um lead através do formulário público;
4. visualizar o lead no painel;
5. abrir o WhatsApp com os dados do lead;
6. alterar o status do lead;
7. converter o lead em cliente;
8. criar um pedido para o cliente;
9. alterar o status do pedido;
10. visualizar o histórico do cliente;
11. acessar a aplicação pelo celular;
12. manter os dados de cada usuário isolados.

Antes de finalizar, verificar se existem erros de console, problemas de responsividade ou fluxos quebrados.

Não adicionar funcionalidades fora do escopo sem necessidade.

---

# 17. Resultado esperado

Ao final, quero ter um MVP publicável que possa ser apresentado a pequenos empreendedores reais.

O produto não precisa estar pronto para atender centenas ou milhares de empresas.

Ele precisa ser suficientemente funcional para testar a hipótese com os primeiros usuários.

Priorize uma implementação simples e funcional em vez de uma grande quantidade de funcionalidades.
