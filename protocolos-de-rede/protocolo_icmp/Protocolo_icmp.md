# Protocolo ICMP

O Protocolo ICMP (Internet Control Message Protocol) é um protocolo de alerta por mensagens, ele basicamente emite avisos sobre a situação da rede.

A estrutura básica do ICMP é composta de tipos e códigos, cada um com sua função:

| Type                        | Code                     | Checksum                          |
| --------------------------- | ------------------------ | --------------------------------- |
| 0 - echo reply              | 0 - ping echo            | Resposta do ping                  |
| 8 - echo request            | 0 - ping echo request    | Envio do ping                     |
| 11 - time exceeded          | 0 - TTL exceeded         | O TTL foi excedido (zerou)        |
| 3 - destination unreachable | 0 - Network unreachable  | Rede não encontrada               |
|                             | 1 - Host unreachable     | Host não encontrado               |
|                             | 3 - Port unreachable     | Porta não encontrada              |
|                             | 4 - fragmentation needed | O pacote precisa ser fragmentado. |

## Exemplo da importância do ICMP 

Ao enviar um ping para um host inexistente na rede, temos como retorno um **Destination Host Unreachable**, indicando que o host de destino não foi encontrado. Sem o aviso do protocolo ICMP, não teríamos nenhum retorno sobre o que ocorreu na rede.

![Destination Host Unreachable](https://github.com/OliveiraaX/protocolos-de-rede/blob/main/protocolos-de-rede/img/destination-host-unreachable-1.png)
