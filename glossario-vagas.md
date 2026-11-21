# Dicionário de termos, siglas, técnicas, ferramentas e certificações — vagas de SOC / Blue Team

> **Origem e limite deste documento.** O dicionário feito antes não foi encontrado (repositório, Drive, Notion e artefatos). Este foi refeito a partir das vagas citadas na sessão do LinkedIn (16–18/11/2026): Logical IT (SOC Jr), Grupo NTSec (Técnico de SOC), Track&Field (Blue Team Jr), Paranapanema (Segurança da Informação Jr), Oakmont (SOC Pleno), TOTVS e Vision Cybersecurity (SOC, Indeed).
> **Não tive o texto dos anúncios**, só os títulos. Os itens abaixo são os que costumam ser pedidos para esses cargos. Para cada vaga, confira a lista real de requisitos e marque o que realmente aparece.

Como ler a coluna **Nível**: 🟢 básico, esperado de júnior · 🟡 diferencial · 🔴 pleno ou acima.

---

## 1. Siglas e termos do dia a dia

| Termo | O que significa | Nível |
|---|---|---|
| **SOC** | *Security Operations Center*: equipe que monitora e responde a eventos de segurança, em geral 24x7. | 🟢 |
| **Blue Team** | Time de defesa: monitora, detecta, responde e endurece ambientes. Oposto do Red Team (ataque simulado). | 🟢 |
| **SIEM** | *Security Information and Event Management*: coleta logs de várias fontes, correlaciona e gera alertas. | 🟢 |
| **EDR / XDR** | *Endpoint / Extended Detection and Response*: agente nos equipamentos que detecta e permite isolar a máquina. XDR amplia para rede, nuvem e e-mail. | 🟢 |
| **IDS / IPS** | Sistema de detecção / prevenção de intrusão. O IPS também bloqueia. | 🟢 |
| **NDR** | *Network Detection and Response*: detecção baseada em tráfego de rede. | 🟡 |
| **SOAR** | *Security Orchestration, Automation and Response*: automatiza respostas e fluxos de tratamento de alertas. | 🟡 |
| **Log** | Registro de eventos de um sistema, aplicação ou equipamento. | 🟢 |
| **Alerta / Evento / Incidente** | Evento é qualquer ocorrência; alerta é um evento que disparou uma regra; incidente é o que foi confirmado como impacto ou risco real. | 🟢 |
| **Falso positivo / Verdadeiro positivo** | Alerta que não era ameaça / alerta que era ameaça de fato. | 🟢 |
| **Triagem** | Primeira análise do alerta: decidir se descarta, escala ou abre incidente. | 🟢 |
| **Nível 1 / 2 / 3 (N1, N2, N3)** | Camadas de analistas: N1 triagem, N2 investigação, N3 caça a ameaças e engenharia de detecção. | 🟢 |
| **Playbook / Runbook** | Roteiro passo a passo para tratar um tipo de alerta ou incidente. | 🟢 |
| **SLA** | *Service Level Agreement*: prazo acordado de atendimento ou resposta. | 🟢 |
| **IoC** | *Indicator of Compromise*: sinal de comprometimento (hash, IP, domínio, URL). | 🟢 |
| **IoA** | *Indicator of Attack*: sinal de comportamento de ataque em andamento. | 🟡 |
| **TTP** | Táticas, técnicas e procedimentos do atacante. | 🟡 |
| **CTI** | *Cyber Threat Intelligence*: inteligência sobre ameaças e atacantes. | 🟡 |
| **Threat Hunting** | Busca proativa por ameaças que as regras não pegaram. | 🔴 |
| **IR / DFIR** | *Incident Response* / *Digital Forensics and Incident Response*. | 🟡 |
| **CVE** | Identificador público de vulnerabilidade, por exemplo CVE-2026-0257. | 🟢 |
| **CVSS** | Nota de 0 a 10 que mede a gravidade técnica de uma vulnerabilidade. | 🟢 |
| **CIA (CID)** | Confidencialidade, Integridade e Disponibilidade, os três pilares da segurança. | 🟢 |
| **IAM / PAM** | Gestão de identidades e acessos / gestão de acessos privilegiados. | 🟡 |
| **MFA / 2FA** | Autenticação com mais de um fator. | 🟢 |
| **DLP** | *Data Loss Prevention*: evita vazamento de dados. | 🟡 |
| **WAF** | *Web Application Firewall*: protege aplicações web. | 🟡 |
| **VPN** | Túnel criptografado de acesso remoto. | 🟢 |
| **DMZ** | Rede intermediária entre internet e rede interna. | 🟢 |
| **IAM de nuvem, CSPM** | Gestão de acesso em nuvem / monitoramento de má configuração na nuvem. | 🔴 |
| **GRC** | Governança, Riscos e Conformidade. | 🟡 |
| **LGPD** | Lei Geral de Proteção de Dados (Brasil). | 🟢 |
| **PCI DSS** | Padrão de segurança de dados de cartões de pagamento. | 🟡 |
| **BCP / DRP** | Plano de continuidade de negócios / plano de recuperação de desastres. | 🟡 |
| **Hardening** | Endurecimento: remover o desnecessário e configurar de forma segura. | 🟢 |
| **Patch / Gestão de patches** | Correção publicada pelo fabricante / processo de aplicá-la. | 🟢 |
| **Gestão de vulnerabilidades** | Ciclo de descobrir, priorizar, corrigir e verificar falhas. | 🟢 |

## 2. Frameworks e padrões

| Termo | O que é | Nível |
|---|---|---|
| **MITRE ATT&CK** | Catálogo público de táticas e técnicas de atacantes (ex.: T1059 Execução por linha de comando). Usado para classificar alertas e medir cobertura de detecção. | 🟢 |
| **Cyber Kill Chain** | Modelo de fases de um ataque (reconhecimento até ação final). | 🟡 |
| **NIST CSF** | Framework de cibersegurança: Identificar, Proteger, Detectar, Responder, Recuperar. | 🟡 |
| **NIST SP 800-61** | Guia de resposta a incidentes: preparação, detecção, contenção, erradicação, recuperação, lições. | 🟡 |
| **ISO/IEC 27001 / 27002** | Norma de sistema de gestão de segurança da informação / controles. | 🟢 |
| **CIS Controls / CIS Benchmarks** | Lista priorizada de controles / guias de configuração segura. | 🟡 |
| **OWASP Top 10** | Principais riscos de aplicações web. | 🟡 |
| **Cyber Defense Matrix, Diamond Model** | Modelos de análise de intrusão (raramente exigidos em júnior). | 🔴 |

## 3. Ferramentas

| Ferramenta | Para que serve | Nível |
|---|---|---|
| **Splunk** | SIEM comercial, muito pedido. Linguagem de busca SPL. | 🟢 |
| **Microsoft Sentinel** | SIEM/SOAR na nuvem Azure. Consultas em KQL. | 🟡 |
| **IBM QRadar** | SIEM comercial. | 🟡 |
| **Elastic Stack (ELK) / Elastic Security** | Busca e SIEM com Elasticsearch, Logstash e Kibana. | 🟡 |
| **Wazuh** | SIEM/XDR de código aberto. Bom para laboratório. | 🟡 |
| **Graylog** | Gestão de logs de código aberto. | 🟡 |
| **Microsoft Defender for Endpoint** | EDR da Microsoft. | 🟢 |
| **CrowdStrike Falcon** | EDR/XDR de mercado. | 🟡 |
| **SentinelOne, Cortex XDR, Trend Micro, Kaspersky** | Outros EDR/antivírus corporativos. | 🟡 |
| **Suricata / Snort** | IDS/IPS de rede de código aberto. | 🟡 |
| **Zeek** | Análise de tráfego de rede em forma de logs. | 🔴 |
| **Wireshark / tcpdump** | Captura e análise de pacotes. | 🟢 |
| **Nmap** | Mapeamento de portas e serviços. | 🟢 |
| **Nessus / OpenVAS / Qualys / Rapid7** | Scanners de vulnerabilidade. | 🟢 |
| **Burp Suite, OWASP ZAP** | Teste de segurança de aplicações web. | 🟡 |
| **Palo Alto, Fortinet (FortiGate), Check Point, Cisco ASA** | Firewalls de mercado. | 🟡 |
| **Proofpoint, Mimecast, Defender for Office 365** | Proteção de e-mail. | 🟡 |
| **VirusTotal, AbuseIPDB, Any.run, Hybrid Analysis, URLScan** | Consulta de reputação e análise de arquivos, URLs e IPs. | 🟢 |
| **MISP, OpenCTI** | Plataformas de inteligência de ameaças. | 🔴 |
| **TheHive, Cortex, Shuffle, Splunk SOAR, Cortex XSOAR** | Gestão de casos e automação de resposta. | 🔴 |
| **Sysmon** | Telemetria detalhada de Windows (processos, rede, registro). | 🟡 |
| **Velociraptor, Volatility, Autopsy** | Coleta e forense (memória e disco). | 🔴 |
| **Active Directory (AD) / Entra ID** | Diretório de usuários e computadores da Microsoft. Muito alvo de ataque. | 🟢 |
| **ServiceNow, Jira, GLPI** | Gestão de chamados. | 🟢 |
| **Linux, Windows Server, PowerShell, Bash, Python** | Base técnica para investigar e automatizar. | 🟢 |

## 4. Técnicas de ataque que o analista precisa reconhecer

| Termo | Resumo | Nível |
|---|---|---|
| **Phishing / Spear phishing** | E-mail ou mensagem falsa para roubar credenciais ou instalar malware. | 🟢 |
| **Malware** | Software malicioso: vírus, trojan, worm, spyware. | 🟢 |
| **Ransomware** | Malware que cifra dados e exige resgate. | 🟢 |
| **Força bruta / Password spraying / Credential stuffing** | Tentativas repetidas de login, com muitas senhas, uma senha em muitas contas, ou credenciais vazadas. | 🟢 |
| **Movimento lateral** | Atacante se espalha de uma máquina para outras dentro da rede. | 🟡 |
| **Escalação de privilégios** | Obter mais permissões do que se tinha. | 🟡 |
| **Persistência** | Manter acesso após reinício, por tarefas agendadas, serviços, chaves de registro. | 🟡 |
| **C2 / C&C** | Servidor de comando e controle usado pelo atacante. | 🟡 |
| **Exfiltração** | Retirada de dados da organização. | 🟡 |
| **Living off the Land (LOLBins)** | Uso de ferramentas legítimas do sistema (PowerShell, certutil) para atacar. | 🔴 |
| **Pass-the-Hash / Kerberoasting / Mimikatz** | Ataques a credenciais em ambiente Windows e AD. | 🔴 |
| **SQL Injection / XSS / CSRF / RCE / LFI** | Falhas clássicas de aplicações web. | 🟡 |
| **DDoS** | Ataque de negação de serviço distribuído. | 🟢 |
| **Engenharia social** | Manipulação de pessoas, não de sistemas. | 🟢 |
| **Zero-day** | Vulnerabilidade explorada antes de haver correção. | 🟢 |
| **Supply chain (cadeia de suprimentos)** | Ataque via fornecedor ou atualização de software. | 🟡 |
| **Beaconing** | Comunicação periódica de uma máquina infectada com o C2. | 🟡 |

## 5. Técnicas de defesa e análise

| Termo | Resumo | Nível |
|---|---|---|
| **Correlação de logs** | Ligar eventos de fontes diferentes para enxergar um ataque. | 🟢 |
| **Regras de detecção (Sigma, YARA, Suricata)** | Sigma descreve detecções de logs; YARA identifica malware por padrões; regras Suricata detectam tráfego. | 🟡 |
| **Contenção, erradicação, recuperação** | Fases da resposta: isolar, remover a causa, restaurar. | 🟢 |
| **Isolamento de host** | Cortar a máquina da rede pelo EDR. | 🟢 |
| **Análise de e-mail (cabeçalho, SPF, DKIM, DMARC)** | Verificar origem e autenticidade de e-mails suspeitos. | 🟢 |
| **Sandbox** | Ambiente isolado para executar e observar arquivos suspeitos. | 🟡 |
| **Segmentação de rede / Zero Trust** | Dividir a rede em zonas / não confiar por padrão em nenhum acesso. | 🟡 |
| **Cadeia de custódia** | Registro de quem manuseou uma evidência digital, para ter validade. | 🔴 |
| **Lições aprendidas / Post-mortem** | Revisão após o incidente para melhorar processos. | 🟢 |
| **Purple Team** | Cooperação entre ataque e defesa para melhorar detecções. | 🔴 |

## 6. Certificações citadas com frequência

| Certificação | Emissor | Foco | Nível |
|---|---|---|---|
| **CompTIA Security+** | CompTIA | Base de segurança. A mais pedida para júnior. | 🟢 |
| **CompTIA CySA+** | CompTIA | Analista de operações de segurança (Blue Team). | 🟡 |
| **CompTIA Network+ / A+** | CompTIA | Redes e suporte, base técnica. | 🟢 |
| **Microsoft SC-900** | Microsoft | Fundamentos de segurança, conformidade e identidade. | 🟢 |
| **Microsoft SC-200** | Microsoft | Analista de operações de segurança (Sentinel, Defender). | 🟡 |
| **Microsoft AZ-900** | Microsoft | Fundamentos de Azure. | 🟢 |
| **ISC2 CC (Certified in Cybersecurity)** | ISC2 | Entrada em segurança. | 🟢 |
| **ISC2 CISSP** | ISC2 | Gestão de segurança. Exige experiência. | 🔴 |
| **CEH** | EC-Council | Hacking ético, teoria. | 🟡 |
| **eJPT** | INE | Pentest básico, prático. | 🟡 |
| **BTL1 (Blue Team Level 1)** | Security Blue Team | Blue Team prático. | 🟡 |
| **GIAC GSEC / GCIH / GCIA** | SANS/GIAC | Segurança, resposta e análise de intrusão. Caras. | 🔴 |
| **Splunk Core Certified User / Power User** | Splunk | Uso do Splunk. | 🟡 |
| **ISO 27001 Foundation / Lead Implementer / Lead Auditor** | PECB, EXIN e outros | Gestão de segurança e auditoria. | 🟡 |
| **EXIN ISFS** | EXIN | Fundamentos de segurança da informação. | 🟢 |
| **ITIL 4 Foundation** | Axelos | Gestão de serviços de TI. | 🟡 |
| **Cisco CCNA / CyberOps Associate** | Cisco | Redes / operações de segurança. | 🟡 |
| **Fortinet NSE 1–4** | Fortinet | Fundamentos Fortinet, gratuitos. | 🟢 |
| **LPIC-1 / RHCSA** | LPI / Red Hat | Linux. | 🟡 |
| **OSCP** | OffSec | Pentest avançado. Raramente exigido em SOC. | 🔴 |

## 7. Termos de vaga (RH e contrato)

| Termo | Significado |
|---|---|
| **Júnior / Pleno / Sênior** | Níveis de experiência. Júnior costuma pedir até 2 anos. |
| **Escala 24x7, 12x36, plantão, sobreaviso** | Regimes de trabalho típicos de SOC: turnos ininterruptos, 12 horas de trabalho e 36 de folga, atendimento fora do horário. |
| **Híbrido / Home office / Presencial** | Modelo de trabalho. |
| **CLT / PJ** | Contrato com carteira assinada / como pessoa jurídica. |
| **Inglês técnico** | Leitura de documentação e relatórios em inglês. |
| **Cursando / formado em TI, Segurança, Redes** | Formação aceita. Em júnior, muitas vagas aceitam quem está cursando. |

---

## Como usar nas candidaturas

1. Para cada vaga, copie a lista real de requisitos e risque o que aparece aqui.
2. Priorize os itens 🟢 e relacione com o que você já fez no laboratório (Wazuh, Suricata, rondas de triagem, MITRE ATT&CK).
3. Os 🟡 e 🔴 que a vaga citar viram a lista de estudo da semana.
4. Cite no currículo termos e ferramentas pelos nomes que a vaga usa, porque filtros automáticos procuram essas palavras.
