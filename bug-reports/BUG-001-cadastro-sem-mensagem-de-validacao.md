# BUG-001: Cadastro exibe mensagem de sucesso com campos obrigatórios em branco

| Campo | Valor |
|---|---|
| Missão | 1. Primeiro contato: crie sua conta e entre no ambiente |
| Severidade | Média |
| Prioridade | Média |
| Status | Aberto |
| Ambiente | Chrome / Windows / Desktop |
| Data | 21/10/2026 |

## Pré-condições
- Usuário não autenticado

## Passos para reproduzir
1. Acessar a tela de cadastro
2. Deixar todos os campos em branco
3. Clicar no botão "Cadastrar"

## Resultado atual
O sistema exibe a mensagem de sucesso "Conta criada com sucesso! confira agora o numero de sua conta", mesmo com
os campos obrigatórios vazios. [A conta foi / não foi realmente criada: confirmar
tentando fazer login.]

## Resultado esperado
O sistema deveria impedir o envio, exibir mensagens de validação nos campos
obrigatórios e manter o usuário na tela de cadastro, sem mensagem de sucesso.

## Evidências
![Tela de cadastro exibindo mensagem de sucesso com todos os campos em branco](../evidencias/BUG-001-Cadastro-exibe-mensagem-de-sucesso-com-campos-obrigatorios-em-branco.png)

## Observações
[O mesmo comportamento ocorre quando apenas alguns campos estão em branco? Se
testou, escreva aqui. Se não, apague esta linha.]
