![Logo](https://www.tbforte.com.br/images/logo-tb-forte.png)

# Portal TBForte - API Backend
_Web API para gestão de solicitações de video, no processo de contagem dos malotes, na mesa de tesouraria_

![](https://img.shields.io/static/v1?label=Nuget&message=v6.0.13&color=blue&style=<STYLE>&logo=<LOGO>) ![](https://img.shields.io/static/v1?label=.NET-Core&message=v6.0&color=purple&style=<STYLE>&logo=<LOGO>) ![](https://img.shields.io/static/v1?label=ASP.NET-Core&message=v6.0&color=purple&style=<STYLE>&logo=<LOGO>) ![](https://img.shields.io/static/v1?label=EF-Core&message=v6.0&color=blue&style=<STYLE>&logo=<LOGO>)

***
## Documentation
* [**Environment**](#environment)
* [**Instalation**](#instalation)
* [**Setup**](#setup)

***
## Environment
- [![](https://img.shields.io/badge/Git-E44C30?style=for-the-badge&logo=git&logoColor=white)](http://git-scm.com/) 
- [![](https://img.shields.io/badge/Visual_Studio-5C2D91?style=for-the-badge&logo=visual%20studio&logoColor=white)](https://visualstudio.microsoft.com/)
- [![](	https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/products/docker-desktop/)
- [![](https://img.shields.io/badge/Microsoft_SQL_Server_2019-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)](https://learn.microsoft.com/pt-br/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver15)

  _`Caso sistema operacional seja windows, ative o WSL`_
 - [![](https://img.shields.io/badge/WSL-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://learn.microsoft.com/pt-br/windows/wsl/install)

***
## Instalation
_`Caso sistema operacional seja windows, use o Git Bash`_ 
#### _Clone este repositório_
```bash
$ git clone ssh://git-codecommit.us-east-1.amazonaws.com/v1/repos/BRSP_tbforte_portal
```
#### _Acesse o diretório_
```bash
$ cd BRSP_tbforte_portal
```
#### _Faça download das imagens e crie os containeres_
```bash
$ docker-compose up
```
***
## Setup
- _Acesse a pasta do projeto via explorador de arquivos_
![Captura de tela_20221111_200146](https://user-images.githubusercontent.com/26409244/201442904-ce2ed8c0-15f5-4d96-9fde-553198a6f6a6.png)
- _execute o arquivo .sln_

![Captura de tela_20221111_201701](https://user-images.githubusercontent.com/26409244/201443197-98118051-5a1b-40e6-8f0c-1efdedcd5fe6.png)
- _No Visual Studio, mude o contexto de docker-compose para WebAPI_

https://user-images.githubusercontent.com/26409244/201445511-403ec4df-3f47-4d8a-a320-94dcdb6e85ac.mp4

***
