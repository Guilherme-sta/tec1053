# 03 — Implementação de chamarProxima

- **Data:** 2026-09-20
- **Autoria:** Guilherme Alves Barbosa
- **Ferramenta:** OpenCode
- **Modelo:** MiMo V2.5 Free (OpenCode Zen)
- **Trilha:** navegador
- **Requisito ou critério alvo:** RF-03, RF-04

## O que foi pedido

"Agora implemente somente chamarProxima em labs/lab-02-fila-facil/src/fila.js. Cumpra RF-03 e RF-04: atender FIFO, retirar da espera, atualizar a senha atual e contar chamadas efetivas. Fila vazia retorna null e preserva todo o estado."

## Contexto fornecido

Código com `emitirSenha` já implementado, `chamarProxima` pendente (throw).

## O que veio

Função que faz `shift()` no `aguardando`, atribui a `atual`, incrementa `totalChamadas`. Caso vazio retorna `null` sem alterar nada.

## O que eu fiz com isso

Apliquei no arquivo, executei os testes no navegador. RF-03 e RF-04 aprovados.
