

## Part I – Answers for Debug Systems Issues

1. 

2. 

		1. 

		2. 


3. 


4. 



## Part II – Linux Laboratory

![A test image](lb.png)

### Criação da Máquina virtual, instalação e configuração do Sistema Operativo

No meu caso, utilizei a versão 6.x do virtual box, de onde criei uma máquina virtual e instalei o SO conforme proposto.
Garanti que todos pacotes estão actualizados, instalei o `net-tools` , o `openssh` e configurei Bridged Adapter como o tipo de rede para a VM em causa.

> **NOTA:** 
 *Aspectos ligados a segurança como o caso de alteração da porta default ssh, criação de utilizadores com privilégios limitados, login por par de chaves RSA, etc, não foram levados em consideração assumindo que não é o que está sendo avaliado. (Mas reconhecendo a necessidade).*

A partir do comando `scp wit-cicd-challenge.jar wit@192.168.31.12:/home/wit/`, garanti que o ficheiro `.jar` fosse carregado da minha máquina (windows no meu caso) para a VM.


### Processo de intalação do docker e garantir que irá executar sem o `sudo`



### Arquitetura e descrição da proposta


### Criação e configuração da rede

Antes de iniciar com a criação dos containers, foi criada um rede bridge para conectarmos posterior conectar todos os containers que forem criados. O seguinte comando foi utilizado para criar a rede com o nome redewit

`docker network create --driver=bridge redewit`

Executando `docker network ls`, será possível confirmar a existência da rede previamente criada.

### Criação e configuração do container SpringBoot



### Crianção e configuração do Proxy



### Criação e configuração do LB



### Configurações gerais do processo















