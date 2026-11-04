# Caminho das Pedras do Lab SOC

Guia para quem quer montar o próprio laboratório de **SOC** (Security Operations Center: a central que monitora e investiga alertas de segurança) sem perder meses refazendo configuração.

Nasceu de dois anos de tentativas reais. Aqui estão a ordem certa, o que cada peça faz e os erros que me custaram tempo.

> Série no LinkedIn, toda terça e quinta. Cada post resume uma etapa deste guia.

## Para quem é
Iniciantes em cibersegurança que querem praticar de verdade, com ferramentas usadas no mercado.

## O que você vai montar
Um laboratório com virtualização, rede privada, monitoramento de endpoints, detecção de rede, firewall e gestão de chamados, ligados por automações simples.

## Mapa das etapas
| Etapa | Tema | O que você aprende |
|---|---|---|
| [01](etapas/01-mapa-do-lab.md) | Mapa do lab | Entender o desenho geral antes de instalar qualquer coisa. |
| [02](etapas/02-rede-segura-tailscale.md) | Rede privada com Tailscale | Conectar as máquinas do lab entre si sem expor nada na internet. |
| [03](etapas/03-virtualizacao-proxmox.md) | Virtualização com Proxmox | Rodar vários servidores do lab em um único equipamento. |
| [04](etapas/04-siem-wazuh.md) | SIEM com Wazuh | Receber alertas de segurança de várias máquinas em um só lugar. |
| [05](etapas/05-chamados-glpi.md) | Chamados com GLPI | Transformar alertas em chamados organizados por cliente. |
| [06](etapas/06-ids-firewall.md) | IDS e firewall (Suricata e pfSense) | Detectar tráfego suspeito e controlar o que entra e sai da rede. |
| [07](etapas/07-automacao-rondas.md) | Automação das rondas | Verificar o ambiente em horários fixos, sem depender de lembrar. |
| [08](etapas/08-backup-recuperacao.md) | Backup e recuperação | Garantir que o lab possa ser restaurado se algo der errado. |
| [09](etapas/09-hardening.md) | Hardening sem se trancar | Reduzir a superfície de ataque sem perder o acesso. |

## Lições aprendidas
Erros reais, contados sem enfeite: veja [licoes-aprendidas](licoes-aprendidas/).

## Privacidade
Este repositório não contém IPs, nomes de clientes, tokens ou dados reais. Os exemplos usam nomes fictícios (Cliente A, Cliente B).

## Como contribuir
Achou um erro ou quer sugerir uma etapa? Abra uma issue.

## Autor
Paulo Roberto F. Moraes — [LinkedIn](https://www.linkedin.com/in/paulorobertofm)
