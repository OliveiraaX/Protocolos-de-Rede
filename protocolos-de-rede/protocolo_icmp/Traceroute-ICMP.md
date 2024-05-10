## Entendendo o TTL Excedido

Quando o TTL se torna 0, normalmente o roteador utiliza o protocolo ICMP para avisar, utilizando o Tipo 11 e Código 0. Isso ocorre porque o TTL foi excedido (zerou), e o roteador descarta o pacote.

| Type                | Code               | Descrição                      |
| ------------------- | ------------------ | ------------------------------ |
| 11 - time exceeded  | 0 - TTL exceeded   | O TTL foi excedido (zerou)     |

Mas é possível manipular o TTL para descobrir o caminho e a rota que o pacote percorre.

Utilizando o comando `traceroute -n`, podemos mapear toda rota traçada.

![traceroute](https://github.com/OliveiraaX/protocolos-de-rede/blob/main/protocolos-de-rede/img/traceroute.png)
