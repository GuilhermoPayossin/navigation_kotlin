# Passagem de parâmetros obrigatórios na tela de Perfil
Nesse commit, a tela de Perfil deixou de ser estática e passou a receber um parâmetro obrigatório chamado nome pela rota perfil/{nome}. Isso exigiu alterações na MainActivity, que passou a extrair o argumento da navegação, no MenuScreen, que agora envia um nome ao navegar, e na PerfilScreen, que exibe o valor recebido no texto da tela. Esse passo foi importante porque introduziu a ideia de uma tela dinâmica, com conteúdo dependente de dados vindos de outra rota.

# Passagem de parâmetros opcionais na tela de Pedidos
Nesse commit, a tela de Pedidos passou a aceitar um parâmetro opcional chamado cliente, usando a rota pedidos?cliente={cliente}. Além disso, foi definido um valor padrão para o caso de o argumento não ser enviado. A PedidosScreen também foi ajustada para receber esse valor e mostrá-lo na interface. Isso tornou a navegação mais flexível, permitindo que a tela funcione mesmo sem todos os dados preenchidos.

# Inserindo valor ao parâmetro opcional na tela de Pedidos
Esse commit complementa o anterior, consolidando o uso do parâmetro opcional no fluxo da aplicação. Agora, o valor de cliente é efetivamente enviado e consumido pela tela de Pedidos, reforçando o comportamento dinâmico da navegação.

# Passagem de múltiplos parâmetros
Aqui a navegação evoluiu para um cenário mais avançado. A rota da tela de Perfil passou a receber nome e idade, e a MainActivity foi atualizada para declarar os tipos de cada argumento com NavType.StringType e NavType.IntType. O MenuScreen passou a navegar enviando os dois valores, e a PerfilScreen foi adaptada para recebê-los e exibi-los juntos na interface. Essa mudança ampliou a complexidade da navegação e mostrou como o app pode lidar com mais de um dado ao mesmo tempo de forma organizada.