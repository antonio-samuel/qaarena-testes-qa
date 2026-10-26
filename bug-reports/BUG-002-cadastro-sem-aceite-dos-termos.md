# BUG-002: Sistema permite cadastro sem aceite dos termos e condições

| Campo | Valor |
|---|---|
| Missão | 2. O cadastro que não liga para os termos |
| Severidade | Média |
| Prioridade | Média |
| Status | Aberto |
| Ambiente | Chrome / Windows / Desktop |
| Data | 21/10/2026 |

## Pré-condições
- Usuário não autenticado

## Passos para reproduzir
1. Acessar a tela de cadastro
2. Preencher todos os campos com dados fictícios (CPF gerado na Massa de Dados e e-mail ainda não utilizado)
3. [Manter / Desmarcar] a opção "Li e aceito os termos"
4. Clicar em "Cadastrar"

## Resultado atual
O cadastro é concluído com sucesso sem que o usuário tenha aceitado os termos
e condições.

## Resultado esperado
O sistema deveria bloquear o cadastro e exibir uma mensagem solicitando o
aceite dos termos, mantendo o usuário na tela.

## Evidências
![Cadastro concluído com a opção de termos desmarcada](../evidencias/BUG-002-cadastro-sem-aceite-dos-termos.mp4)

## Observações
Sem aceite dos termos, a empresa não teria registro de consentimento do usuário.
