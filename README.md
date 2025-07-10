# An-lise-scar
Análise do padrão de nacionalidade e etnia dos ganhadores das principais categorias (para minha análise em questão, considerei apenas Diretor, Ator, Ator coadjuvante, Atriz e Atriz coadjuvante) da premiação do óscar desde a sua primeira edição até a última. O programa deve funcionar para as premiações que virão, contanto que o site o imdb não passe por mudanças estruturais no armazenamento de informação via HTML.

Os prompts são 100% funcionais e algumas condições devem ser levadas em conta para possíveis usuários:
1 - Não tenho muita prática em Web Scraping, provavelmente alguém com mais experiência resolveria os desafios que encontrei de maneira mais prática e direta.

2 - Nas primeiras edições do Óscar havia a categoria 'Diretor Assistente', essa categoria DEVE ser negligenciada e caso você as inclua os prompts não funcionarão.

3 - Você verá que eu dividi os programas para os anos de 1929 - 2004 e 2005 em diante. Essa divisão não é arbitrária, é onde existe a maior modificação na 
estrutura HTML do site, como não tenho muito prática preferi encerrar o programa ali e começar outro do zero.


Nesses arquivos você encontrará:


--- Prompts principais ---


Oscar_nacionalidade 1929 - 2004.ipynb ---> prompt de extração da nacionalidade dos vencedores das categorias nos anos em questão

Oscar_nacionalidade 2005 - 2025.ipynb ---> prompt de extração da nacionalidade dos vencedores das categorias nos anos em questão

Genero 1929 - 2004.ipynb ---> prompt de extração dos gêneros dos filmes que ganharam as categorias elencadas

Genero 2005 - 2025.ipynb ---> prompt de extração dos gêneros dos filmes que ganharam as categorias elencadas 

    Para exemplificar possíveis confusões: No óscar do ano de 1995 Jessica Lange recebe a estatueta de melhor atriz. O programa Oscar_nacionalidade 1929 - 2004
    entra no ano da premiação em questão, vê que a vencedora da noite foi Jessica Lange, entra em seu perfil vai URL e armazena seu local de nascimento (EUA). 
    O programa Genero 1929 - 2004, acessa o filme referente a essa vitória (Blue Sky) e armazena seus gêneros (Drama e Romance).

    
--- Prompts acessórios ---


HTML2004.ipynb ---> prompt usado para verificar a estrutura do site e o que diferia dos anos subsequentes. Foi usado apenas para me dar suporte do que fazer com os anos anteriores a 2005.

ETL_nacionalidade.ipynb ---> prompt usado para fazer a ETL de alguns pontos, adicionar etnia aos atores e preparar os dados para utilização no PowerBI.


--- Arquivos CSV ---


Todos os arquivos csv gerados pelos prompts aramazenando as informações.


--- Arquivo pbix ---


Analise diversidade oscar.pbix ---> o Dashboard interativo mostrando análises pertinentes.


DISCLAIMER: 

Essa é uma produção completamente didática, especulatória e sem qualquer fim lucrativo. Eu compreendo a complexidade do termo 'etnia' e aqui foi feita uma análise extremamente simplória apenas para provar, objetivamente, a hegemonia estado-unidense das premiações, bem como a distribuição quase que totalitária dos prêmios para pessoas brancas.
