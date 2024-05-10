# Ping

Normalmente utilizado para verificar a comunicação de rede entre hosts. O resultado permite saber se a comunicação está ocorrendo, medir o tempo de resposta e detectar problemas de lentidão.

Na imagem abaixo foi enviado um ping e no protocolo ICMP, nós temos o `Type: 8 (Echo (ping) request)` com o código 0:
![Ping Enviado](https://github.com/OliveiraaX/protocolos-de-rede/blob/main/protocolos-de-rede/img/Ping%20Enviado.png)

Se estiver tudo certo o servidor responderá com o `Type: 0 (Echo (ping) reply)`:
![Servidor Recebendo](https://github.com/OliveiraaX/protocolos-de-rede/blob/main/protocolos-de-rede/img/Servidor%20Recebendo.png)

Às vezes, o protocolo ICMP pode ser bloqueado por um firewall no host em que você está efetuando o teste.
