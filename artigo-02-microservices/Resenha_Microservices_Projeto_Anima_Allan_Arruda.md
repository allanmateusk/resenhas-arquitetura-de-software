Resenha crítica: Arquitetura de Microservices
aplicada ao Projeto Anima na DTI Sistemas
O artigo “Microservices”, escrito por Martin Fowler e James Lewis, apresenta os princípios
fundamentais da arquitetura de microsserviços e discute como esse estilo arquitetural pode
melhorar a escalabilidade, manutenção e evolução de sistemas modernos. A proposta central dos
autores é a construção de aplicações como um conjunto de pequenos serviços independentes, que
se comunicam por meio de mecanismos leves, geralmente APIs HTTP. Essa abordagem contrasta
com o modelo tradicional de sistemas monolíticos, onde toda a aplicação é construída e implantada
como uma única unidade.
Os autores argumentam que a arquitetura de microsserviços surgiu como resposta às limitações
dos sistemas monolíticos. Em aplicações monolíticas, qualquer pequena alteração exige a
reconstrução e implantação de todo o sistema. Com o crescimento da aplicação, esse modelo
tende a se tornar difícil de manter, escalonar e evoluir. Nesse contexto, os microsserviços surgem
como uma alternativa capaz de dividir a aplicação em partes menores, independentes e focadas
em capacidades específicas do negócio.
Uma das principais características destacadas no artigo é a organização dos serviços em torno das
capacidades do negócio. Em vez de dividir equipes e sistemas por camadas técnicas — como
interface, lógica de negócio e banco de dados — os microsserviços incentivam a divisão baseada
em domínios funcionais. Isso permite que equipes multidisciplinares sejam responsáveis por todo o
ciclo de vida de um serviço, desde o desenvolvimento até a operação em produção. Esse conceito
é frequentemente associado à filosofia “you build it, you run it”, na qual o time que desenvolve
também mantém o serviço em funcionamento.
Outro ponto importante apresentado pelos autores é o uso de endpoints inteligentes e canais de
comunicação simples. Em vez de concentrar a lógica de integração em ferramentas complexas
como ESBs (Enterprise Service Bus), a arquitetura de microsserviços prefere que cada serviço
contenha sua própria lógica de negócio e utilize mecanismos simples de comunicação, como APIs
REST ou sistemas de mensageria. Essa abordagem aumenta a autonomia dos serviços e reduz a
dependência de componentes centralizados.
Esses conceitos podem ser observados na prática em projetos modernos de desenvolvimento de
software, como o Projeto Anima desenvolvido na empresa DTI Sistemas. Nesse projeto, o objetivo
principal é fornecer benefícios e descontos para estudantes, integrando diferentes sistemas e
serviços responsáveis por gerenciar usuários, validação de estudantes e aplicação de descontos
em produtos ou serviços.
Durante minha atuação no projeto, utilizei principalmente C# no backend para desenvolver APIs
responsáveis pela lógica de negócio do sistema. Essas APIs processam solicitações relacionadas à
verificação de elegibilidade de estudantes e à aplicação de benefícios associados ao programa. No
frontend, foi utilizado o framework Vue.js para construir interfaces dinâmicas e responsivas,
permitindo que os usuários consultem e utilizem os descontos disponíveis.
Embora o sistema não seja composto por dezenas de microsserviços independentes, muitos dos
princípios apresentados por Fowler e Lewis podem ser identificados na arquitetura utilizada. Por
exemplo, a separação entre backend e frontend representa uma divisão clara de responsabilidades
dentro do sistema. O backend expõe APIs que encapsulam a lógica de negócio, enquanto o
frontend consome essas APIs para apresentar informações ao usuário de forma interativa.
Outro aspecto relevante é a preocupação com a modularidade do sistema. Mesmo dentro de uma
aplicação baseada em APIs, a organização do código em camadas bem definidas permite que
funcionalidades sejam modificadas ou evoluídas sem afetar todo o sistema. Essa prática se
aproxima da ideia de componentes substituíveis descrita no artigo, que enfatiza a importância de
dividir sistemas em partes que possam evoluir de maneira relativamente independente.
O uso de APIs também facilita a integração com outros sistemas, algo essencial em um projeto
como o Anima, que depende de informações externas para validar estudantes e aplicar benefícios.
Essa integração reforça o conceito de comunicação entre serviços através de interfaces bem
definidas, um dos pilares da arquitetura de microsserviços.
Em conclusão, o artigo de Fowler e Lewis apresenta uma visão abrangente sobre a arquitetura de
microsserviços e seus impactos no desenvolvimento de software moderno. No contexto do Projeto
Anima na DTI Sistemas, foi possível observar na prática a aplicação de vários desses conceitos,
especialmente na separação entre backend e frontend, na utilização de APIs e na organização
modular do sistema. Essa experiência demonstra como os fundamentos teóricos apresentados no
artigo podem ser aplicados em ambientes corporativos, contribuindo para o desenvolvimento de
sistemas mais flexíveis, escaláveis e alinhados às necessidades do negócio.