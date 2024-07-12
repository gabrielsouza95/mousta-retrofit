# Retrofit das Moustas
Contém um resumo do projeto de retrofit para as moustas do FabLab CITeBauru

## CNC
De acordo com o [dicionário Collins](https://www.collinsdictionary.com/dictionary/english/cnc) CNC, em tradução livre, é "Controle Numérico Computacional" que é um meio de controlar como máquinas operam, utilizando um computador ou um microcontrolador(MCU). Então, impressoras, plotters, impressoras 3D, cortadoras laser, são todas máquinas que utilizam CNC para transformar arquivos gerados pelos usuários em um resultado físico.

Pra isso, geralmente é associado uma [MCU](https://www2.decom.ufop.br/imobilis/iot-cpu-vs-mcu-vs-soc-vs-fpga/) com, geralmente, interfaces de potências para controlar os [atuadores](https://www.feis.unesp.br/Home/departamentos/engenhariaeletrica/aula-5---sensor-25-04-2013b.pdf) que vão gerar alguma coisa no mundo material, como um motor que gera algum movimento, que empurram plástico ou que aquecem o hot-end, como acontece nas impressoras.

## Problema das Moustas
As impressoras, apesar de boas, as 3 Moustas estão com problema que, no ponto que chegou, já não vale ficar fazendo manutenção comum, pois vai ficar dando problema, ainda mais com a utilização do público que não tem tanto conhecimento específico. Então, para deixa-las preparadas para o público em geral poder utilizar e ainda por cima ficar 100% manutenível, seria interessante fazer um retrofit nelas, assim elas podem rodar muito tempo sem ficar parando para manutenção, em pé de igualdade com as Sethi3D.

## O projeto
Então, para um retrofit nas moustas, seria interessante trocar o firmware para o [Marlin](https://marlinfw.org/) e para ficar possível retornar, pegar um [kit ramps](https://pt.aliexpress.com/item/32966993463.html?gatewayAdapt=glo2bra), já garantindo todas as funcionalidades.

Para melhorar a confiabilidade da extrusora, seria interessante a troca para um [kit de extrusora direta](https://multipecascuritiba.com.br/produto/kit-extrusora-completa-mk8-e3d/) dado que atualmente ela utiliza extrusora bowden, que, apesar de boa, para o manuseio por parte de várias pessoas com níveis de conhecimento variados, a extrusora direta garante funcionamento por mais tempo sem precisar parar para manutenção por ter entupido por um manuseio incorreto (que é totalmente normal e esperado em máquinas para uso da comunidade). Essa troca, além de trocar o tipo de extrusão, já viria com o mesmo modelo de bico das Sethi3D, assim padronizando as máquinas do laboratório e facilitando a manutenção.

Um aspecto das Moustas que seria de grande valor fazer um upgrade seria a troca dos fusos comuns, que utilizam castanhas de latão. Uma delas, por exemplo, está com problema na rosca de uma das castanhas, que faz a mesa "pular" após algumas camadas e avanço do eixo Z. Uma forma de resolver seria a utilização de [fusos e castanhas trapezoidais](https://multipecascuritiba.com.br/produto/fuso-trapezoidal-tr8-passo-8mm-330mm-com-castanha/) que dariam, praticamente, vida infinita pra essa parte, não sendo mais um incômodo para nós.

Para a realização do projeto, contando o tempo e esforço que vou precisar investir, acredito que consigo fazer por 80R$H e, apesar de já ter alguma experiência na área, como nunca fiz um retrofit desses e vai ser necessário uma engenharia reversa para poder comprar um kit ramps mais simples sem a tela LCD, aproveitando o já existente, não sei dizer quanto tempo seria necessário, mas acredito que pelo menos umas 30H investidas em cada Mousta que, com umas 2 à 6H semanais investidas, daria para terminar o projeto em uns 3~4 meses, sem contar imprevistos que aconteçam no meio do caminho.

### Lista de materiais
- 1x [Kit ramps](https://pt.aliexpress.com/item/32966993463.html?gatewayAdapt=glo2bra)
- 1x [Kit extrusora direta](https://multipecascuritiba.com.br/produto/kit-extrusora-completa-mk8-e3d/)
- 1x [Kit fuso trapeozoidal com castanha](https://multipecascuritiba.com.br/produto/fuso-trapezoidal-tr8-passo-8mm-330mm-com-castanha/)

## Para Futuros upgrades
Com os upgrades mencionados, as Moustas já ficam prontas para ficarem funcionando por um bom tempo sem precisar ficar parando para manutenção, mas, ainda assim, alguns pontos, como as peças estruturais de ABS ainda seriam um elo fraco, que poderiam falhar com o passar dos anos, então, seria interessante fazermos engenharia reversa das peças e replica-las em alumínio. Para isso, poderiamos utilizar a CNC de 4 eixos que se encontra parada, precisando de broca, mas que uma vez funcionando, poderiamos, com a compra de alguns tarugos de alumínio, refazer a Mousta toda em peças de alumínio e, ai sim, ficariam indestrutíveis. Inclusive, poderiamos vender as peças e como serviço de upgrade de Moustas também, já fazendo uma geral nas Moustas que estão com outros grupos pela Unesp primeiramente.

## Referências
- 1: https://www.collinsdictionary.com/dictionary/english/cnc
- 2: https://www2.decom.ufop.br/imobilis/iot-cpu-vs-mcu-vs-soc-vs-fpga/
- 3: https://www.feis.unesp.br/Home/departamentos/engenhariaeletrica/aula-5---sensor-25-04-2013b.pdf
- 4: https://marlinfw.org/
- 5: https://pt.aliexpress.com/item/32966993463.html?gatewayAdapt=glo2bra
- 6: https://multipecascuritiba.com.br/produto/kit-extrusora-completa-mk8-e3d/
- 7: https://multipecascuritiba.com.br/produto/fuso-trapezoidal-tr8-passo-8mm-330mm-com-castanha/
