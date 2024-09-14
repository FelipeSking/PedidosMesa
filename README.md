# Sistema de Pedidos de Restaurante

Este é um projeto simples de um **Sistema de Pedidos de Restaurante** feito em HTML, CSS e JavaScript. Ele permite que os usuários façam pedidos de diferentes categorias de produtos (bebidas, entradas, pratos, drinks) e enviem o pedido via WhatsApp.

## Funcionalidades

- Visualização de produtos separados por categorias: Bebidas, Entradas, Pratos e Drinks.
- Adição de produtos ao carrinho de compras.
- Remoção de produtos do carrinho.
- Cálculo automático do total do pedido.
- Envio de pedidos via WhatsApp.

## Tecnologias Utilizadas

- **HTML5**: Para a estrutura básica do site.
- **CSS3**: Para o estilo da página e layout.
- **JavaScript**: Para a lógica de manipulação do carrinho e produtos.
- **WhatsApp API**: Para o envio dos pedidos diretamente para um número de WhatsApp.

## Como Usar

### 1. Clonar o repositório

Clone este repositório em sua máquina local:
```bash
git clone https://github.com/FelipeSking/PedidoMesa.git
```
### 2. Abrir o projeto
Basta abrir o arquivo index.html no navegador para começar a usar o sistema.

3. Configurar o número de WhatsApp
No arquivo index.html, substitua SEU_NUMERO_AQUI pela URL do seu número de WhatsApp no seguinte trecho:

javascript
Copiar código
const whatsappURL = `https://wa.me/SEU_NUMERO_AQUI?text=${encodeURIComponent(mensagem)}`;
Exemplo:

javascript
Copiar código
const whatsappURL = `https://wa.me/5527999999999?text=${encodeURIComponent(mensagem)}`;
Agora, o sistema enviará o pedido diretamente para esse número via WhatsApp.

4. Personalizar os Produtos
No arquivo index.html, você pode editar a lista de produtos disponíveis. Para adicionar ou modificar um produto, ajuste o objeto produtos da seguinte forma:

javascript
Copiar código
const produtos = [
  { id: 1, nome: 'Hambúrguer', preco: 15.00, categoria: 'pratos', imagem: 'link-da-imagem' },
  { id: 2, nome: 'Pizza', preco: 30.00, categoria: 'pratos', imagem: 'link-da-imagem' },
  // Adicione mais produtos aqui
];
5. Personalizar as Categorias
Você pode organizar os produtos nas seguintes categorias: bebidas, entradas, pratos, drinks.

6. Adicionar imagens aos produtos
Para cada produto, adicione a URL de uma imagem relevante no campo imagem do objeto do produto. Certifique-se de que o link da imagem seja válido.

javascript
Copiar código
imagem: 'https://via.placeholder.com/80'


Observações:

Este é um projeto simples e voltado para aprendizado. Para usá-lo em produção, é recomendável integrar com um backend e banco de dados.
O envio de mensagens via WhatsApp só funciona com números válidos no formato internacional.
Contribuições
Fique à vontade para enviar pull requests, relatar problemas ou sugerir melhorias!






