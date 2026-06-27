# Shopify Snippets Library

Biblioteca de snippets Liquid reutilizáveis para customizações comuns em lojas Shopify. Todos os exemplos usam placeholders para que possam ser adaptados com segurança em qualquer projeto.

## Snippets incluídos

### 1. Botão WhatsApp (`snippets/WhatsApp-Button.liquid`)
Adiciona um botão flutuante de contato via WhatsApp na loja.
- Botão redondo com ícone do WhatsApp
- Número e mensagem customizáveis
- Responsivo e fácil de estilizar com CSS

```liquid
{% render 'WhatsApp-Button' %}
```

### 2. Lista de Eventos — Listras Horizontais (`snippets/events-list.liquid`)
Exibe uma lista de eventos futuros em layout de faixas horizontais.
- Detecção de locale (BR e outros)
- Exibe data e título em PT/EN conforme o idioma da loja
- Design responsivo com pill de data estilizado

```liquid
{% render 'events-list' %}
```

### 3. Barra de Frete Grátis (`snippets/free-shipping-bar.liquid`)
Mostra uma barra de progresso incentivando o cliente a atingir o valor mínimo para frete grátis.
- Cálculo dinâmico baseado no total do carrinho
- Threshold e mensagens customizáveis
- Barra animada e responsiva

```liquid
{% render 'free-shipping-bar' %}
```

### 4. Embed de Evento ao Vivo (`snippets/live-event.liquid`)
Incorpora um evento ao vivo (ex: stream no Vimeo) com suporte multilíngue e formulário de lembrete.
- Detecção de locale (BR e outros)
- Título, descrição, data e detalhes via placeholders
- Integração com formulário de newsletter

```liquid
{% render 'live-event' %}
```

### 5. Card de Upsell (`snippets/product-upsell-card.liquid`)
Sugere produtos relacionados para aumentar o ticket médio.
- Puxa dados do produto dinamicamente via handle
- Exibe imagem, título e preço
- Card estilizado com botão de adicionar ao carrinho

```liquid
{% render 'product-upsell-card' %}
```

### 6. Contador Regressivo de Promoção (`snippets/promo-countdown-timer.liquid`)
Cria urgência com um timer regressivo para campanhas promocionais.
- Data de encerramento configurável
- Countdown em tempo real (dias, horas, minutos, segundos)
- Design moderno e fácil de reutilizar

```liquid
{% render 'promo-countdown-timer' %}
```

## Observações
Todas as datas, títulos e links são placeholders — substitua pelos dados reais do seu projeto. Os snippets foram desenvolvidos para ser genéricos e reutilizáveis, podendo ser combinados em temas Shopify customizados.

## Licença
MIT License — livre para usar, modificar e distribuir.
