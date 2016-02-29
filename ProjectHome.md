# DA - Wireless Password Recovery #



É uma pequena ferramenta de recuperação de senha que permite visualizar os nomes de usuário e senhas armazenadas pelo serviço ” Configuração Automática de WLAN ” do Windows Vista, Windows 7, Windows 8 e Windows Server. A seguinte informação é exibida: nome de usuário, campo de senha descriptografada, além das informações do computador e usuário que efetuou o login. Você pode exportar todas estas informações para arquivo de texto.

## DA\_WifiPerfilEx DLL ##

Esta disponível uma Unmanaged DLL que contém todas as funções que você precisa, escrita para que você possa utilizar as funções Wifi de qualquer linguagem de programação, inclusive linguagens gerenciadas como Java e C#.

É uma dll desenvolvida em C++ escrita em código nativo (unmanaged), gerando uma interface com API Wifi do Windows onde é possível manipular o perfil de rede sem fio, sem precisar utilizar todos os requisitos necessários para isto, tais como elevação de direitos, contexto de usuário local, cripotografia e etc.

A dll possui seis funções Export em português Brasil para fácil entendimento, para saber mais sobre o funcionamento do código que manipula a API Wifi leia nosso post sobre como capturar senhas de rede sem fio nesta mesma categoria.

## Lista de Funções para exportação ##

```
static  DAWIFIPERFILEX_API std::wstring Perfil();
static  DAWIFIPERFILEX_API std::wstring Ssid();
static  DAWIFIPERFILEX_API std::wstring Tipo();
static  DAWIFIPERFILEX_API std::wstring Seguranca();
static  DAWIFIPERFILEX_API std::wstring Senha();
static  DAWIFIPERFILEX_API bool Conectado();
```

## Como Utilizar ##

<a href='http://www.youtube.com/watch?feature=player_embedded&v=FMQoTAkfJao' target='_blank'><img src='http://img.youtube.com/vi/FMQoTAkfJao/0.jpg' width='425' height=344 /></a>


---


### Junte-se a nós (Join Us) ###

Para participar envie um e-mail ou apenas nos ajude reportando um erro.

To Join us send an email or just help us reporting na issue.

desenvolvimento.aberto@live.com