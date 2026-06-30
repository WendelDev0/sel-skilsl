# Selva Skills

Repositorio compartilhado de skills da equipe Selva para uso no Codex e no Claude.

## Skills disponiveis

- `copy-selva`: ajuda a criar, revisar e padronizar copies, anuncios, criativos, landing pages, emails e mensagens comerciais no tom da Selva.
- `trafego-selva`: ajuda a planejar, revisar e otimizar campanhas de trafego pago, funis, segmentacoes, ofertas e diagnosticos de performance.

## Estrutura

```text
skills/
  copy-selva/
    SKILL.md
  trafego-selva/
    SKILL.md
AGENTS.md
CLAUDE.md
```

## Como usar no Codex

1. Baixe ou clone este repositorio.
2. Copie as pastas de `skills/` para a pasta de skills do Codex:

```powershell
Copy-Item -Recurse ".\skills\copy-selva" "$env:USERPROFILE\.codex\skills\copy-selva"
Copy-Item -Recurse ".\skills\trafego-selva" "$env:USERPROFILE\.codex\skills\trafego-selva"
```

3. Em uma conversa, chame a skill pelo nome:

```text
Use a skill copy-selva para revisar esta campanha.
Use a skill trafego-selva para montar um plano de campanha.
```

## Como usar no Claude

1. Baixe ou clone este repositorio.
2. Copie as pastas de `skills/` para a pasta de skills do Claude:

```powershell
Copy-Item -Recurse ".\skills\copy-selva" "$env:USERPROFILE\.claude\skills\copy-selva"
Copy-Item -Recurse ".\skills\trafego-selva" "$env:USERPROFILE\.claude\skills\trafego-selva"
```

3. Em uma conversa, chame a skill pelo nome:

```text
Use a skill copy-selva para criar 10 headlines.
Use a skill trafego-selva para diagnosticar esta conta.
```

## Comandos recomendados para a equipe

Instalar ou atualizar as skills no Codex:

```powershell
git clone https://github.com/WendelDev0/sel-skilsl.git
cd sel-skilsl
Copy-Item -Recurse -Force ".\skills\copy-selva" "$env:USERPROFILE\.codex\skills\copy-selva"
Copy-Item -Recurse -Force ".\skills\trafego-selva" "$env:USERPROFILE\.codex\skills\trafego-selva"
```

Instalar ou atualizar as skills no Claude:

```powershell
git clone https://github.com/WendelDev0/sel-skilsl.git
cd sel-skilsl
Copy-Item -Recurse -Force ".\skills\copy-selva" "$env:USERPROFILE\.claude\skills\copy-selva"
Copy-Item -Recurse -Force ".\skills\trafego-selva" "$env:USERPROFILE\.claude\skills\trafego-selva"
```

## Padrao para contribuir

1. Edite apenas a pasta da skill que deseja melhorar.
2. Mantenha os comandos claros e acionaveis.
3. Inclua exemplos de entrada e saida quando adicionar um novo fluxo.
4. Abra um pull request explicando o que mudou e quando usar a nova versao.
