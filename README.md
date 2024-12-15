# @eriveltonsilva/prettier-config

Este repositório contém uma configuração personalizada para o Prettier, projetada para ser reutilizável em vários projetos meus.

## Prettier

O Prettier é uma ferramenta de formatação de código que garante consistência no estilo de código.

## Conteúdo do Repositório

### Arquivos e Pastas

- **`index.json`**: Contém as configurações principais para o Prettier.
- **`README.md`**: Documentação do repositório (este arquivo).

## Configuração do Prettier

As configurações definidas em `index.json` incluem:

```json
{
  "bracketSameLine": true,
  "experimentalTernaries": true,
  "jsxSingleQuote": true,
  "printWidth": 80,
  "semi": false,
  "singleAttributePerLine": true,
  "singleQuote": true
}
```

### Explicação das Configurações

- **`bracketSameLine`**: Mantém os delimitadores de fechamento de JSX na mesma linha dos elementos quando possível, melhorando a legibilidade do código JSX.
- **`experimentalTernaries`**: Habilita um comportamento experimental para ternários, deixando-os mais flexíveis na formatação (pode ser descontinuado em futuras versões).
- **`jsxSingleQuote`**: Usa aspas simples em vez de aspas duplas em atributos JSX.
- **`printWidth`**: Limita a largura das linhas a 80 caracteres, melhorando a legibilidade em telas menores.
- **`semi`**: Remove os pontos e vírgulas ao final das linhas, seguindo uma convenção de estilo minimalista.
- **`singleAttributePerLine`**: Garante que cada atributo em tags HTML/JSX seja colocado em uma linha separada, aumentando a clareza.
- **`singleQuote`**: Usa aspas simples em vez de aspas duplas para strings.

## Usage

**Instale**:

```bash
npm i -D @eriveltonsilva/prettier-config
```

**Edite `package.json`**:

```jsonc
{
  "name": "My project",
  // ...
  "prettier": "@eriveltonsilva/prettier-config",
  "scripts": {
    "format": "prettier --write ."
  }
}
```

**Execute o script para formatar seu código**:

```bash
npm run format
```

## Licença

Este repositório é licenciado sob a [MIT License](LICENSE).

---

Aproveite a configuração e mantenha seu código limpo e consistente!
