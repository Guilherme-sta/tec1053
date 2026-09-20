# 04 — Implementação de reiniciarFila

- **Data:** 2026-09-20
- **Autoria:** Guilherme Alves Barbosa
- **Ferramenta:** OpenCode
- **Modelo:** MiMo V2.5 Free (OpenCode Zen)
- **Trilha:** navegador
- **Requisito ou critério alvo:** RF-05

## O que foi pedido

"Implemente somente reiniciarFila em labs/lab-02-fila-facil/src/fila.js, conforme RF-05. Restaure os quatro campos no mesmo objeto recebido. A confirmação já é feita pela interface; não coloque confirm(), HTML ou eventos nesta função."

## Contexto fornecido

Código com `emitirSenha` e `chamarProxima` já implementados, `reiniciarFila` pendente (throw).

## O que veio

Função que atribui valores iniciais aos quatro campos no mesmo objeto: `aguardando=[]`, `atual=null`, `totalChamadas=0`, `proximaSenha=1`.

## O que eu fiz com isso

Apliquei no arquivo, executei os testes no navegador. RF-05 aprovado. Todos os 24 testes passaram.
