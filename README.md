# Teste Avaliativo para Desenvolvedor Mobile na MobApps

## Descrição e funcionalidades do app:

O app deve permitir a consulta de filmes utilizando a API TheMovieDatabase. *Nenhuma das funcionalidades abaixo exigem autenticação do usuário.

Link para documentação da api: [https://www.themoviedb.org/documentation/api](https://www.themoviedb.org/documentation/api)

- Listagem de filmes que estão em cartaz - [https://developers.themoviedb.org/3/movies/get-now-playing](https://developers.themoviedb.org/3/movies/get-now-playing)

    - Use o parâmetro `language` com o valor pt-BR ou en.
    - Campos sugeridos: Title (caso use a língua `pt-BR`), name, release date e vote average.
    - Mostre uma imagem, usando os campos `backdrop_path` ou `poster_path` (Url para Imagens podem ser montadas de acordo com a documentação (https://developers.themoviedb.org/3/configuration))
    - A exibição pode ser em formato de lista ou grade(No caso de grade, exiba apenas o atributo `Title`)

- Detalhes do filme ( https://developers.themoviedb.org/3/movies/get-movie-details )
- Busca de filmes https://developers.themoviedb.org/3/getting-started/search-and-query-for-details
- Salvar filme como favorito
- Listagem de favoritos

## Requisitos técnicos

Uso de algum framework ou biblioteca para organização de arquitetura e/ou redução de código "boilerplate":
- Dagger2 ou Dagger
- Databind
- RxAndroid/RxJava
- ButterKnife

Framework para comunicação com API's externas
- Volley
- Ion
- Wasp
- Retrofit

*Recomendamos Retrofit

Carregamento de imagens usando padrão de "lazyload"
- Picasso
- Fresco
- Glide
- Ion
- Volley

*Recomendamos Glide

Uso de alguma arquitetura com separação de responsabilidades:
- MVP
- MVVM
- CLEAN

### Obs:

- As bibliotecas e arquiteturas citadas são apenas sugestões, sinta-se a vontade para usar outras.

- O design pode ser feito conforme você queira. Caso não tenha algo em mente, siga o padrão do Material Design.

Alguns pontos que serão ser avaliados
- Qualidade é melhor que quantidade.
- Evite fazer requisições desnecessárias. Exemplos de tratamentos:
    - Cache de imagens.
    - Tente manter o estado durante rotações (caso seja permitido).
- Uso de níveis de SDK compatíveis com o mercado.
- Mantenha uma estrutura consistente de navegação, seja por abas ou menu deslizante, conforme o caso.
- Preocupação com compatibilidade e bom uso de biblioteca de suporte: Support Library v4, Appcompat v7, Design Library, AndroidX
- Uso de componentes novos e/ou do Material Design: Toolbar, RecyclerView, AppBar, CoordinatorLayout, SnackBar, FloatActionButton e etc...
- Preocupação com organização de código/padronização.
- Uso de design patterns.

Opcionais:
- Escrever testes unitários.
- Tratar mudança de orientação
