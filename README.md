# Firewall Humano — Campanha de Segurança da Informação

> "Nenhuma tecnologia bloqueia o que você deixa passar."

Campanha educativa para os colaboradores da **SisFEAP** (ERP para universidades e Fundações de Amparo à Pesquisa), desenvolvida como trabalho acadêmico (AD1) da disciplina **Segurança Aplicada ao Desenvolvimento**, UDESC/CEAD.

## Como executar

1. Abra a pasta `campanha-seguranca-informacao`.
2. Dê dois cliques em `index.html` (Chrome, Edge ou Firefox).

Não é preciso servidor, instalação nem build. Com internet, a página usa as fontes Bebas Neue e Fira Code do Google Fonts; sem internet, ela usa fontes equivalentes do sistema.

## Estrutura

```
campanha-seguranca-informacao/
├── index.html          estrutura e conteúdo da campanha (HTML semântico)
├── css/style.css       apresentação: variáveis, layout, componentes
├── js/main.js          comportamento: exibe o nome em texto se o logo faltar
├── assets/images/      imagens da campanha e logo da SisFEAP
├── extras/simulador/   simulador e checklist guardados para uso futuro (fora da página)
└── README.md
```

O script é clássico (`defer`), e não ES module, porque módulos são bloqueados pelo navegador quando a página é aberta direto do disco (`file://`).

### Reativar o simulador e o checklist

Os arquivos em `extras/simulador/` não são carregados pela página. Cada um traz no topo as instruções para voltar a usá-lo: o HTML das seções, o CSS, as funções JavaScript e os dados das 10 situações.

## Seções e conteúdos da disciplina

| Seção | Conteúdos |
|---|---|
| Abertura | Conceito da campanha, domínio do usuário |
| Ativos | Ativos de informação, dado/informação/conhecimento, classificação, controle |
| Pilares | Confidencialidade, integridade, disponibilidade |
| Ameaças | Ameaça × vulnerabilidade × risco, ameaças internas/externas, engenharia social, malware, técnicas de ataque, uso indevido de recursos |
| Hábitos | Segurança física e lógica, controle de acesso |
| Dev | SQL Injection, NoSQL Injection, XSS, CSRF, testes de segurança |
| Política | Normas e leis, monitoramento, testes, auditoria, planos de segurança |
| Incidente | Protocolo: Pare → Preserve → Reporte → Não resolva sozinho |

## Limitações

- Contatos (`seguranca@sisfeap.example`, ramal 4040) e regras são ilustrativos; o domínio `.example` é reservado para exemplos.
- Os exemplos de código vulnerável são apenas exibidos como texto, nunca executados.
- Layout pensado para telas de computador (não otimizado para celular).
