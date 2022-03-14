# Projeto-1---A-Jornada-do-Her-i
Projeto requisitado pela Blue EdTech. O projeto consiste em um programa simples com 5 perguntas, respondidas apenas em "sim" e "nao". Para cada quantidade de "nao"s respondidos, um final diferente é demonstrado.

//----------------------------- Textos ---------------------------------- //

Intro: "A lua ilumina você pela janela. Já é tarde, e você coça seus olhos, sonolento. Seu corpo pede por descanso, mas seu código ainda não estáa funcional. Pela última vez, você confere suas linhas de programação e torce para que não hajam mais erros..."

Questão 1? Você tomou todos as 5 xícaras de café?
Questão 2? Você já revisou todas as linhas do seu programa?
Questão 3? Você já rodou seu programa no terminal 3 vezes?
Questão 4? Você já inseriu o programa no GitHub?
Questão 5? Você se distraiu fazendo as 4 tarefas anteriores?

Você falha miseravelmente: Seus péssimos hábitos te tornam um péssimo programador. Revise seus comportamentos e melhore!
Você falhou: Talvez você não seja o pior dos piores, mas com certeza não está nem perto dos melhores. Tente melhorar!
Voce chegou perto: Você está na média. Preste atenção nos comportamentos que farão de você um dos melhores!
Voce conseguiu, mas podia ser melhor: Seu código funciona... 99% das vezes. Um pouco mais de atenção não teria sido ruim.
Você é o melhor: As vezes eu me esqueço que você é o melhor! Além de ser cuidadoso, você fez algo a mais, e conseguiu seu merecido descanso!

//-------------------------- Explicações -------------------------------//

1. Introdução: comando console.log + texto de introdução;
Adicionado de um console.log() para espaçamento.

2. Variáveis: 
contagem: variável responsável pelo referenciamento dentro da array "questoes";
questoes: array responsável pelo armazenamento das strings de perguntas;
respostas: array responsável pelo armazenamento das respostas;
a,b,c,d,e: variáveis responsáveis pelo gerenciamento de "Sim" e "Não";
r1,r2,r3,r4,r5: variáveis extraídas da array "respostas";
final: variável responsável pela averiguação em relação aos finais possíveis.

3. Funções: Enquanto a variável "contagem" for menor que 5, uma constante "index" é criada, entregando em forma de prompt as strings inseridas na array "questoes".
Esse prompt já recebe o sanatize para toLowerCase, transformadno as respostas em caracteres minúsculos, e inserindo as respostas dentro da constante index.
Por sua vez, a constante index é passa por tratamento, sendo verificada se corresponde a um string "sim" ou "nao". Se nao for referente a nenhum dos dois, um console.log é inserido com o texto "Sua resposta é inválida. Tente novamente."
E retorna a mesma pergunta, até receber um string "sim" ou "nao".

Se a constante index for "sim" ou "nao", ela armazena esse string na array "respostas", utilizando como referência a variável "contagem" para posicionamento.

Após a condição do while ser quebrada, ou seja, a variável "contagem" ser igual a 5, retiramos as strings de dentro da array "respostas" em forma de variáveis, denominadas "r1,r2,r3,r4,r5".

A partir de então, o código compara as variáveis "rn" com respostas em forma de string "sim" ou "nao".
Se a string for correspondente a "sim", a variavel referente ao "r" ("a,b,c,d,e") não recebe adição de valor.
Se a string for correspondente a "nao", a variável referente ao "r" ("a,b,c,d,e") recebe a adição de + 1.

Por fim, a variável "final" soma todas as variáveis "a,b,c,d,e".
Se o valor da variável "final" for igual a 5, então um console.log com o pior final é mostrado.
Se o valor da variável "final" for igual a 4 ou 3, então um console.log com o final ruim é mostrado.
Se o valor da variável "final" for igual a 2, então um console.log com o final medíocre é mostrado.
Se o valor da variável "final" for igual a 1, então um console.log com o final bom é mostrado.
Se o valor da variável "final" for igual a 0, então um console.log com o melhor final é mostrado.
