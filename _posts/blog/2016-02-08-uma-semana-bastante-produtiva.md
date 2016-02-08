---
categories: blog
layout: blog
title: Uma semana bastante produtiva
subtitle: "Progresso do projeto em 08/02/2016"
permalink: "2016-02-08-uma-semana-bastante-produtiva/"
author: Arnaldo Gomes
author-link: "http://www.agnoldo.com/"
background: "rgb(119, 40, 23)"
published: true
---
## Uma semana bastante produtiva

Retornei as atividades com o projeto na semana passada, dia 2. Hoje, dia 8, posso informar que o projeto se encontra no seguinte estado:

- conversão de livros de PDF para EPUB: por causa de um _crash_* no nosso NAS, este processo foi paralisado ainda no seu início. Menos de 4.000 obras foram convertidas. Estamos aguardando uma "folga" para tentarmos recuperar o disco que entrou em modo degradado (ou então substitui-lo);

- desenvolvimento do _backend_: os primeiros dias deste período de forte dedicação ao projeto foram dedicados a esta tarefa. No momento as funcionalidades de Biblioteca, Favoritos e Meus Arquivos já estão praticamente 100% operacionais no nosso _backend_. Ah, optamos pela dupla [CouchDB](http://couchdb.apache.org/) (servidor\*\*)/[PouchDB](http://pouchdb.com/) (cliente) para viabilizar a futura sincronização de progresso de leitura entre diferentes clientes vinculados a uma mesma conta (exemplo: usuário lê no smartphone e continua no tablet);

- melhoria da interface do _app_ móvel: muitas melhorias foram feitas na interface. O destaque vai para o menu lateral e para a remoção de diversos bugs chatos na interação. Também foi implementada a função de busca textual sensível ao contexto em quase todas as telas do _app_.

Os próximos passos são:

- consertar problema do NAS o mais rápido possível;

- após o NAS consertado, prosseguir com processo de conversão de livros, que está sendo realizado com o apoio da ferramenta [Calibre](https://calibre-ebook.com/);

- também após o NAS consertado, implementar a importação completa do _backend_, que hoje conta apenas com cerca de 4.000 obras em seu banco de dados;

- implementar mecanismo de armazenamento (_backend_) e _download_ de obras (_app_ cliente). Para o _download_ será necessário provavelmente usar o plugin [ngCordova Archive](http://ngcordova.com/) ou similar;

- implementar mecanismo de conta/_login_. A ideia principal do mecanismo de conta/_login_ é possibilitar o armazenamento de perfil de usuário no nosso _backend_ e mantê-lo automaticamente sincronizado entre diferentes dispositivos. Desta forma será possível a um usuário continuar a leitura entre diferentes clientes vinculados a uma mesma conta, conforme citado anteriormente ao explicarmos a opção pelo _PouchDB_;

- implementar, se possível, integração com redes sociais, tais como _Facebook_, _Twitter_ e _Google+_. Neste caso, implementar também mecanismo de compartilhamento de obras (sugestão por _post_) e, talvez, até envio de mensagens;

- implementar, se possível, mecanismo de avaliação (_rating_) de obras em tela _Meus Dados_. Desta forma usuário poderá atribuir nota a obras consumidas;

- implementar ou remover tela _Recentes_, que mostrará as últimas obras recentemente abertas para reprodução;

- projetar e implementar tela _Configurações_.


* Isto também não estava no _script_. É o segundo _crash_ em seis meses no nosso NAS.

\*\* Tecnicamente estamos usando o serviço [Cloudant](https://cloudant.com/), da IBM. Trata-se de um _fork_ bastante compatível com o CouchDB mas com recursos adicionais interessantes, tais como busca textual (com auxílio do [Lucene](https://lucene.apache.org/)).
