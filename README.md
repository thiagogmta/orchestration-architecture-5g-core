# Orchestration Architecture for The 5G Core



## Descrição do Projeto

Este projeto versa sobre a preparação de um ambiente local para execução do núcleo 5G de forma orquestrada através do Kubernetes. Com o objetivo de instanciar nossa infraestrutura localmente utilizaremos o Minikube que permite a criação de um cluster Kubernetes no seu host local.

<p align="center">🚀 Em construção... 🚧</p>



## Instalação do Kubernetes e Minikube

> Para este guia foi utilizado as configurações de Hardware e Software listadas a seguir que servem apenas como registro da ambientação. Não significa portanto que que este guia não possa ser aplicado num ambiente com características físicas diferentes. As ferramentas descritas podem ser executadas no Windows, Linux e Mac.:
>
> - Notebook Dell Inspiron 7460
>   - Processador: Intel i5 7th Gen
>   - Memória 16 GB DDR 4
>   - HD: 320 GB SSD
> - Windows Pro 65 bits
>   - Virtual Box 6.1

Para instalação do Kubernetes e Minikube recomendo o material oficial do [Kubernetes ](https://kubernetes.io/docs/tasks/tools/) que disponibiliza material de instalação para todas as plataformas.

### Preparando...

Inicialmente iremos instalar o Chocolatey:

**Windows Terminal (opicional)**

Passo opcional mas recomendável é instalar o windows terminal através da loja de aplicativos do windows. Este terminal oferece mais funcionalidades que o padrão do sistema.

**Chocolatey**

O chocolatey é um gerenciador de pacotes para Windows. Iremos utiliza-lo para instalação do kubernetes.

1. Abra o terminal como administrador (segure shift e clique com o botão direito do mouse no ícone do terminal > Executar como administrador).
2. Cole o seguinte comando:

```shell
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

Ao teclar [ENTER] o chocolatey será instalado.

## Instalação do Kubernetes

> O kubernetes é uma ferramenta para orquestração de containers.

Com o terminal no modo administrador execute:

```powershell
choco install kubernetes-cli
```

Criando um diretório (**definir**)

```
mkdir .kube
cd .kube
```

## Instalação do Minikube

> O minikube é uma ferramenta que permite a execução do kubernetes em um computador local. Essa ferramenta irá criar um cluster kubernetes localmente para teste em seu computador local.

Novamente com o terminal em modo administrador iremos utilizar o chocolatey para instalação do minikube:

```shell
choco install minikube
```



### Autor

---



 <sub><b>Thiago Guimarães Tavares</b></sub>

[![Gmail Badge](https://img.shields.io/badge/-thiagogmta@gmail.com-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:thiagogmta@gmail.com)](mailto:thiagogmta@gmail.com)