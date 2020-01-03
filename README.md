# desligaServidor
Fiz esse script para passar aos clientes caso necessitem desligar o servidor para algum tipo de manutenção. Ex: Manutenção elétrica, desligar o servidor antes que a bateria do nobreak acabe, ou qualquer outro bom motivo que seja.

Adicione o usuário desligar e altere o shell do user em /etc/passwd de:

desligar:x:1011:0:,,,:/home/desligar:/bin/bash

para

desligar:x:1011:0:,,,:/home/desligar:/sbin/desligar

Coloque o script em /sbin e logue com ssh
