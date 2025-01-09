# Phishing para captura de senhas do Facebook

### Ferramentas

- Kali Linux
- setoolkit

### Configurando o Phishing no Kali Linux

- Acesso root: ``` sudo su ```
- Iniciando o setoolkit: ``` setoolkit ```
- Tipo de ataque: ``` Social-Engineering Attacks ```
- Vetor de ataque: ``` Web Site Attack Vectors ```
- Método de ataque: ```Credential Harvester Attack Method ```
- Método de ataque: ``` Site Cloner ```
- Obtendo o endereço da máquina: ``` ifconfig ```
- URL para clone: http://www.facebook.com

## Resutados

![Alt text](./passwd.png "Optional title")

### Executando Exercício

#### Problema encontrado
- Felizmente (para a segurança do site) o Facebook possui uma tecnologia que impede esse tipo de clonagem, fazendo com que as senhas e e-mails sejam criptografadas.

#### Solução
Depois de ver o que seria possível fazer para burlar essa criptografia, foi feito o seguinte:

- Depois que entrei no site, salvei o template como "index.html".

![Alt text](./img1.png "Optional title")

- Também foi necessário entrar no "View Page Source".

![Alt text](./img2.png "Optional title")

- No "View Page Source" eu copiei todo o código que estava na página.

![Alt text](./img3.png "Optional title")

- No arquivo index que salvei, abri ele como bloco de notas e colei o código que havia copiado.

![Alt text](./img4.png "Optional title")

- Então pesquisei no bloco de notas a palavra "Button" até encontrar o botão de login com um ID, então apaguei esse ID e salvei o arquivo.

### Usando o Setoolkit

- Em vez de selecionar a opção de clonar um site, eu escolhi a opção 3 "Custom Import".

![Alt text](./img5.png "Optional title")

- Coloquei onde estava localizado o arquivo 'index.html'.

![Alt text](./img6.png "Optional title")

- Foi necessário tambem o url do site do facebook.

- Então foi criado a copia.

## Resultado
![Alt text](./resultado.png "Optional title")