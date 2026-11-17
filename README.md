# GAN Lab: Uma Ferramenta de Experimentação Visual e Interativa para Redes Adversárias Generativas

Por 
[Minsuk Kahng](https://minsuk.com),
[Nikhil Thorat](https://nikubaba.com),
[Polo Chau](https://poloclub.github.io/polochau/),
[Fernanda Viégas](http://www.fernandaviegas.com) e 
[Martin Wattenberg](https://www.bewitched.com)

## Visão Geral

O GAN Lab é uma ferramenta inovadora de visualização interativa para qualquer pessoa aprender e experimentar com Redes Adversárias Generativas (GANs, do inglês *Generative Adversarial Networks*), uma classe popular de modelos complexos de aprendizado profundo (*deep learning*). Com o GAN Lab, você pode treinar interativamente modelos GAN para distribuições de dados 2D e visualizar seu funcionamento interno, de forma semelhante ao [TensorFlow Playground](http://playground.tensorflow.org/).

O GAN Lab utiliza o [TensorFlow.js](https://js.tensorflow.org/), uma biblioteca de aprendizado profundo acelerada por GPU que roda diretamente no navegador. Tudo, desde o treinamento do modelo até a visualização, é implementado em JavaScript. Os usuários precisam apenas de um navegador web como o Chrome para executar o GAN Lab. Nossa abordagem de implementação amplia significativamente o acesso das pessoas a ferramentas interativas de aprendizado profundo.

![Captura de tela do GAN Lab](ganlab-teaser.png)


## Demonstração Funcional

Clique no seguinte link:

[https://poloclub.github.io/ganlab/](https://poloclub.github.io/ganlab/)

Funciona na maioria dos navegadores web modernos. Sugerimos o uso do Google Chrome.


## Desenvolvimento

Esta seção descreve como você pode desenvolver o GAN Lab.

### Instalar Dependências

Execute os seguintes comandos: 

```bash
$ git clone https://github.com/poloclub/ganlab.git
$ cd ganlab
$ yarn prep
```

Embora seja improvável, pode ser necessário instalar algumas dependências básicas relacionadas a JavaScript (por exemplo, yarn).


### Executando Sua Demonstração

Execute o seguinte comando:

```bash
$ ./scripts/watch-demo

>> Waiting for initial compile...
>> 3462522 bytes written to demo/bundle.js (2.17 seconds) at 00:00:00
>> Starting up http-server, serving ./
>> Available on:
>>   http://127.0.0.1:8080
>> Hit CTRL-C to stop the server
```

Em seguida, acesse `http://localhost:8080/demo/`. 

O script `watch-demo` monitora alterações no código TypeScript (por exemplo, `demo/ganlab.ts`)
e compila o código para você.


## Créditos

O GAN Lab foi criado por 
[Minsuk Kahng](https://minsuk.com),
[Nikhil Thorat](https://nikubaba.com),
[Polo Chau](https://poloclub.github.io/polochau/),
[Fernanda Viégas](http://www.fernandaviegas.com/) e 
[Martin Wattenberg](http://www.bewitched.com/),
sendo o resultado de uma colaboração de pesquisa entre a Georgia Tech e o Google Brain/[PAIR](https://pair.withgoogle.com).
Agradecemos também a Shan Carter e Daniel Smilkov, 
à [equipe Google Big Picture](https://research.google.com/bigpicture/) e ao 
[Google People + AI Research (PAIR)](https://pair.withgoogle.com), além do 
[Georgia Tech Visualization Lab](http://vis.gatech.edu/)
pelo feedback.
 
Para mais informações, confira 
[nosso artigo científico](http://minsuk.com/papers/kahng-ganlab-vis2018.pdf):     
 
[Minsuk Kahng](https://minsuk.com),
[Nikhil Thorat](https://nikubaba.com),
[Polo Chau](https://poloclub.github.io/polochau/),
[Fernanda Viégas](http://www.fernandaviegas.com/) e 
[Martin Wattenberg](http://www.bewitched.com/).
"GAN Lab: Understanding Complex Deep Generative Models using Interactive Visual Experimentation."
*IEEE Transactions on Visualization and Computer Graphics, 25(1) (VIS 2018)*, Jan. 2019.
[doi.org/10.1109/TVCG.2018.2864500](https://doi.org/10.1109/TVCG.2018.2864500)
