# TTL (Time to Live)

TTL (Time to Live) é o tempo de vida do pacote IP e serve justamente para que o pacote não fique vagando eternamente pela rede.

Cada vez que um pacote IP passa por um roteador (hop), o seu TTL é decrementado (-1) até se tornar 0. Quando o valor se torna 0, o roteador descarta o pacote.

Ele é um campo do protocolo IP e cada sistema operacional implementa um valor padrão para esse campo.

## Exemplo

- O Windows usa o TTL padrão de 128
- O Linux usa TTL padrão de 64
- O Unix usa TTL padrão de 255

Esses valores podem ser alterados pelo usuário.
