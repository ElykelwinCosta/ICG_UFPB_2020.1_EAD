Primeira atividade – Introdução à Computação Gráfica – 2020.1

A atividade passada pelo professor tinha como missão fazer download do programa OpenGL disponível no repositório da disciplina, compilar e executar este programa. 
Uma vez compilado, ao ser executado, o programa deveria apresentar uma janela contendo um triângulo colorido, como na Figura 1.
















Eu comecei a atividade no Windows 7, fiz o Download do programa, e partir para pesquisar como compilar e executar o mesmo no Windows, porém o que encontrei foi um monte de informações espalhadas, sem um padrão especifico, e que muitas vezes utilizava de certas “gambiarras“ para criar e executar programas em OpenGL.

Primeiramente tentei com o CodeBlocks, seguindo esse vídeo tutorial: Instalando e configurando OpenGL no codeblocks / windows, até consegui executar, e apareceu o triângulo colorido como solicitado, porém, percebi que estava rodando um executável de fora da pasta /modern_opengl, e além disso o triângulo ficava girando, como demonstrado na Figura 2.



Continuei tentando no CodeBlocks, porém sem sucesso, então parti para o Visual Code 2019.
Comecei com esse tutorial, porém não obtive sucesso, ficou dando um erro de inicialização do programa, como demonstrado na figura 3.


Então, como não consegui sucesso de forma alguma, adquiri um curso de OpenGL na Udemy, como apresentado na Figura 4.


Porém também não obtive sucesso, pois no curso é utilizado o Cmake, enquanto no projeto é utilizado o Makefile, e eu, por inexperiência, não consegui compilar, então por recomendação de colegas e por ver mais facilidade na instalação, decidi partir para o Ubuntu.

Depois de várias pesquisas sobre como utilizar o OpenGL no Ubuntu, encontrei um tutorial, ensinando a compilar códigos em C e OpenGL no Ubuntu, e quando tudo parecia perfeito, novamente dei de cara com um erro. O código compilou, o triângulo apareceu, porém todo em branco, como apresentado na figura 5.






Como já estava sem saber o que fazer perguntei aos colegas se alguém teve o mesmo problema, e um deles me indicou que adicionasse um comando, export MESA_GL_VERSION_OVERRIDE=3.3, antes de compilar o código, como demonstra a Figura 6.


Porém deu o mesmo erro da Figura 5, então decidi pesquisar, e acabei encontrando uma questão com o mesmo problema que o meu no StackOverflow, como mostra a Figura 7




E enfim o caso foi solucionado. Na verdade utilizando esse comando, ou o comando do colega, dá certo do mesmo jeito, só que eu tenho que colocar esse comando e o executável do programa tudo junto para rodar e eu estava colocando separado, o que fazia com que esse comando fosse inútil. Mas apesar de todos os contratempos a missão foi cumprida, como mostra a Figura 8.



Referências:
Como configurar OpenGL no Visual Studio Windows
Compilando código em C e OpenGL no Linux
How can I get Opengl 3.3 (with GLSL 3.3) support through mesa on an Intel HD Graphics 3000 iGPU?

Instalando e configurando OpenGL no codeblocks / windows

Learn OpenGL
