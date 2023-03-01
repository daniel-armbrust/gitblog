---
title: "O que é Cloud Computing?"
description: "O post tem o objetivo de descrever em linhas gerais o que é Cloud Computing."
date: 2020-06-25T10:20:42-03:00
lastmod: 2020-06-25T10:20:42-03:00
featuredImage: "/blog/images/featured_image-1593112059-o-que-e-cloud-computing.jpg"
rssFullText: true
draft: false
comment:
  enable: true
---

## 1. Introdução

Algumas das muitas definições existentes para o termo Cloud Computing:

- Cloud Computing é um modelo computacional no qual é possível provisionar recursos de TI sob demanda, de 
acordo com o seu negócio e pagar somente pelo uso que se faz. Em sua essência, é uma nova forma de se 
provisionar recursos e serviços de TI.

- É uma forma de entrega/aluguel de recursos computacionais (servidores, storage, banco de dados, rede, 
software, etc), através da Internet.

- É uma nova arquitetura  no qual muda-se para uma nova forma de se adquirir TI. Agora paga-se pelo uso 
dos recursos em um modelo que se adequa a demanda, o que se convencionou chamar de elasticidade. Esta 
nova forma de aquisição de serviços de infraestrutura de TI reduz custo, e aumenta a produtividade.

- ***Simon Wardley, "Cloud Computing - Why IT Matters" - OSCON 09***
  - Cloud Computing é um termo genérico usado para descrever a transformação disruptiva da TI em uma economia 
  baseada em serviços, impulsionada por um conjunto de condições econômicas, culturais e tecnológicas.

{{< raw >}}
   <br>
{{< /raw >}}

{{< youtube okqLxzWS5R4 >}}

{{< raw >}}
   <br>
{{< /raw >}}

- ***2008, Gartner***
  - "...um estilo de computação no qual recursos escaláveis e elásticos habilitados para TI, são fornecidos 
  como um serviço a clientes externos que usam tecnologias da Internet."

- ***Forrester Research***
  - "...capacidades de TI (serviços, software ou infraestrutura) entregues via tecnologias da Internet em um 
  modelo self-service no qual se paga somente por aquilo que é usado."

- ***2009/2011, NIST (National Institute of Standards and Technology)***
  - Cloud Computing é um modelo para permitir acesso onipresente, conveniente e de rede sob demanda, a um 
  conjunto compartilhado de recursos de computação configuráveis (redes, servidores, armazenamento, aplicativos 
  e serviços) que podem ser rapidamente provisionados e liberados, com o mínimo esforço de gerenciamento ou 
  interação do provedor de serviços. Esse modelo de nuvem é composto de cinco características essenciais, três 
  modelos de serviço e quatro modelos de implantação."

- ***Cloud Computing: Concepts, Technology & Architecture. Prentice Hall, 2013***
  - "A computação em nuvem é uma forma especializada de computação distribuída que introduz modelos de utilização 
  para provisionar remotamente recursos escaláveis e medidos."

## 2.Definições do NIST

De acordo com o *[NIST (National Institure of Standards and Technology)](https://www.nist.gov/)*, *Computação em Nuvem*
é um modelo que permite acesso através da Internet a um conjunto de recursos computacionais (rede, armazenamento, 
servidores, serviços, etc) nos quais podem ser rapidamente criados e apagados, de forma fácil, sem a necessidade 
de qualquer intervenção humana (ex: ligar para um *Helpdesk* para solicitar a criação de um servidor).

Um provedor de *Computação em Nuvem*, ***deve possuir algumas características que são essenciais***. Além disso, um usuário 
deve ser capaz de *implementar sua aplicação (deploy)* ou *provisionar sua infraestrutura*, sobre um dos 
***três modelos de serviços existentes***. 

### Características essenciais

Estas são características essenciais que devem estar presentes quando falamos de *Computação em Nuvem*. Basicamente, um 
provedor de serviços deve minimamente possuir:

- **Autoatendimento sob demanda (On-demand self-service)**
  - Um consumidor pode criar servidores, redes, banco de dados, etc, conforme sua demanda, sem necessitar de qualquer 
  intervenção humana.

- **Amplo acesso à rede (Broad network access)**
  - Os recursos computacionais estão disponíveis através da rede (Internet) e são acessados via mecanismos padronizados, 
  e que podem ser utilizados por celulares, tablets, laptops ou estações de trabalho.

- **Conjunto de recursos (Resource pooling) / Multitenancy**
   - Os recursos computacionais de um provedor são agrupados para servir múltiplos clientes, isolados uns dos outros, 
   através de um modelo conhecido como multi-tenant (multilocatário). Os diferentes recursos físicos e virtuais, são 
   dinamicamente atribuídos e reatribuídos, de acordo com a necessidade do cliente. O cliente geralmente não tem controle 
   ou conhecimento sobre a localização exata dos recursos fornecidos pelo provedor de cloud. Porém, o provedor normalmente 
   especifica a localização em nível de país, estado ou datacenter.

- **Rápida elasticidade (Rapid elasticity)**
  - Os recursos computacionais podem ser criados e apagados a qualquer momento. Os clientes devem ter a impressão de que 
  os recursos são ilimitados (podem ser adquiridos em qualquer quantidade e a qualquer momento).
  - A elasticidade é uma propriedade fundamental. É ela quem dá o “poder” para se dimensionar recursos computacionais, 
  diminuindo ou expandindo-os facilmente, com o mínimo de atrito. Além de maximizar a utilização dos recursos (utilizar 
  somente o necessário e escalar somente quando necessário), possibilita redução de custo trazendo benefícios ao negócio.
  - Elasticidade é uma das "fortes considerações" que os consumidores levam em conta quando planejam a adoção da Computação em Nuvem.

- **Serviço medido (Measured service)**
   - É a habilidade que um provedor de serviços cloud tem em relação ao acompanhamento da utilização dos recursos 
   de TI pelos seus consumidores.
   - O provedor de serviços em cloud automaticamente controla, monitora e otimiza o uso dos recursos pelos clientes. 
   Isto também é reportado, provendo transparência tanto para o provedor de serviços quanto para os clientes que 
   utilizam os serviços.

{{< raw >}}
   <br>
{{< /raw >}}

- ***[NIST - Definition of Cloud Computing](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-145.pdf)***
- ***[NIST - Cloud Computing Reference Architecture](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication500-292.pdf)***

### Modelo de Serviços

Além das características essenciais, um provedor deve ser capaz de oferecer serviços dentro das modalidades abaixo:

- ***IaaS - Infrastructure as a Service (Infraestrutura como serviço)***
   - É a capacidade que um provedor de serviços tem de oferecer uma infraestrutura de processamento (compute), 
   armazenamento (storage) e rede (network). O consumidor não precisa se preocupar em gerenciar a virtualização, 
   infraestrutura física ou mesmo os dispositivos de rede.
   - Exemplo(s): *[Oracle Cloud - OCI](https://www.oracle.com/cloud/), [Amazon Web Services (AWS)](https://aws.amazon.com/), 
   [DigitalOcean](https://www.digitalocean.com/), [Linode](https://www.linode.com/), 
   [Google Compute Engine (GCE)](https://cloud.google.com/compute/).*

- ***PaaS - Platform as a Service (Plataforma como serviço)***
   - O provedor de serviços oferece uma plataforma que permite os usuários executar, desenvolver ou gerenciar aplicações. 
   Este modelo abstrai detalhes relacionados a infraestrutura de base como rede, virtualização e o sistema operacional.
   Ambiente *"ready-to-use"*, já com os recursos pré-configurados e pronto pra uso.
   - Exemplo(s): *[Heroku](https://www.heroku.com/)*

- ***SaaS - Software as a Service (Software como serviço)***
   - É o modelo mais comum e amplamente utilizado. São aplicativos hospedados na nuvem que funcionam sem necessitar 
   realizar download ou instalação local. Neste modelo, não há gerenciamento ou controle da infraestrutura de base 
   (redes, servidores, sistema operacional, etc).
   - Exemplo(s): *[Oracle Commerce](https://www.oracle.com/applications/customer-experience/ecommerce/), 
   [Oracle ERP Cloud](https://www.oracle.com/applications/erp/), [Google G Suite](https://gsuite.google.com/), 
   [Trello](https://trello.com/), [Gmail](https://www.google.com/gmail/about/).*

{{< raw >}}
   <br>
{{< /raw >}}

{{< youtube 36zducUX16w >}}

{{< raw >}}
   <br>
{{< /raw >}}

### Modelo de Serviços

- ***Nuvem Pública***
   - A infraestrutura da Computação em Nuvem é disponibilizada e comercializada para o público em geral. 
   - Este é o modelo mais utilizado e vendido ao público por grandes corporações como *Oracle*, *Google*, *Microsoft* e *Amazon*.

- ***Nuvem Privada***
   - A infraestrutura da Computação em Nuvem é para uso exclusivo de uma única organização. 
   - As tecnologias Cloud são utilizadas dentro de ambientes controlados.

- ***Nuvem Comunitária***
   - A infraestrutura da Computação em Nuvem é utilizada por uma comunidade particular de clientes de diferentes 
   organizações que compartilham interesses em comum. 
   - A administração da nuvem comunitária, normalmente é feita por administradores da própria comunidade ou às vezes por um terceiro.

- ***Nuvem Híbrida***
   - A infraestrutura da Computação em Nuvem normalmente é composta de duas ou mais nuvens (privada, comunitária 
   ou pública) conectadas entre si. 
   - Neste modelo, um consumidor pode escolher provisionar recursos de TI "mais sensíveis", em termos de segurança, 
   em sua nuvem privada, e recursos "menos sensíveis" serem provisionados em nuvem pública.
   - Como exemplo, a *Oracle* possui uma máquina chamada *Oracle Cloud at Customer*. Esta por sua vez implementa toda a 
   tecnologia da Computação em Nuvem dentro do datacenter do cliente. Além disto, esta máquina se conecta aos serviços 
   de nuvem pública da *Oracle*.

### Terminologias

Algumas terminologias que estão presentes quando falamos em *Computação em Nuvem*:

- **Alta disponibilidade (High Availability - HA)**
  - Ambientes computacionais configurados para estarem sempre disponíveis (24 horas, 7 dias por semana, 31 dias por 
  mês e 365 dias do ano). Esses ambientes possuem equipamentos de hardware redundantes, além da arquitetura de software 
  ser projetada em alta disponibilidade (não possuem um ponto único de falha). Quando existe qualquer falha, componentes 
  de backup são utilizados de forma transparente e sem causar impacto ao usuário final.

- **Tolerante a falhas (Fault Tolerance)**
  - Descreve como um provedor de Computação em Nuvem, garante o mínimo de indisponibilidade para os serviços que são 
  vendidos aos seus consumidores.

- **Escalabilidade (Scalability)**
  - Representa a capacidade de um recurso de TI em lidar com demandas de uso que aumentam ou diminuem.
  - Diferentes meios referente a escalabilidade dos serviços:
    - *Scaling out/in*
      - Conhecido como escalabilidade horizontal.
      - Alocação ou liberação de recursos de TI do mesmo tipo.
      - *Scaling Out* → adição de recursos.
      - *Scaling In* → remoção de recursos.
    - *Scaling up/down*
      - Conhecido como escalabilidade vertical.
      - Menos comum de ser utilizado pois existe indisponibilidade dos recursos envolvidos.
      - Um recurso de TI é substituído por outro recurso de maior ou menor capacidade.
      - *Scaling Up* → substitui um recursos por um de maior capacidade.
      - *Scaling Down* → substitui um recurso por um de menor capacidade.