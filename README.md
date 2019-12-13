# Previsão de Reprovação dos alunos da educação básica do Distrito Federal através do Censo Escolar

## O que é o Censo Escolar
O Censo Escolar é o principal instrumento de coleta de informações da educação básica e a mais importante pesquisa estatística educacional brasileira. É coordenado pelo Inep e realizado em regime de colaboração entre as secretarias estaduais e municipais de educação e com a participação de todas as escolas públicas e privadas do país.

Ele abrange as diferentes etapas e modalidades da educação básica e profissional:
- Ensino regular (educação infantil, ensino fundamental e médio);
- Educação especial – modalidade substitutiva;
- Educação de Jovens e Adultos (EJA);
- Educação profissional (cursos técnicos e cursos de formação inicial continuada ou qualificação profissional).

A coleta de dados das escolas tem caráter declaratório e é dividida em duas etapas. A primeira etapa consiste no preenchimento da Matrícula Inicial, quando ocorre a coleta de informações sobre os estabelecimentos de ensino, gestores, turmas, alunos e profissionais escolares em sala de aula. A segunda etapa ocorre com o preenchimento de informações sobre a Situação do Aluno, e considera os dados sobre o movimento e rendimento escolar dos alunos, ao final do ano letivo.

(Fonte: [Site do Inep](http://portal.inep.gov.br/censo-escolar))

Os microdados do CENSO ESCOLAR são publicados anualmente e contém informações sobre as matrículas dos alunos, turmas onde os alunos estão matriculados, docentes e escolas.

## Objetivo Geral
Classificar os alunos matriculados no ensino fundamental do Distrito Federal em APROVADOS ou REPROVADOS de acordo com as características encontradas na tabela de matrículas da base de dados do CENSO ESCOLAR do INEP.

## Objetivos Específicos
* Selecionar as características individiais dos alunos que podem ser utilizadas neste projeto, tais como: transporte escolar utilizado, condição física do aluno, etc;
* Identificar as características mais importantes que podem auxiliar a classificar um aluno como APROVADO ou REPROVADO;

## Metodologia
Para treinar o algoritmo, vamos utilizar a base de dados do ano subsequente para determinar os alunos que foram reprovados. Para isso, vamos identificar os alunos pelo campo ID_ALUNO e verificar aqueles que cujo campo TP_ETAPA_ENSINO permaneceu inalterado de um ano para o outro. Desta forma, a base de dados de um determinado ano será utilizado para treinar o algoritmo e o do ano subsequente para testá-lo.
