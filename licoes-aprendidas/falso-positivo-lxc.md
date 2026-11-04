# O falso positivo do container

## O que aconteceu
O SIEM acusava arquivos suspeitos em várias máquinas.

## Causa raiz
Eram artefatos normais de containers LXC, que a regra de verificação interpretava como suspeitos.

## Lição
Nem todo alerta é incidente. Conhecer o ambiente evita escalar ruído.

## O que fazer diferente
- Documente falsos positivos conhecidos para classificar mais rápido.
- Registre a decisão no chamado, para ter histórico e métrica.

> Status: rascunho. Será expandido com a versão didática e ilustrada.
