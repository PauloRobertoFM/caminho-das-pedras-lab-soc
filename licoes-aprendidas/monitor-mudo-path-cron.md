# O monitor mudo

## O que aconteceu
Uma rotina de vigilância da infraestrutura parecia rodar, mas não detectava nada.

## Causa raiz
O agendador (cron) usa um ambiente diferente do terminal e não encontrava os comandos necessários. Cada execução falhava sem avisar.

## Lição
Quem vigia também precisa ser vigiado. Falha silenciosa é pior que falha barulhenta.

## O que fazer diferente
- Teste o script no mesmo ambiente do agendador, com PATH explícito.
- Monitore o próprio monitor, com alerta se a rotina ficar muda.

> Status: rascunho. Será expandido com a versão didática e ilustrada.
