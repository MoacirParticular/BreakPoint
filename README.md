# Debug (Ainda não esta pronto)

### Você, às vezes, se sente travado em alguma tarefa, sem conseguir evoluir? Fica olhando para o computador, com a tarefa ali, e não consegue avançar? Você precisa de uma opinião de alguém, mas não consegue?

A solução para algum problema relacionado à realização de uma tarefa pode estar na técnica Rubber Duck Debugging, que está em explicar sua tarefa para o Rubber Duck, um pato de borracha. Esta é uma técnica lúdica para utilizar a criatividade e resolver problemas relativamente complexos.

O método é descrito assim:
>Peça, pegue emprestado, compre, faça você mesmo ou de alguma outra forma, obtenha um pato de borracha.
>Coloque o pato sobre sua mesa de trabalho e diga a ele que você vai apenas explicar alguns trechos de código para ele.
>Explique ao pato o que o código deveria fazer. Explique com o máximo de detalhes, linha a linha.
>Em algum ponto da explicação, você vai perceber que algo do que você está dizendo é mentira. O que você diz que o código deveria fazer, não é realmente o que ele faz. 
>O pato continuará sentado, sereno, contente pelo conhecimento avançado que ele tem de programação ter te ajudado a descobrir o problema com o código.

[Rubber duck debugging](http://en.wikipedia.org/wiki/Rubber_duck_debugging)

[Vanessa Moura](https://www.youtube.com/watch?v=5sE3_CjwnR0)

Esse é o método do pato de borracha. Embora seja muito efetivo, algumas vezes são necessários truques extras para facilitar a vida do querido pato. Então, agora que você já conhece o método principal, vamos aos métodos que vez por outra quebram um galho até você encontrar o pato.

Para exemplificar as técnicas discutidas abaixo, será utilizado um código muito simples. Crie um projeto de uma única view e na implementação desta view utilize o seguinte código:

```

- (void)viewDidLoad 
  { 
    [super viewDidLoad]; 
    [self performSelector:@selector(metodoInexistente:)]; 
  }
  
 ```

O código acima chama o método metodoInexistente em self, que é um UIViewController. Este método não está implementado, então quando a execução do app chegar a este ponto, o app vai travar e o programador verá uma tela mais ou menos como a da Figura 2 abaixo.

![](https://github.com/MoacirParticular/MoacirParticular/blob/main/Imagens/baby-yoda-soup.gif)

Mas que código é esse ? 
_Pensando isso você está?_

Pois é se você não sabe, deveria saber, todo programador swift deve pelo menos entender um código Objective-C, um dia você vai se deparar com um e ai vai lembrar de mim.....

_vamos voltar para o nosso tutorial de Debug._ ![](https://github.com/MoacirParticular/MoacirParticular/blob/main/Imagens/chewbacca.png)




