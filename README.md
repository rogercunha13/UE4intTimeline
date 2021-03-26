# UNREAL ENGINE 4 - BLUEPRINTS INTERMEDIÁRIO

## CONTROLE DA LUZ USANDO TIMELINE

## TIMELINE

Os nós da linha de tempo são nós especiais dentro de Blueprints que permitem que uma animação simples baseada em tempo seja projetada e reproduzida rapidamente com base em eventos no jogo. As linhas do tempo são como sequências de matinê simples, pois permitem que valores simples sejam animados e que eventos sejam disparados ao longo do tempo. Eles podem ser editados diretamente dentro do editor Blueprint clicando duas vezes na Linha de tempo na guia Gráfico ou na guia Meu Blueprint. Eles são especificamente construídos para lidar com tarefas simples e não cinematográficas, como abrir portas, alterar luzes ou executar outras manipulações centradas no tempo para atores em uma cena.

## UTILIZANDO A TIMELINE

Para isso, foi criado uma Blueprint tipo Actor para o controle da luz (componente point light):
![Imagem_BP_Controledaluz](Imagens/Imagem_BP_Controledaluz.jpg)

- Criado uma **Variável** do tipo **PointLight** com o nome de "ReferenceLuz" para que o objeto BP_ControledaLuz tenha referência do PointLight inserido no Level.

- Inserido o Actor (BP_ControledaLuz) no level:

![Imagem_Actor_noLevel](Imagens/Imagem_Actor_noLevel.jpg)

Realizar a referência (conhcecimento da PointLight) ao BP_ControledaLuz;

![Imagem_Referencia_Luz](Imagens/Imagem_Referencia_Luz.jpg)

No Event Graph do **BP_ControledaLuz**:

- Adicionar uma Timeline:
  - AddTimeline; ![Imagem_AddTimeLine](Imagens/Imagem_AddTimeLine.jpg)


Inserir o nome da TimeLine e em seguida clicar duas vezes em cima da TimeLine:

  ![Imagem_Timeline](Imagens/Imagem_Timeline.JPG)


Após clicar na TimeLine:

- Adicionar uma ColorTrack:

![Imagem_ColorTrack](Imagens/Imagem_ColorTrack.JPG)

Adicionar os pontos de tempo no Color:

![Imagem_PontosTempos_Color](Imagens/Imagem_PontosTempos_Color.jpg)

Em cada Ponto, é realizado a escolha da cor desejada:

![Imagem_escolherCor](Imagens/Imagem_escolherCor.jpg)

Ao clicar duas vezes em cada ponto, poderá escolher a cor desejada do tempo determinado:

![Imagem_EsolhendoaCor_ColorTrack](Imagens/Imagem_EsolhendoaCor_ColorTrack.jpg)

Após a configuração das cores, realizar
