# BUG-003: Cupom QA10 aplica 5% de desconto em vez de 10%

| Campo | Valor |
|---|---|
| Missão | 6. O cupom que promete 10 e entrega 5 |
| Severidade | Alta |
| Prioridade | Alta |
| Status | Aberto |
| Ambiente | Chrome / Windows / Desktop |
| Data | 25/10/2026 |

## Pré-condições
- Usuário válido da massa de dados do ambiente
- Cupom QA10 disponível

## Passos para reproduzir
1. Fazer login com o usuário válido
2. Adicionar ao carrinho um produto de 
3. Acessar o carrinho e clicar em "Ir para checkout"
4. Inserir o cupom QA10 e clicar em "Aplicar"
5. Conferir o valor do desconto exibido

## Resultado atual
O sistema aplica desconto de 5% (R$ [valor do desconto aplicado]) sobre o
produto de R$ [valor do produto].

## Resultado esperado
O sistema deveria aplicar desconto de 10% (R$ [valor esperado]), conforme o
nome do cupom indica.

## Evidências
![Checkout exibindo desconto de 5% após aplicar o cupom QA10](../evidencias/BUG-003-checkout-qa10.png)

## Observações
- Usuário utilizado: [e-mail ou nome do usuário da massa de dados]
- O bug envolve cálculo de valor financeiro, por isso a severidade é Alta.
