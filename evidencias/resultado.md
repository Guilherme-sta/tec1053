# Resultado — Lab 02: Fila Fácil

- **Dupla:** Guilherme Alves Barbosa
- **Data:** 2026-09-20
- **Rota:** Lab 02 — Fila Fácil (fluxo básico)
- **Ferramenta:** OpenCode
- **Modelo:** MiMo V2.5 Free (OpenCode Zen)

## Resumo dos testes

| Momento | Passando | Falhando | Total |
|---|---|---|---|
| Início (antes de implementar) | 0 | 24 | 24 |
| Final (após as três funções) | 24 | 0 | 24 |

**Saída final dos testes (24/24 aprovados):**

```
PASSOU | RF-01 · estado inicial completo
PASSOU | RF-07 · estados iniciais independentes
PASSOU | RF-06 · ausência de senha
PASSOU | RF-06 · senha com três dígitos
PASSOU | RF-06 · senha com dois algarismos
PASSOU | RF-06 · não truncar após 999
PASSOU | RF-02 · primeira emissão retorna 1
PASSOU | RF-02 · emissão atualiza a fila
PASSOU | RF-02 · emissão avança a numeração
PASSOU | RF-02 · emitir preserva atendimento e contador
PASSOU | RF-02 · numeração continua após chamada
PASSOU | RF-03 · chamada retorna a primeira senha
PASSOU | RF-03 · remove somente a primeira da espera
PASSOU | RF-03 · atual acompanha a última chamada
PASSOU | RF-03 · conta somente chamadas efetivas
PASSOU | RF-03 · chamar não avança proximaSenha
PASSOU | RF-04 · chamar fila inicialmente vazia retorna null
PASSOU | RF-04 · fila vazia preserva todos os campos
PASSOU | RF-03 · FIFO com emissão entre chamadas
PASSOU | RF-05 · reinício restaura o mesmo objeto
PASSOU | RF-05 · primeira emissão após reinício
PASSOU | RF-05 · reiniciar duas vezes é válido
PASSOU | RF-07 · operar uma fila não modifica outra
PASSOU | RF-02/03 · mil emissões e chamadas sem duplicação
24 aprovados · 0 falhas · 24 testes
```

## Capturas do protótipo e roteiro visual

- `01-inspecao.png` — inspeção inicial do código e especificação
- `02-emissao.png` — protótipo após implementar emitirSenha
- `02-emissao-testes.png` — testes RF-02 após implementação
- `03-chamar-1.png` / `03-chamar-02.png` — protótipo com chamarProxima funcionando
- `03-chamadas-testes.png` — testes RF-03/RF-04
- `04-reiniciar-01.png` / `04-reiniciar-02.png` — protótipo com reiniciarFila
- `04-reiniciar-testes.png` — testes RF-05

**Conclusão do roteiro visual:** emissão, chamada, esvaziamento, cancelamento e confirmação do reinício foram testados no navegador com sucesso.

## Arquivos alterados

- `labs/lab-02-fila-facil/src/fila.js` — implementação dos corpos de `emitirSenha`, `chamarProxima` e `reiniciarFila`

## Decisão de implementação

Optei por implementar as três funções de forma separada de forma incremental em vez de pedir o código completo. Isso permitiu que eu pudesse validar e registrar cada função com a saída dos testes.

## Intervenção humana

Foi necessária intervenção humana no início do processo: o agente tentou implementar as três funções de uma vez e declarar os testes aprovados sem execução real. O usuário solicitou que o trabalho fosse feito **instrução por instrução**, com cada função isolada, aplicada manualmente e verificada com a saída real dos testes. Isso garantiu que cada incremento fosse validado antes de avançar.

## Dúvidas e limitações restantes

Nenhuma. Todos os 24 testes foram aprovados. O fluxo básico está completo.
