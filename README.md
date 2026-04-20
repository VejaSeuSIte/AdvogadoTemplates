# AdvogadoTemplates

Templates de site para advogados **autônomos** brasileiros — não escritórios. Construídos a partir da análise de sites reais de profissionais solo em diferentes nichos (família, trabalhista, previdenciário, criminal, tributário, sucessões).

**Demo ao vivo:** [vejaseusite.github.io/AdvogadoTemplates](https://vejaseusite.github.io/AdvogadoTemplates/)

## Quatro arquétipos, quatro templates

| # | Nome | Perfil | Quando serve |
|---|---|---|---|
| 01 | `banner-retrato` 🆕 | Hero com foto cutout + reviews Google | Trabalhista/INSS com retrato profissional — identidade visual forte, volume médio |
| 02 | `personal-brand` | Marca pessoal editorial | Família, sucessões, consultivo PF — cliente por indicação e Instagram |
| 03 | `high-conversion` | Alta conversão PF | Trabalhista/INSS de volume — Google Ads + WhatsApp |
| 04 | `quiet-authority` | Autoridade discreta | Criminalista ou tributarista premium — só indicação |

Cada template já vem com:

- Identidade do advogado (foto, nome, OAB) como elemento central
- WhatsApp integrado (botão flutuante + CTAs pré-formatados)
- Áreas de atuação em linguagem de cliente, não em juridiquês
- Placeholder completo em português brasileiro
- Rodapé com OAB, CNPJ, Política de Privacidade e disclaimer do Provimento CFOAB 205/2021
- Responsivo até 320px, zero dependências JS

## Como usar

```bash
gh repo clone VejaSeuSIte/AdvogadoTemplates meu-site
cd meu-site/templates/<escolha-um>
# edite o index.html — nome, OAB, WhatsApp, áreas, endereço
```

Deploy direto no GitHub Pages — zero build, zero `node_modules`.

### Substituindo a foto (banner-retrato)

O `banner-retrato` usa uma silhueta SVG estilizada como placeholder no hero e na seção "Quem Sou". Para substituir pela foto real:

1. Exporte sua foto em PNG com fundo transparente (peça pro fotógrafo ou use [remove.bg](https://remove.bg))
2. Coloque em `templates/banner-retrato/assets/retrato.png`
3. No `index.html`, troque o bloco `<svg viewBox="0 0 400 520" …>` dentro de `.portrait` por `<img src="assets/retrato.png" alt="Dra. …" />`

## Metodologia

Foram analisados doze sites reais de advogados autônomos brasileiros:

- Marcia Laino (família · RJ) — base do `personal-brand`
- Karina Roizenblit (trabalhista · RJ) — base do `banner-retrato`
- Camila Morais (trabalhista · SP) — base do `banner-retrato`
- Elisangela B. Taborda (tributário · SP)
- Neil Alden (tributário · DF)
- Ademilson Carvalho (criminal · RJ/SP)
- e outros autônomos em família, previdenciário e consumidor

A partir dos padrões observados, quatro arquétipos ficaram claros — e cada template cobre um deles sem tentar ser tudo.

## Licença

MIT. Use, modifique, venda, embute em serviço. Sem atribuição obrigatória.
