---
typora-copy-images-to: upload

---

### Serviços Web

São soluções para aplicações se comunicarem independente de linguagem, softwares e hardwares utilizados.

São API's que se comunicam por meio de redes sobre o protocolo HTTP.

![img](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img/img0.png?raw=true)

## Vantagens


- Linguagem comum
- Integração
- Reutilização de Implementação
- Segurança
- Custo

## Principais Tecnologias

- SOAP

- REST

- XML

- JSON

  SOAP é um protocolo baseado em XML para acessar serviços web principalmente por HTTP. É independente de plataforma e software. O meio de transporte genérico, ou seja, pode ser usado por outros protocolos além do HTTP.

  XML (Extensible Markup Language) é uma linguagem de marcação criada na década de 90 pela W3C, facilita a separação de conteúdo, não tem limitação de criação de tags, é uma linguagem comum para integrações entre aplicações.

  #### Estrutura do SOAP Message

  

![img1](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img/img01.png?raw=true)



- SOAP Envelope é o primeiro elemento do documento e é usado para encapsular toda a mensagem SOAP

- SOAP Header é o elemento onde possui informações de atributos e metadados de requisição.

- SOAP Body é o elemento que contém os detalhes da mensagem.

  #### Exemplo;

  ![img2](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img/img02.png?raw=true)

### WSDL

WSDL (Web Services Description Language), usado para descrever Web Services, funciona como um contrato do serviço. A descrição é feita em um documento XML, onde é descrito o serviço, especificações de acesso, operações e métodos.

### XSD

XSD (XML Schema Definition), é um schema no formato XML usado para definir a estrutura de dados que será validada no XML, o XSD funciona como uma documentação de como deve ser montado o SOAP Message (XML) que será enviado através de Web Service.

![img03](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img/img03.png?raw=true)

[Link da imagem](http://soapclient.com/xml/soapresponder.wsdl 

### SOAP na prática

Nesta etapa será usado a ferramenta Open Source do SOAP, caso gostaria de baixar, deixarei o [link.](https://www.soapui.org/downloads/soapui/)

Ao instalar a ferramenta e abrir será exibido a seguinte interface; 

![img04](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img/img04.png?raw=true)

Em seguida inicia um serviço SOAP, clicando em SOAP, irá ser exibida a seguinte janela;

![img05](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img/img05.png?raw=true)

Com o novo projeto SOAP aberto, insira as informações necessárias para o novo serviço, como na seguinte imagem:

![img06](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img/img06.png?raw=true)

No campo WSDL colei o link http://soapclient.com/xml/soapresponder.wsdl, ele preenche o campo nome automático, em seguida ok.

Irá criar um novo projeto, binding e os métodos já definidos na XSD e o WSDL, e poderá ser executado e poderá ver o seu funcionamento na prática. 

### REST

Rest (Representational State Transfer - Transferência Representacional de Estado), é um estilo de arquitetura (design de arquitetura) de software que define a implementação de um serviço web. Podem trabalhar comos formatos XML, JSON ou outros.

#### Vantagens de se utilizar o REST

Permite integração entre aplicações e também entre cliente e servidor em páginas web e aplicações, utiliza dos métodos HTTP para definir a operação que está sendo efetuada. e possuí uma arquitetura de fácil compreensão.

Estrutura do REST

![img07](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img/img07.png?raw=true)

### API

API (Application Programming Interface), são conjuntos de rotinas documentos e disponibilizados por uma aplicação para que outras aplicações possam consumir suas funcionalidades. Ficou popular com o aumento dos serviços web, as maiores plataformas de tecnologia disponibilizam APIs para acessos de suas funcionalidades, algumas delas são: Facebook, Twitter, Telegram, Whatsapp, GitHub... 

### Principais Métodos HTTP

- GET - Solicita a representação de um recurso.
- POST - Solicita  a criação de um recurso.
- DELETE - Solicita a exclusão de um recurso.
- PUT - Solicita a atualização de um recurso.

### JSON

JSON (JavaScript Object Notation), possuí uma formatação leve utilizada para troca de mensagens entre sistemas, usa-se de uma estrutura de chave e valor e também de listas ordenadas. Um dos formatos mais populares e mais utilizados para troca de mensagens entre sistemas.

Exemplo;

![img08](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img/img08.png?raw=true)

### Código de Estado

O código de estado é usado pelo servidor para avisar o cliente sobre o estado da operação solicitada. [link para consulta especificada.](https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Status)

- Cód 100 + = Informativo.
- Cód 200 + = Sucesso.
- Cód 300 + = Redirecionamento.
- Cód 400 + = Erro do Cliente.
- Cód 500 + = Erro do Servidor.

