## Um olhar sobre os alunos do 9º ano da rede pública do estado do RJ focado no desempenho em matemática 

#### Tema
Uma análise do desempenho em matemática e de alguns aspectos do perfil socioeconômico dos alunos do 9º ano das escolas públicas do estado do RJ.

### Contexto e escolha do tema
Um grupo de professores de matemática pretende oferecer aulas gratuitas dessa disciplina para alunos da rede pública do estado do RJ. Eles preferem prestar esse serviço para estudantes do último ano do ensino fundamental para que eles ingressem no ensino médio sem nenhuma pendência no aprendizado de matemática. Para isso, esse grupo de professores voluntários gostaria de ter informações sobre o desempenho desses estudantes em matemática e conhecer um pouco mais esta população (por exemplo, que região tem o pior e melhor desempenho, qual gênero e cor costumam ter o pior e o melhor desempenho, se esses alunos têm acesso à internet em casa, qual a proporção de alunos que já foram reprovados na escola alguma vez etc.). Com essas informações em mãos, eles poderão tomar decisões como em qual região atuar e como abordar a disciplina em suas aulas.
A escolha deste tema nasceu de um antigo projeto de uma amiga, que infelizmente acabou não saindo do papel. A ideia era justamente reunir um grupo de professores voluntários para oferecer apoio no aprendizado de matemática aos alunos do ensino fundamental da rede pública do RJ. Talvez a breve análise apresentada neste projeto ajude a estimulá-la (ou outras pessoas) a concretizar esta ideia.

### Sobre as bases de dados
Nesta análise foram utilizados os microdados do Sistema de Avaliação da Educação Básica (Saeb) referentes às avaliações aplicadas em 2021 e do  Indicador de Nível Socioeconômico (Inse), mensurado com base no questionário socioeconômico aplicado pelo Saeb. 
O Saeb é uma pesquisa realizada pelo Instituto Nacional de Estudos e Pesquisas Educacionais Anísio Teixeira (Inep) a cada dois anos, por meio de provas e questionários, que possibilita diagnosticar a educação básica do Brasil e identificar fatores externos à experiência no ambiente escolar propriamente dito que podem interferir no desempenho dos alunos. São avaliados nesta pesquisa todos alunos matriculados no 5º e no 9º ano do ensino fundamental e nas 3ª e 4ª séries do ensino médio da rede pública e uma amostra de estudantes da rede privada de áreas rurais e urbanas.
Os microdados do Saeb estão disponíveis neste link: https://www.gov.br/inep/pt-br/areas-de-atuacao/avaliacao-e-exames-educacionais/saeb/resultados. Para esta análise utilizei a planilha referente aos resultados dos alunos do 9º ano, chamada **TS_ALUNO_9EF**. E os microdados do Inse podem ser consultados aqui: https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/indicadores-educacionais/nivel-socioeconomico. Utilizei a base de dados do link Escolas **(Atualizado em 10/05/2023)**.

O Indicador de Nível Socioeconômico do Inep, o Inse, é calculado com base nos microdados dos questionários respondidos pelos alunos que fazem a prova do Saeb. As questões giram em torno da renda familiar, do nível de escolaridade dos pais, acesso à internet, cor, gênero, idade, tempo dedicado aos estudos etc., possibilitando que se conheça um pouco mais a realidade social dos alunos da rede de ensino avaliada. Neste link há uma descrição de cada nível do índice, que abrange uma escala de 1 a 8: chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://download.inep.gov.br/areas_de_atuacao/Indicadores_de_nivel_Nota_tenica_2021.pdf. Resumidamente, o nível 1 diz respeito aos estudantes que responderam possuir itens básicos em casa (uma geladeira, uma televisão, um banheiro) e cujos pais têm um nível de escolaridade que varia entre o 5º ano do ensino fundamental incompleto e o ensino fundamental completo. Já no extremo oposto, o nível 8, se refere aos estudantes que responderam possuir em casa a quantidade máxima indicada de cada bem no questionário (três ou mais televisões, três ou mais banheiros, três ou mais celulares com internet, dois ou mais computadores etc.) e cujos pais têm nível superior completo. 

O ideal seria que todos os microdados disponíveis nas bases do Inep fossem analisados e discutidos neste projeto, porém isso não será possível no prazo definido. Então, foram selecionadas algumas perguntas do questionário que nos ajudam a conhecer mais a população analisada. São elas:
1. Qual é o seu gênero?
2. Qual é a sua cor?
3. Qual é a sua idade?
4. Quantos computadores têm na sua casa? 
5. Quantos celulares com internet têm na sua casa?
6. Na sua casa tem Wi-fi?
7. Você já foi reprovado(a)? 
8. Fora da escola em dias de aula, quanto tempo você usa para estudar?

Creio serem perguntas que podem auxiliar os professores a decidir o lugar e com qual segmento da população atuar. Por exemplo, com base nas informações coletadas, eles podem decidir auxiliar somente (ou pricipalmente) estudantes negros, caso o desempenho deles se prove ser mais baixo que o dos estudantes de outras etnias. Ou ainda talvez decidam atender somente a população feminina e negra de uma determinada região. (Estes são só alguns exemplos, as possibilidades são várias.)

### Sobre a análise exploratória dos microdados 
A princípio, a análise procura descobrir qual é o desempenho de matemática dos alunos do 9º ano da rede pública do estado do RJ com base na proficência em matemática calculada pelo Saeb. Portanto, as primeiras perguntas feitas para os dados foram: Qual é a proficiência em matemática dos alunos do 9º ano das escolas públicas do estado do RJ? E no interior e na capital?
Com base nessa pergunta, podemos comparar o desempenho dos alunos e perceber em qual região há uma necessidade maior de auxílio nessa disciplina.
Posteriormente, exploramos os dados a cerca do questionário socioeconômico para conhecermos um pouco mais o perfil desses estudantes, como a idade deles; quantos já foram reprovados ou não; se eles têm acesso à internet e a dispositivos eletrônicos em casa; a proporção de negros, brancos, indígenas e amarelos; e a proporção de meninos e meninas.  
A partir dessa exploração, procurei extrair informações como a proficiência em matemática entre os alunos negros e comparar o segmento desta população que apresenta proficiência abaixo da média do estado (que acredito ser a população que de fato interessa aos professores) com os alunos brancos também com uma poficiência abaixo da média. Também foi feita uma comparação da proficiência em matemática por gênero. 
Por fim, foram explorados os dados do Inse, que nos informam quais segmentos da rede de ensino (municipal, estadual ou federal), e em qual localidade (capital ou interior), apresentam escolas com índice socioeconômico mais baixo, que seriam o foco desses professores voluntários.

### Ferramentas utilizadas na análise
Python e as bibliotecas pandas, matplotlib e seaborn para o tratamento da base de dados e a análise exploratória.
Tableau para a criação do dashboard.

Dê uma olhada no dashboard neste link (ou no PDF incluído neste repositório): https://public.tableau.com/app/profile/mariana.oliveira3648/viz/Projeto-Reprograma/Histria1?publish=yes

Acesse as bases de dados tratadas nesse link: https://drive.google.com/drive/folders/1pYr3YyNw4899jbjIxcmIHMP7sokJ6mQb?usp=sharing
