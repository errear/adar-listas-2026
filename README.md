# adar-202002-listas
Repo para templates das listas de exercícios do curso ADAR do 2° semestre de 2020 e correção das listas dos alunos.

Os quatro templates estão em `templates/`, no formato Quarto (`.qmd`), com
código R executado pelo knitr. Os enunciados e o código dos exercícios foram
preservados na conversão de R Markdown.

Para renderizar, instale o [Quarto](https://quarto.org/docs/get-started/) e
tenha o R e os pacotes utilizados pelo template disponíveis. Execute na raiz
do repositório, por exemplo:

```sh
quarto render templates/lista-1-adar-2020-template.qmd --to html
```

Todos os templates geram HTML com os recursos incorporados. A lista 1 também
permite gerar PDF (requer uma distribuição TeX):

```sh
quarto render templates/lista-1-adar-2020-template.qmd --to pdf
```

Para editar com pré-visualização:

```sh
quarto preview templates/lista-2-adar-2026-template.qmd
```

A renderização executa os chunks habilitados. A lista 3 contém código que lê
`S_America_model_wtd_v2.nc`; disponibilize esse arquivo em `templates/` antes
de renderizá-la. Os chunks originalmente marcados com `eval = FALSE`
continuam sem execução.
