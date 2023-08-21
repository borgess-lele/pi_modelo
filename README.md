# Projeto Integrador - Venda e Estoque de Loja

Um Projeto pensado na venda de mercadorias presencial e também controle de estoque.

Cadastre seu projeto nesse [link](https://docs.google.com/spreadsheets/d/1V_1h6hJ3cNLK5eY7Hy5B8hQDxYy8GcZNHyFfC2HdawI/edit?usp=sharing).

Professores: [Marco André Mendes](github.com/marcoandre) e [Alann Perini](https://github.com/AlannKPerini).

Equipe:
- [Letícia](https://github.com/borgess-lele)

  
Links do projeto:
(*Coloque aqui os links para a documentação do projeto e os repositórios e plubicação do backend e frontend.*)
-   [Documentação](https://github.com/borgess-lele/pi_modelo)
-   Backend: [Repositório](github.com/marcoandre/pi-backend) e [Publicação](https://pi-backend.herokuapp.com/)
-   Frontend[Repositório](github.com/marcoandre/pi-frontend) e [Publicação](https://pi-frontend.herokuapp.com/)

**1.1.1 Ponto de Vendas (PDV)**

**Gerenciamento de vendas para uma padaria**

O Gerenciamento de Vendas irá incluir um controle de estoque, com as mercadorias que determinada loja vende, neste controle de vendas terá permissão para que o funcionário consiga fazer seu login e realizar uma venda e também um outro login pra que ele consiga ter acesso ao estoque, onde poderá cadastrar novos produtos, excluir produtos que não existem mais na loja, e visualizar quantos produtos ainda restam nesta determinada loja. Teremos também uma tela onde o consumidor poderá fazer sua encomenda online, escolhendo seu produo, forma de pagamento e retirada do produto.

# 2. Situação Problema

Doce Trufa é uma empresa de trufas que faz a venda de doces e existe desde 207, o Dono se chama Gislaine Borges, ela tem 42 anos e é quem gerencia este empreendimento, dentro da empresa existem hoje 3 funcionários que trabalham para o bom funcionamento da empresa, que produzem os docces e realizam as vendas dos mesmos. O dono da empresa sempre pensa em estrátegias e soluçoes para melhorias internas e externas de sua empresa e também para facilitar o andamento das coisas. 

Atualmente na Doce Trufa existem certos problemas como por exemplo: não exite um sistema para fazer as vendas corretamente, então é feito todas as vendas manualmente e com isso certamente não exite um controle de estoque, onde só se sabe que o produto está em falta quando o cliente vem atrás do mesmo.

# 3. Descrição da proposta

O foco deste software é para que facilite as vendas e o controle de estoque da empresa;

As pessoas que terão acesso a este sistema será somente quem trabalha na loja e o dono;

Poderá ser feito no sotware venda de produtos, cadastramento de funcionários novos e controle de mercadoria.

Dentro destes problemas que notamos, a intenção é fazer um sistema onde cada funcionário tenha seu login e senha para realizar suas vendas no caixa e também que cada um tenha um login de acesso ao estoque para que os mesmos consigam cadastrar novos produtos, excluir produtos que estão em inatividade na loja e para ter o controle de quando está prestes a acabar determinado produto, e também a realização de novos cadastro de login e senha quando um funcionário novo for contratado, para que ele não necessite usar o login e a senha de outra pessoa. Precisará ser desenvolvido também uma tela na qual  liente poderá realizar sua compra online, escolhendo sua mercadoria, sua forma de pagamento e forma como deseja retira sua encomenda.

# 4. Regras de negócio

- **RN01 – Criação da Venda:** Para iniciar uma venda no caixa, é necessário primeiro abrir logar ao sistema.
- **RN02 – Inserir Produtos:** Para inserir um produto na venda, é necessário que o produto esteja cadastrado no sistema e que a quantia comprada seja acima de zero.
- **RN03 – Acesso ao Estoque:** Para acessar ao estoque, é necessário fazer o login.
- **RN04 – Cadastro de novos produtos:** Para realizar cadastro de um novo produtos é necessário ter um produto novo e as informaçoes do mesmo.
- **RN05 – Venda online:** Para que o clientte consiiga realizar seu pedido, é necessário que o mesmo preencha os campos obrigtório como: Doce que deseja, forma de pagamento, forma de retirada, nome e telefone.
- **RN06- Bloqueio de Compra de Produtos Esgotados:** O sistema deve impedir que os clientes comprem produtos que não estejam disponíveis em estoque.
  
 
# 5. Requisitos funcionais

**Entradas:**

- **R.F. 01 - Gerenciamento de Produtos:(crud)** Adicionar, editar e remover produtos do catálogo, incluindo descrições, preços, imagens e opções de personalização.
  - **Dados necessários:** login e senha
  - **Usuários:** todos os níveis de usuário.

- **R.F. 02 - Gerenciamento de Cliente:(crud)** Adicionar, editar e remover produtos do carrinho, fazer compras, escolher forma de pagamento e enderço para entrega 
  - **Dados necessários:** cadastro
  - **Usuários:** todos os clientes

**Processamento:**

- **R.F. 03 - Autenticação de usuário:** tem como propósito autenticar o acesso ao sistema, verificando se o usuário pode acessá-lo e, caso possa, o direcionando para a página principal de seu perfil de acesso. 
  - **Dados necessários:** login, senha. 
  - **Usuários:** todos os níveis de usuário.

- **R.F. 04 - Controle de entrada Estoque:** Manter um registro preciso dos níveis de estoque, atualizando-os automaticamente conforme as vendas são feitas.
  - **Dados necessários:** produto,quantidade
  - **Usuários:** todos os níveis de usuário.
]

- **R.F. 05 - Gestão de Pedidos:** Visualizar, processar e atualizar o status dos pedidos recebidos, desde o pagamento até o envio.
  - **Dados necessários:** login e senha.
  - **Usuários:** todos os níveis de usuário.


**Saídas:**


- **R.F. 06 - Histórico de Compras cliente:** Permitir que os clientes acessem um histórico de suas compras anteriores, incluindo detalhes de produtos e datas.
  - **Dados necessários:** data inicial , data final , pedidos
  - **Usuários:** cliente/administrador

- **R.F. 07- Relatórios de Vendas:** Gerar relatórios detalhados sobre as vendas, incluindo informações sobre produtos mais vendidos, receitas e tendências.
  - **Dados necessários:** login e senha.
  - **Usuários:** todos os níveis de usuário.

# 6. Requisitos não funcionais

**Sistema de Vendas**:
- R.N.F. 01 - Navegador homologado: O sistema deverá ser homologado somente para o navegador Google Chrome.
- R.N.F. 02 - Processador: É recomendado para o sistema  no mínimo um processador Intel i3, similar ou superior a geração 7100 ou AMD Ryzen 3 da geração similar ou superior ao 3100, para que o servidor funcione em sua melhor performance.
- R.N.F. 03 - Memória RAM: é recomendável que o sistema possua no mínimo 2GB de Ram para melhor performance.
- R.N.F. 04 - Arquitetura: A arquitetura que será utilizada para criação do sistema será Rest.
- R.N.F. 05 - Conexão com banco de dados: Para conexão com o banco de dados, o sistema utilizará a ferramenta de MySQL Connector.
- R.N.F. 06- Banco de dados: O sistema será implementado com o banco de dados MySQL.
- R.N.F. 07 - Implementação: O sistema deverá ser desenvolvido com linguagem ...........
- R.N.F. 08 - Segurança: Ficará a critério do responsável do estabelecimento a segurança dos acessos ao sistema, tendo consciência das pessoas que possua permissão para acesso.
- R.N.F. 09 - Ambiente de Desenvolvimento Integrado (IDE): Para criação do sistema, será utilizado django, view, react-native.
- R.N.F. 10 - Disponibilidade: O sistema irá atender 99% do tempo de uso, somente ocorreria problemas de cadastro, remoção, inserção ou alteração em casos de falta de rede ou energia.
- R.N.F. 11 - Legais: O sistema deve atender às exigências da LGPD (Leis Gerais da Proteção de Dados).