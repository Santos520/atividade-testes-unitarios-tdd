# Registro do ciclo de TDD

## Comportamento escolhido

Calcular a taxa de entrega de um pedido conforme a distância percorrida e o valor total do pedido.

## Red

**Teste criado:** test_taxa_entrega_2km — verifica se um pedido de R$ 50,00 com distância de 2 km possui taxa de entrega de R$ 5,00.

**Motivo da falha:** O teste falha inicialmente quando a função calcular_taxa_entrega ainda não está implementada ou não retorna o valor esperado.

## Green

**Implementacao realizada:** Implementação da função calcular_taxa_entrega(distancia_km, total_pedido) com a regra de taxa inicial de R$ 5,00 para distâncias de até 3 km. Em seguida, foram contempladas as regras de acréscimo de R$ 2,00 por quilômetro excedente e entrega gratuita para pedidos a partir de R$ 100,00.

## Refactor

**Melhoria realizada:** Organização da implementação e dos testes para facilitar a leitura e a manutenção do código. Caso nenhuma refatoração tenha sido necessária, a implementação foi mantida como estava.
**Resultado final:** Os testes automatizados foram executados com pytest e passaram, incluindo os três cenários obrigatórios: 2 km com pedido de R$ 50,00, 4 km com pedido de R$ 50,00 e 5 km com pedido de R$ 100,00.
