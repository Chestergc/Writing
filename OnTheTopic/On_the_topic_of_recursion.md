# On the topic of recursion

## Translation

Então. Eu estive assistindo um filme hoje que me deixou meio pra baixo. Nem era ruim o filme, eu só sei que querendo ou não eu odeio com cada fibra do meu ser quando os filmes que eu assisto não levam a lugar algum. Quando o universo do filme decide por ser recursivo e acabar exatamente onde começou.

Um sistema recursivo é autoreferencial, o que quer dizer que ele precisa de soluções que ele mesmo cria para responder a pergunta que ele está fazendo. Como todos os tópicos bons de se conversar a respeito na vida, este tem um exemplo simples e fácil de entender:

```py
def fact(x):
    if x==0:
      return 1
    else:
      return x * fact(x-1)
```
O que essa fórmula quer dizer é, olha se o número que está sendo passado é zero, se for, manda de volta, se não, o numero que a gente procura vai ser o número multiplicado pelo que voltar da função quando se colocar nela o número menos um.

Bem fácil de ver onde isso dá errado, coloque um número moderadamente pequeno nessa fórmula, como 100, e pra chegar no resultado se precisa passar pelo programa cem vezes, não é muito eficiente, e por estas e outras programadores tentam não usar recursividade em programas onde ela pode ser desmontada, eliminando a necessidade de um programa que referencia a sí mesmo.

O problema dessa veia de pensamento não é a programação, isso é só um jeito de pensar a respeito, o problema é quando a recursividade começa a aparecer no mundo real e as coisas começam a se tornar cíclicas.

Não deve ser surpresa pra maioria das pessoas que se importam o bastante pra ler isso que eu tenho passado por algumas crises de identidade nos últimos tempos. Eu não sei mas o que sou, não sei o que quero e não aguento mais viver a minha vida entre um momento feliz e outro.

E foi hoje a tarde que eu me dei conta do motivo pra não aguentar mais.

Eu ví Suicide Squad hoje. E quando a última cena começou a passar eu me dei conta de que, eu também, sempre volto pro mesmo lugar onde comecei, querendo ou não.

Eu sei o que vai acontecer daqui em diante:

* Em algumas semanas, ou quem sabe alguns mêses, eu vou arrumar alguém que eu vou acreditar ser o amor da minha vida.

* Nesse meio tempo eu vou estar entrando em algum campo de pesquisa que me agrada no momento, e vai ser o catalísta de algumas conversas boas que vamos ter.

* Eu vou começar a viver como uma pessoa normal por alguns mêses, eu vou ter um emprego, eu vou estudar.

* Eu vou fazer alguma coisa ridículamente incrível, que as pessoas da minha convivência não vão nem acreditar que foi ideia minha.

* Vou começar a ter autoestima de novo.

* Vou fazer mais algumas coisas legais que nunca vão sair do papel por um motivo ou outro e a pessoa que estiver comigo vai tentar me ajudar a fazer alguma delas, sem sucesso.

* Vou começar a ficar deprimido. Não desesperadoramente no começo, só o bastante pra dita pessoa notar.

* Alguma coisa vai acontecer. Nós vamos terminar. Eu vou ficar ainda mais depressivo.

* Reset.

O resultado do programa vai ser que eu vou ter algumas cicatrizes novas pra mostrar e umas histórias a mais pra lembrar.

Como aquela vez que nós andamos uns cem quilômetros a pé. Ou aquelas fotos que fizemos na galeria do café. Ou aquela vez que a gente ficou bebendo no estúdio e conversando a noite toda.

Eu não aguento mais ficar assim por saber que é assim que eu sempre fico.

Eu posso até fingir por um tempo que a minha vida mudou e que eu fugi do ciclo, mas a vida não muda, são pessoas diferentes passando pelas mesmas situações, em lugares diferentes.

Eu me sinto preso em uma rotina sem sentido, sozinho e sem vontade de conhecer mais ninguém, repetindo os mesmos erros por não saber o que mais eu posso fazer. Se eu pudesse colocar só mais uma cláusula no algoritmo.

```py
def life(drunk, loving):
  if drunk==True:
    return cycle1
  elif loving==True:
    return cycle2
  else:
    return 0;
```

Guilherme Chimello
