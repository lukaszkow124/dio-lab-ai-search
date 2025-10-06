# dio-lab-ai-search

# AI Search

## Criação dos recursos necessarios

Será necessario criar 3 recursos - AI Search, Storage Account e Azure AI Services.

### AI Search

Criar conforme imagens abaixo:

<img width="975" height="501" alt="image" src="https://github.com/user-attachments/assets/9c63431d-3f4a-40d1-a86d-b47c74ca2567" />

Seleccionar nome, grupo e pricing tier:

<img width="975" height="677" alt="image" src="https://github.com/user-attachments/assets/29bb3e5a-315e-44f1-92be-6451f357ce12" />

### Azure AI Services

Criar conforme imagens abaixo:

<img width="975" height="654" alt="image" src="https://github.com/user-attachments/assets/115c6e48-b1d6-4e6e-84bd-ea8020ef5fd8" />

Seleccionar dados conforme imagem abaixo:

<img width="975" height="626" alt="image" src="https://github.com/user-attachments/assets/de429a75-1d7f-49c5-a240-96cd75a95a18" />

### Storage account

Criar conforme imagens abaixo:

<img width="975" height="607" alt="image" src="https://github.com/user-attachments/assets/ce54cc50-4b11-4f8f-bf18-95b8265b2bf5" />

Seleccionar seguintes opções:

<img width="975" height="876" alt="image" src="https://github.com/user-attachments/assets/9f9f265b-d864-4988-926a-b5d4c2cea11b" />

Após criação mudar configurção default para permitir blob anonymous access:

<img width="975" height="796" alt="image" src="https://github.com/user-attachments/assets/f49f0fac-2cd8-45b4-b8c7-3cb7e19dbf25" />

## Carregamento dos documentos para criar base de pesquisa

Carregar no storage criado os documentos com classificação das lojas de cafes (documentos na pasta docs do repo):

<img width="975" height="350" alt="image" src="https://github.com/user-attachments/assets/af86c062-747c-4565-a4e9-84201121075e" />

<img width="975" height="386" alt="image" src="https://github.com/user-attachments/assets/a7840068-3f79-4549-8384-2c4e7fd92f4e" />


## Definição da fonte para serviço de pesquisa (AI Search)

Documentos carregados no passo anterior servem como base para serviço da pesquisa. Será necessario definir os mesmos como fonte dos dados.
Como tal será necessario importar dados atraves opção assinalada:

<img width="975" height="348" alt="image" src="https://github.com/user-attachments/assets/9920162c-7c8e-404c-8d39-969489424414" />

Preencher os dados em seguinte forma:

<img width="975" height="619" alt="image" src="https://github.com/user-attachments/assets/50867b35-8347-43f2-ae2d-a99bb00db1fa" />

> Connection string deve apontar para o nosso storage com ficheiros

### Enriquecimento dos dados com recurso do AI

Seleccionar as opções para fazer uso do AI para enriqucer os dados nos documentos:

<img width="975" height="575" alt="image" src="https://github.com/user-attachments/assets/1c49d248-500a-4ab4-9cfd-ce7003430486" />

<img width="975" height="248" alt="image" src="https://github.com/user-attachments/assets/2ae89dcc-7e36-432c-ae74-98f1ea89cc29" />

<img width="975" height="521" alt="image" src="https://github.com/user-attachments/assets/50f27fd0-4917-413d-a5f6-1314e8423a33" />

### Definir dados do indice

Configurar dados do indice em seguinte forma:

<img width="975" height="518" alt="image" src="https://github.com/user-attachments/assets/88044bb6-a0cf-4e28-8ef0-bb0f75346107" />

### Definir dados do indexer

Configurar dados em seguinte forma:

<img width="975" height="567" alt="image" src="https://github.com/user-attachments/assets/7bc33c99-c5d9-4758-8eb0-382196aaea05" />

### Estado do indexer

Verificar se indexer correu e processou os documentos:

<img width="975" height="381" alt="image" src="https://github.com/user-attachments/assets/9e1e143e-0868-4f2c-9bd5-88676277c3fd" />

## Explorar possibilidades de pesquisa sobre os dados importados

Pesquisa pela locação das classificações:

<img width="975" height="777" alt="image" src="https://github.com/user-attachments/assets/65e4dd02-8dba-442d-aa83-968572e99eac" />

Processo detetou localizações e retorno dados relativos ao query usada na pesquisa.

Pesquisa pelo sentimentos:

<img width="975" height="784" alt="image" src="https://github.com/user-attachments/assets/29b544f7-213b-4637-b007-3f9d86c59cef" />

Com enriqueciemnto o processo extraiu os sentimentos das classificações e permite efetuar pesquisa sobre o mesmo.

## Resumo

Ferramenta poderosa para mineração dos dados, que cria, com base nos dados não estruturados, o conjunto dos dados pesquisaveis nos varias vertentes.




