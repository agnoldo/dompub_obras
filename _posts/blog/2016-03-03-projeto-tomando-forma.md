---
categories: blog
layout: blog
title: Projeto tomando forma
subtitle: "Progresso do projeto em 03/03/2016"
permalink: "2016-03-03-projeto-tomando-forma/"
author: Arnaldo Gomes
author-link: "http://www.agnoldo.com/"
background: "rgb(119, 40, 23)"
published: true
---

Depois de duas semanas de dedicação parcial (afinal tenho emprego normal e ainda queridos esposa, filhos, família e amigos), retomei o projeto em caráter de dedicação exclusiva nesta semana. Em quatro dias o progresso foi muito interessante e posso informar que o projeto se encontra no seguinte estado:

- conversão de livros de PDF para EPUB: processo foi retomado após manutenção do nosso NAS. Mais de 10.000 obras já foram convertidas e estão sendo armazenadas em serviços de hospedagem em nuvem;

- desenvolvimento do _backend_: para melhorar o desempenho, houve uma mudança radical e muito bem sucedida no projeto. O _backend_ foi parcialmente transformado em arquivos estáticos armazenados no Github, em comparação à antiga opção por banco NoSQL. A melhoria de tempo de resposta e escalabilidade tem sido notável até agora;

- melhoria da interface do _app_ móvel: algumas melhorias no _backend_, tais como a conversão e o armazenamento em nuvem de capas de livros, tem gerado impacto positivo na interface do app móvel;

- criação de [comunidade Facebook](https://www.facebook.com/dominiopublicoxyz/) para discussões sobre o projeto e seu conteúdo;

- implementação de mecanismo básico de armazenamento (_backend_) e _download_ de obras (_app_ cliente). Para o _download_ foi utilizado o plugin [ngCordova Archive](http://ngcordova.com/).

Os próximos passos são:

- prosseguir com processo de conversão de livros, que está sendo realizado com o apoio da ferramenta [Calibre](https://calibre-ebook.com/);

- completar a importação do _backend_, que hoje conta com cerca de 10.000 obras em seu banco de dados;

- implementar, se possível, mecanismo de conta/_login_. A ideia principal do mecanismo de conta/_login_ é possibilitar o armazenamento de perfil de usuário no nosso _backend_ e mantê-lo automaticamente sincronizado entre diferentes dispositivos. Desta forma será possível a um usuário continuar a leitura entre diferentes clientes vinculados a uma mesma conta, conforme citado anteriormente ao explicarmos a opção pelo _PouchDB_;

- implementar, se possível, integração com redes sociais, tais como _Facebook_, _Twitter_ e _Google+_. Neste caso, implementar também mecanismo de compartilhamento de obras (sugestão por _post_) e, talvez, até envio de mensagens e resenhas;

- implementar, se possível, mecanismo de avaliação (_rating_) de obras em tela _Meus Dados_. Desta forma usuário poderá atribuir nota a obras consumidas;

- implementar ou remover tela _Recentes_, que mostrará as últimas obras recentemente abertas para reprodução;

- projetar e implementar tela _Configurações_.
