# Introdução #

Windows Wireless: API nativa Wifi.

As chaves de rede sem fio ( WEP / WPA ) são  armazenadas em seu computador  pelo serviço ” Configuração Automática de WLAN ” do Windows Vista, Windows 7, Windows 8 e Windows Server 2008. Você pode facilmente ler, descriptografar.

O Windows Vista ou versão superior não converte o WPA- PSK  em uma nova chave de valor binário como Windows XP , mas simplesmente mantem a chave original que você digita. Assim, sob o Windows Vista ou superior , a chave WPA- PSK original que você digitou é exibida no formato de chave ASCII.

Se o processo é executado no contexto da conta LocalSystem no mesmo computador, então você pode desencriptar material de chave.

Utilizando este método é possível também desencriptar qualquer outra senha armazenada pelo sistema operacional Windows.

Desenvolvido em C++

blog do programa:

http://desenvolvimentoabertotools.wordpress.com/2014/03/17/captura-senha-de-rede-wireless-versao-1-0-alpha-windows/

Como funciona o programa:

http://desenvolvimentoaberto.wordpress.com/2014/01/25/como-ler-senhas-de-redes-sem-fio-wireless/