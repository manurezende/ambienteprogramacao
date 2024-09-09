# Preparação de ambiente
### Vamos preparar o ambiente para desenvolvimento de aplicações

#### Neste abiente iremos instalar e configurar os seguintes recursos:
- Maquina virtual (virtual box)
- Distribuição Linux(ubuntu server)
- Nasm
- Compilador da linguagem C
- Configurar o ip entre a maquina real e a virtual
- Configurar via SSH entre VSCode e o ServidorLinux
- Instalar as extensões: material, icon, nasm, SSH e linguagem C/C++

#### Maquina virtual (VirtualBox)

!["Logo VirtualBox"](logovirtual.png)

Máquina virtual é uma ferramenta que permite a criação de novos "computadores" e sistemas operacionais, para estudo e trabalho.

Para o nosso estudo iremos utilizar a VirtualBox, da Oracle.
Para instalar basta fazer o download no link a seguir:
<a href="https://www.virtualbox.org/wiki/Downloads" target="_blank"> VirtualBox </a>


##### criando a maquina virtual para o nosso estudo

- configuração:
    > - nome da maquina: servidor
    > - memoria: 4GB(4096)
    > - processador: 2
    > - disco: 100GB
    > - IP e porta do host: 127.0.0.1 e 22
    > - IP e porta do convidado: 10.0.2.15 e 22

- tela inicial de configuração
<img src=telaconfig1.png width=500 height=400>


- tela de configuração do hardware
<img src=telaconfig2.png width=850 height=300>



- tela de configuração do disco
<img src=telaconfig3.png width=850 height=300>


- tela de configuração final
<img src=telaconfig4.png width=850 height=300>


- tela de configuração de rede
<img src=telarede1.png width=550 height=400>


- tela de configuração do ip e das portas
<img src=telarede2.png width=950 height=300>

#### destribuição ubuntu server

  <img src=ubuntu.png width=200 height=200>

para o nosso estudo iremos utilizar uma distribuição linux paraa servidores chamada Ubuntu. Acompanhe o processo de intalação:


faça o download aqui:
<a href="https://ubuntu.com/download/server" target="_blank"> Ubuntu server </a>

- acompanhe a instalação

- tela de inicio da instalação

 <img src=instal1.png width=500 height=400>

 - seleção de idioma

 <img src=instal2.png width=500 height=300>

 - seleção de teclado

 <img src=instal3.png width=800 height=300>

 - tipo de tipo de intalação
 <img src=instal4.png width=800 height=300>

- configuração de rede
 <img src=instal5.png width=800 height=300>

- configuração do proxy
 <img src=instal6.png width=800 height=300>

- pacotes de atualização
<img src=instal7.png width=800 height=500>

- tela de configuração do disco
<img src=instal8.png width=800 height=500>

- configurações finais
<img src=instal9.png width=800 height=500>

- tela configuração do usuario
<img src=instal10.png width=800 height=500>

- tela configuração do ssh
<img src=instal11.png width=800 height=500>

- fim da instalação
<img src=instal12.png width=800 height=500>


#### atualização do sistema

Para correta utilização do servidor Ubuntu que acabamos de instalar, será necessario realizar a atualização do sistema.

Execute o comando a baixo:

```
sudo apt -y && sudo apt uograde -y
```
reinicie seu servidor usando o comando abaixo:

```
reboot
```

#### instalação do compilador NASM
O compilador do NASM é uma ferramenta que nos permite programar em Assembly. Assim é possivel criar programas que manipulam dados que estão nos registradores do processador.

Para instalar o NASM no Ubuntu, usamos o comando:
```
sudo apt install nasm -y
```

#### Instalação do compilador da linguagem C

Em Linux, o compilador da linguagem C é o GCC. Ele é uma ferramenta importante para o desenvolvimento de programas em C.

Para instalar use o comando:
```
sudo apt install gcc-y
```

#### Conexão servidor e VScode via SSH

Precisamos instalar uma estensão no VScode para acessar o nosso servidor de forma remota.

!["extensão SSH"](ssh.png)

Configuração do acesso remoto:

!["cofiguração SSH"](ssh1.png)