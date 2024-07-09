https://forms.gle/wYkAQ28MjcUiPTqE7

- Você terá até as 22h30 para realizar e entregar a prova (código no github + link do github pages).
- A prova é individual.
- É vedado, durante a prova, o porte e/ou o uso de aparelhos sonoros, fonográficos, de comunicação ou de registro eletrônico ou não, tais como: notebooks, celulares, tablets e similares.
- Nenhum aluno está autorizado a sair de sala em período inferior a 60 minutos do horário do início da prova.
- É estritamente proibido acessar websites que não sejam o github, documentação MDN, w3schools, links disponíveis nos slides.
- O aluno deverá criar/utilizar um repositório no Github somente para a prova, e identificar o RA na descrição do repositório.
- O repositório precisa ser configurado para subir uma página no Github Pages, pois através do site publicado que a correção da prova será corrigida e avaliada.
- Certifique-se de que o código está devidamente publicado no repositório Github e que o link do site gerado pelo Github Pages está funcionando corretamente
- Ao término da prova, levante o braço e aguarde o atendimento do professor ou do fiscal.

No final do formulário foi disponibilizado um vídeo, mostrando o resultado esperado.

### QUESTÕES:

#### Estrutura da Página (2 pontos)

- Utilize a seguinte estrutura de projeto: a Home ficará na raiz, em index.html e as outras páginas ficarão em pastas separadas (0.5 ponto): 
   - Página principal: ./index.html; 
   - Página de municípios: ./municipios/index.html; 
   - Página de favoritos: ./favoritos/index.html.

- Utilize uma grid para organizar o conteúdo da página, onde o conteúdo principal (main) ocupa a maior parte do espaço. (1 ponto)

- O header tem cor de fundo #047ae0 e o footer tem cor de fundo #444. (0.25 pontos)

- Adicione o texto "© 2024 Prova SUB de Programação Web" no footer. (0.25 pontos)

#### Página de Estados (./index.html) (2.5 pontos).

- Utilize a API  do IBGE para buscar dados dos estados brasileiros. (1 ponto)

- Liste o nome de cada estado dentro de uma lista (ul/li). (0.25 pontos)

- Remova os bullet points da lista, utilizando css na ul ou na li. (0.25 pontos)

- Cada estado deve estar em um link (âncora <a>) que direciona para a página de municípios (./municipios/index.html), passando a UF (Unidade Federativa) do estado via querystring ex: ?uf=PR. (0.5 pontos)

- Os links (âncoras) dos estados devem ter cor #444 com uma transição no hover para alterar a opacidade para 0.8. (0.5 pontos)

#### Página de Municípios (./municipios/index.html) (4 pontos)

- Utilize a API do IBGE para buscar os municípios de um estado específico, baseado na UF passado via querystring. (1 ponto)

- Exiba o título h2 da página como "Municípios de {UF}", onde {UF} é substituído pelo UF (Unidade Federativa) recebido na querystring. (0.5 pontos)

- Liste os municípios dentro de uma lista não ordenada (ul/li). (0.25 pontos)

- Remova os bullet points da lista, utilizando css na ul ou na li. (0.25 pontos)

- Cada município deve ser exibido como um item de lista (li) com o nome do município e um botão para favoritar. (0.25 pontos)

- O botão de favoritar deve ter cor de fundo #edd83b e uma transição no hover para alterar a opacidade para 0.8. (0.25 pontos)

- Ao clicar no botão de favoritar, o objeto do município deve ser adicionado a uma lista de favoritos no localStorage. Utilize favoritos como nome da chave localStorage. (1.5 pontos)

#### Página de Favoritos (./favoritos/index.html) (1 ponto)

- Buscar a lista de favoritos salva em localStorage e exibir o nome do municipio em uma ul/li cada município favoritado. (1 ponto).

#### Funcionalidades Extras (0.5 pontos)

- Adicione um link (âncora) com o texto "Ver favoritos", no header da página principal e na página de municípios, o link deve direcionar para a página de favoritos (./favoritos/index.html). (0.25 ponto)

- Adicione um link (âncora) com o texto "Ir para a home", no header das páginas de municípios e de favoritos, que direciona para a página principal (./index.html). (0.25 ponto)


URL para api de estados: https://servicodados.ibge.gov.br/api/v1/localidades/estados
URL para api de municípios: https://servicodados.ibge.gov.br/api/v1/localidades/estados/{uf}/municipios
Vídeo de exemplo: https://youtu.be/j0vsLKOHsRs
