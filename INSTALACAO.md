# Instalação do pacote

## 1. Repositório

O repositório de perfil deve se chamar exatamente:

`antoniomotajr/antoniomotajr`

## 2. Copie os arquivos

Mantenha esta estrutura:

```text
antoniomotajr/
├── README.md
├── INSTALACAO.md
├── assets/
│   └── github_fullstack_ia_animado_lento.gif
├── profile/
│   ├── stats.svg
│   └── top-langs.svg
└── .github/
    └── workflows/
        └── github-stats.yml
```

## 3. Faça o primeiro push

Depois de enviar os arquivos para o GitHub, abra:

`Actions` → `Atualizar estatísticas do GitHub`

Clique em:

`Run workflow`

A execução vai gerar os SVGs reais em `profile/` e fazer o commit automaticamente.

## 4. Atualização automática

O workflow também está configurado para executar diariamente às 03:00 UTC.

## 5. Permissões

O workflow já declara:

```yaml
permissions:
  contents: write
```

Isso permite que o GitHub Actions atualize os arquivos SVG dentro do próprio repositório.

## Observação

Os SVGs incluídos no pacote são apenas placeholders iniciais. Eles não representam estatísticas reais. A primeira execução bem-sucedida do workflow os substituirá pelos cards reais.
