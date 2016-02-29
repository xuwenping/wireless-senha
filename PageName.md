Unmanaged Dll

É uma dll criada com código C/C++ nativo ou seja é desenvolvida com código não gerenciado e será compilada em linguagem de máquina para executar diretamente no hardware.

DA\_WifiPerfilEx.dll

É uma dll desenvolvida em C++ escrita em código nativo (unmanaged), gerando uma interface com API Wifi do Windows onde é possível manipular o perfil de rede sem fio, sem precisar utilizar todos os requisitos necessários para isto, tais como elevação de direitos, contexto de usuário local, cripotografia e etc.

A dll possui seis funções Export em português Brasil para fácil entendimento, para saber mais sobre o funcionamento do código que manipula a API Wifi leia nosso post sobre como capturar senhas de rede sem fio nesta mesma categoria.

static  DAWIFIPERFILEX\_API std::wstring Perfil();
static  DAWIFIPERFILEX\_API std::wstring Ssid();
static  DAWIFIPERFILEX\_API std::wstring Tipo();
static  DAWIFIPERFILEX\_API std::wstring Seguranca();
static  DAWIFIPERFILEX\_API std::wstring Senha();
static  DAWIFIPERFILEX\_API bool Conectado();

Código Aberto

Disponibilizamos esta dll em uma solução Open Source desenvolvida no Microsoft Visual Studio, escrita em C++   e dividida em dois projetos o primeiro, o DA\_APP é um projeto C++ MFC visual de onde efetuamos a chamada da dll e testamos seus retornos, o segundo é o wawifiperilex.dll e que gera a dll que controla e retorna todo o gerenciamento da API Wifi .


Uso

A Dll pode ser usada por outras linguagens e chamar funções diretamente da API  Wifi do Windows sem precisar se preocupar todos os complexos detalhes para manipular código em um nível mais baixo. Na imagem abaixo temos o resultado da compilação em C++, mas você pode usar esta dll de qualquer linguagem que suporte código unmanaged.

Exemplo:

Este código é usado para chamar a dll nativa de uma linguagem baseada no Windows Framework, onde não é permitido o uso por referencia de uma dll que não seja criada para código CLR. No exemplo abaixo é possível chamar a senha wieless descriptografada diretamente do C#.

Visual Studio - C#

Por Exemplo, no visual Studio para poder compilar código unmanaged é necessário alterar as propriedades do projeto. Na janela de propriedades do projeto, na opção Debug, Enable Debug, clique em: Enable Native Code Debugging.
