---
typora-copy-images-to: upload

---

### Serviços Web

São soluções para aplicações se comunicarem independente de linguagem, softwares e hardwares utilizados.

São API's que se comunicam por meio de redes sobre o protocolo HTTP.

![img](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img0.png?raw=true)

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

  

![img1](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img01.png?raw=true)



- SOAP Envelope é o primeiro elemento do documento e é usado para encapsular toda a mensagem SOAP

- SOAP Header é o elemento onde possui informações de atributos e metadados de requisição.

- SOAP Body é o elemento que contém os detalhes da mensagem.

  #### Exemplo;

  ![img2](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img02.png?raw=true)

### WSDL

WSDL (Web Services Description Language), usado para descrever Web Services, funciona como um contrato do serviço. A descrição é feita em um documento XML, onde é descrito o serviço, especificações de acesso, operações e métodos.

### XSD

XSD (XML Schema Definition), é um schema no formato XML usado para definir a estrutura de dados que será validada no XML, o XSD funciona como uma documentação de como deve ser montado o SOAP Message (XML) que será enviado através de Web Service.

![img03](https://github.com/Cleber-Woheriton/desafio-github-repositorio/blob/main/Fundamentos_de_Arquitetura_de_Sistemas/img03.png?raw=true)

[Link da imagem](http://soapclient.com/xml/soapresponder.wsdl 

### SOAP na prática

Nesta etapa será usado a ferramenta Open Source do SOAP, caso gostaria de baixar, deixarei o [link.](https://www.soapui.org/downloads/soapui/)

Ao instalar a ferramenta e abrir será exibido a seguinte interface; 

