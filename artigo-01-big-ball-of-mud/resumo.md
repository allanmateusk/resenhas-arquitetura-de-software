Resenha Crítica – Big Ball of Mud (Foote & Yoder,
1997)
O artigo “Big Ball of Mud”, de Brian Foote e Joseph Yoder, apresenta uma reflexão
realista sobre a arquitetura de software predominante no mundo real. Diferente dos
modelos ideais ensinados em livros e defendidos por arquiteturas formais e padrões
bem estruturados, os autores analisam o que de fato acontece na prática: sistemas que
crescem de forma desorganizada, orientados por necessidades imediatas e pressões de
mercado, resultando em estruturas caóticas, difíceis de manter e com baixa coesão.
O conceito de “Big Ball of Mud” descreve sistemas que surgem de decisões
incrementais, correções rápidas e protótipos que nunca foram descartados. Ao longo do
tempo, pequenas adaptações acumulam complexidade estrutural, levando à erosão da
arquitetura original — quando ela existe. Funções longas, código duplicado, ausência de
documentação, uso excessivo de variáveis globais e forte acoplamento entre módulos
são sintomas comuns desse padrão.
Entretanto, o artigo não condena esse fenômeno de maneira simplista. Pelo contrário,
os autores argumentam que a “lama” não surge por incompetência, mas como resposta
a forças reais: pressão por prazo, limitação de recursos, mudanças constantes de
requisitos, rotatividade de equipe e necessidade de manter o sistema funcionando a
todo custo. Em muitos contextos, priorizar entrega sobre arquitetura é uma decisão
economicamente racional.
Um dos pontos mais relevantes do texto é a relação entre crescimento incremental e
erosão arquitetural. O padrão “Piecemeal Growth” mostra que sistemas evoluem por
pequenas alterações contínuas. Quando essas mudanças não são acompanhadas por
refatoração e consolidação, a estrutura degrada-se gradualmente. O padrão “Keep It
Working” reforça essa ideia ao destacar que sistemas críticos não podem parar, o que
dificulta intervenções estruturais profundas.
Ao refletir sobre minha experiência no último estágio na PRODEMGE, no projeto da
Receita Estadual, é possível observar claramente a aplicação prática dos conceitos do
artigo. Tratava-se de um sistema antigo, que cresceu lentamente ao longo de anos,
sem acompanhar a evolução dos princípios modernos de desenvolvimento. A base de
código era fortemente legada, com funções espalhadas por múltiplos módulos e forte
acoplamento entre camadas.
Pequenas alterações de regra de negócio frequentemente exigiam modificações em
diversos pontos do sistema. Não havia uma separação clara de responsabilidades,
muitas validações estavam duplicadas, e a ausência de documentação tornava o
processo de entendimento lento e arriscado. Era comum que uma simples mudança
gerasse efeitos colaterais inesperados em outras partes do código.
Essa situação reflete exatamente o padrão “Big Ball of Mud”. O sistema não era
necessariamente mal-intencionado em sua concepção; ele simplesmente evoluiu sob
pressões institucionais e operacionais. Como sistema governamental, não podia parar.
Portanto, priorizava-se manter o funcionamento — mesmo que isso implicasse
acréscimo de complexidade técnica.
O padrão “Sweeping It Under the Rug” também se manifestava de forma indireta.
Frequentemente, criavam-se novas camadas ou métodos intermediários apenas para
isolar partes mais críticas do código legado. Embora isso não resolvesse a raiz do
problema, permitia que novas funcionalidades fossem adicionadas com menor risco.
Por outro lado, a reconstrução total (“Reconstruction”) era impraticável. Sistemas
governamentais possuem alto custo de substituição e grande dependência institucional.
Assim, a estratégia viável era a melhoria incremental e a refatoração gradual — quando
possível.
Conclui-se que o artigo de Foote e Yoder permanece extremamente atual. Ele oferece
uma visão madura sobre arquitetura de software, reconhecendo que excelência técnica
não ocorre isoladamente de fatores econômicos e organizacionais. A principal lição é
que compreender as forças que levam à formação de uma “Big Ball of Mud” é o
primeiro passo para mitigá-las.
Mais do que evitar a lama, é necessário aprender a evoluir sistemas de forma
consciente, equilibrando entrega de valor imediato com sustentabilidade técnica de
longo prazo. A experiência na PRODEMGE evidencia que ignorar princípios de
arquitetura pode não impedir o sistema de funcionar — mas certamente tornará sua
evolução cada vez mais custosa e arriscada.