<h1 align="center">
  <img alt="Fastfeet" title="Fastfeet" src=".github/logo.png" width="300px" />
</h1>

<h3 align="center">
  Desafio final: FastFeet 
</h3>

<p>Esse projeto é o Desafio Final para emissão do Certificado do Bootcamp GoStack, que se constitui de uma aplicação completa (Back-end, Front-end e Mobile) de gerenciamento logístico de uma transportadora fictícia chamada FastFeet.</p>

## Sobre o desafio

FastFeet é uma aplicação de logística, feito com o intuíto de auxiliar no gerenciamento e no controle das entregas de encomendas.

Esse auxílio é feito através de ferramentas que permitem, ao administrador, o cadastro de entregadores, destinatários e encomendas; a associação destas encomendas aos entregadores que, por sua vez, administram suas entregas através do aplicativo mobile; e o gerenciamento dos problemas ocorridos nas entregas possibilitando, eventualmente, o cancelamento das mesmas.

No aplicativo mobile, o entregador tem acesso às encomendas atribudas a ele (pendenetes e já concludas); tem os recursos de confirmação de retirada de encomenda e de entrega conclúida (atestada por uma foto da assinatura do destinatário); e, também, a possibilidade de cadastrar um problema com uma entrega especfica e visualizar o histórico de problemas atribuídos.

As tecnologias utilizadas no desenvolvimento, foram: Node.js, ReactJS e React Native.

## Back-end

Para executar o back-end é preciso acessar, via terminal, a pasta 'backend' e seguir os seguintes passos:

**1.** Criar novos containers de Postgres e Redis no Docker, com o comando:

`docker`

**2.** Startar bancos de dados no Docker, com o comando: 

`docker start db_fastfeet redisfastfeet`

**3.** Gerar as tabelas no banco de dados, através das migrations e seeds do Sequelize, com os comandos:

`yarn sequelize db:migrate`

e

`yarn sequelize db:seed:all`

**4.** Configurar o MailTrap no arquivo 'src/config/mail.js' com o 'user' e 'pass' da sua conta.

**5.** Finalmente, executar o comando `yarn dev` para rodar a api.

## Web

Esse desafio **não precisa ser entregue** e não receberá correção. Além disso, o código fonte **não está disponível** por fazer parte do **desafio final**, que será corrigido para **certificação** do bootcamp. Após concluir o desafio, adicionar esse código ao seu Github é uma boa forma de demonstrar seus conhecimentos para oportunidades futuras.

## Mobile

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.
