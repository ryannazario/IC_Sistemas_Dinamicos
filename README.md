# Modelo inicial de Iniciação Científica em Quarto

Este projeto é um ponto de partida **editável** para uma IC sobre sistemas dinâmicos discretos.

## Preparação no Windows

1. Instale o Quarto: https://quarto.org/docs/get-started/
2. Instale o VS Code: https://code.visualstudio.com/
3. No VS Code, instale a extensão `Quarto`.
4. Tenha Python 3 instalado.
5. Abra esta pasta no VS Code, acesse **Terminal > Novo Terminal** e execute:

```powershell
quarto --version
quarto install tinytex
py -m pip install jupyter numpy matplotlib
```

## Produzir o texto

Edite `iniciacao-cientifica.qmd`. O cabeçalho entre `---` define título, autor e formatos de saída.

- `#` cria uma seção; `##` uma subseção.
- `$...$` inclui fórmula na mesma linha.
- `$$...$$` inclui fórmula destacada.
- `[@may1976]` ou `@may1976` cita uma referência de `referencias.bib`.
- `@eq-mapa-logistico` referencia uma equação, e `@fig-orbita` referencia o gráfico.
- Blocos com `` ```{python} `` são executados para criar gráficos e resultados.

## Gerar arquivos

No terminal, dentro da pasta do projeto:

```powershell
quarto render iniciacao-cientifica.qmd --to html
quarto render iniciacao-cientifica.qmd --to pdf
```

Serão criados `iniciacao-cientifica.html` e `iniciacao-cientifica.pdf`.

## Observações

- O layout fornecido é acadêmico genérico, **não** é certificado como ABNT/USP.
- Para padrões específicos, ajuste a formatação e o estilo bibliográfico conforme as instruções da orientadora e do programa.
- Substitua os trechos ilustrativos por resultados próprios e mantenha fontes corretamente citadas.
