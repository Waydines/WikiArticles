# Contribuindo para Artigos na Waypédia

Português · [English](./CONTRIBUTING.md)

Obrigado por querer contribuir para a Waypédia! Para garantir que todos os artigos sigam um padrão consistente, siga as diretrizes abaixo.

## Criando um Artigo

Os artigos devem ser arquivos `.mdx` e devem ser adicionados à pasta `src`. O nome do arquivo deve seguir estas regras:

- Use apenas letras minúsculas
- Não use acentos ou caracteres especiais
- Evite usar mais de um espaço consecutivamente, a não ser que realmente seja necessário
- Não deixe espaços no início ou fim do nome

## Organização por Idioma

Coloque o artigo na subpasta correspondente dentro de `src`:

- Para artigos em português: `src/pt/`
- Para artigos em inglês: `src/en/`

## Estrutura do Arquivo

Cada artigo deve começar com uma _frontmatter_ no seguinte formato:

```yml
---
id: "identificador único do artigo (deve ser o mesmo entre traduções)" # OBRIGATÓRIO
title: "Título do artigo" # OBRIGATÓRIO
banner: "URL de uma imagem banner" # opcional
short_description: "descrição extremamente curta (algo como 5 palavras) para o artigo" # optional
---
```

🔹 O campo `id` deve ser o mesmo para todas as versões traduzidas do artigo.

## Atualizando o `mappings.json`

Após criar o artigo ou adicionar uma tradução a ele, adicione a seguinte entrada no arquivo `mappings.json`:

```json
"id-do-seu-artigo": {
    "en": "nome-do-arquivo-em-ingles",
    "pt": "nome-do-arquivo-em-portugues"
}
```

**⚠ Não inclua .mdx no final do nome do artigo na definição acima.**

Se o seu artigo ainda não tiver certa tradução, você deverá retirar a linha que definiria o nome do arquivo daquela respectiva língua.

## Revisão e Pull Requests

> [!CAUTION]
> Antes de enviar sua contribuição, confira se todas as regras foram seguidas.
> Caso contrário, sua pull request pode ser recusada.

Pull Requests deverão ser inicialmente feitas à ramificação `staging`.
Se tiver dúvidas, sinta-se à vontade para perguntar. Obrigado por contribuir com a Waypédia!
