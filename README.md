![Logo](https://www.tbforte.com.br/images/logo-tb-forte.png)

# Portal TBForte - API Backend
_Web API para gestão de solicitações de video, no processo de contagem dos malotes, na mesa de tesouraria_

![](https://img.shields.io/static/v1?label=Nuget&message=v6.0.13&color=blue&style=<STYLE>&logo=<LOGO>)

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

![Captura de tela_20221114_185653](https://user-images.githubusercontent.com/26409244/201776480-f228095e-3db2-4ac5-8944-5f342fe733af.png)

- _No Visual Studio, mude o contexto de docker-compose para WebAPI_

![recording-2022-11-14-18-51-58](https://user-images.githubusercontent.com/26409244/201776051-bc457200-fe76-48ca-aaf1-91395725360d.gif)

- _Abra o arquivo **appsettings.json**, altere o valor do atributo **Server** na string de conexão, para **127.0.0.1,1433**_

![recording-2022-11-14-19-07-42](https://user-images.githubusercontent.com/26409244/201778330-e9155395-66b4-4202-944d-05910eaf9677.gif)

- _Abra o **Management Studio**, conecte no server criado pelo docker. Usando as informação da string de conexão, criar um Database com o mesmo nome usado no atributo **Database**_

![image](https://user-images.githubusercontent.com/26409244/201780929-9608d4a8-8636-4705-b0e6-58acc03bdec7.png)

- _No Visual Studio, abra o gerenciador de soluções do nuget, digite o comando **update-database**. Isso criara as tabelas no banco de dados_

![recording-2022-11-14-19-13-44](https://user-images.githubusercontent.com/26409244/201779521-02f548af-92f4-4592-9f54-0befb927c467.gif)

- _Altere novamente, o valor do atributo **Server** na string de conexão, para **db**_
- _Altere novamente o contexto do projeto para **docker-compose** e execute o projeto_

![recording-2022-11-14-19-35-57](https://user-images.githubusercontent.com/26409244/201782658-d41c0ed8-7e07-48c6-b90e-2f6da7303d92.gif)

***
## Tecnologias

As seguintes tecnologias foram usadas na construção do projeto:

- [.NET Core 6](https://learn.microsoft.com/pt-br/dotnet/)
- [ASP.NET Core 6](https://learn.microsoft.com/pt-br/aspnet/core/?view=aspnetcore-6.0)
- [Entity Framework Core 6](https://learn.microsoft.com/pt-br/ef/core/)
- [Microsoft Identity Web](https://learn.microsoft.com/pt-br/azure/active-directory/develop/microsoft-identity-web)
