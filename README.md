Crash
O Crash é um jogo multiplayer que usa uma cadeia sha256 em combinação com uma seed de cliente indeterminada para gerar rodadas de maneira justa.

Geração de Cadeia
Para gerar a cadeia, começamos com bytes seguramente aleatorios. A partir daí, iteramos 10 milhões de vezes, alimentando a seed anterior em uma função sha256. Os jogos de Double leem a cadeia em uma ordem inversa.

A seed final/terminal desta cadeia é 492bd10144a3525e2745718fe4d25e08affbea483872d8e8b86191b20ce0a7a8

Gerando um hash
Para obter uma aleatoriedade justa, criamos um hash sha256 hmac usando a seed do servidor como chave e a seed do cliente como valor.

A cadeia do Crash de 10 milhões de hashes sha256 foi gerada em 2019-04-04 05:59AM UTC. Decidimos usar 0000000000000000000415ebb64b0d51ccee0bb55826e43846e5bea777d91966, o hash do bloco Bitcoin 570132, extraído em 2019-04-04 06:35AM UTC como a seed do cliente para esta cadeia.
