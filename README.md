
# Reconhecimento Facial e transformação de imagens em Dados no Azure ML

Neste Artigo, vou mostrar um pouco de como foi usar o Azure AI Visio Studio para fazer reconhecimento facial, extração de texto e tambem o recurso de legendas em imagem, muito util quando falamos sobre acessibilidade. Espero que esse passo a passo te ajude a tambem utilizar esses recursos incriveis.

## Primeiros passos
Antes de utilizar os recursos, é necessario criar um grupo de recursos no [Portal azure](https://portal.azure.com/). Caso ainda não tenha uma conta no Azure, voce precisa criar em [ml.azure.com](https://ml.azure.com/)

Selecione a opção **Criar um recurso**
![Selecionando a opção de criar um recurso](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/criando%20recurso.png)

Em categorias, selecione **IA + Machine learning**, e após isso na opção **Serviços cognitivos**, clique em criar 
![Criando recurso de visão computacional](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/recurso%20de%20vis%C3%A3o%20computacional.png)

Preencha essas configurações
![](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/configura%C3%A7%C3%B5es.png)

Mais abaixo voce vera essa opção de tipo de preço, nela selecione **Standard SO**, e abaixo marque a caixa de que leu e compreendeu os termos, e em seguida clique em **examinar + criar**.
![](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/tipo%20de%20pre%C3%A7o.png)

# Portal Azure AI Vision Studio
Antes de começar, é necessario algumas configurações no portal Azure AI Vision Studio.

Dentro do [Portal Azure AI Vision Studio](https://portal.vision.cognitive.azure.com/), vá na opção **View all resources**, e marque o recurso que voce criou anteriormente, e clique em **Select as default resource**. Após clicar, nada acontecera na tela, e é isso mesmo que deve ocorrer, e então clique no **X** no canto superior direito.
![](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/ver%20recursos.png)

![](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/deixando%20recurso%20como%20padr%C3%A3o.png)



# Detecção de rosto
No [Portal Azure AI Vision Studio](https://portal.vision.cognitive.azure.com/), o primeiro recurso que usei foi o detecção de rosto.

Selecione a opção **Face** no portal e em seguida a **Detect faces in an image**
![](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/menu%20face.png)
![](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/recurso%20detec%C3%A7%C3%A3o%20facial.png)

Feito isso, voce vai ter opções de imagens próprias do site ou de usar imagens salvas na sua galeria.
![Tela de uso do recurso de deteção de rosto do portal Azure AI Vision Studio](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/usando%20recurso%20detec%C3%A7%C3%A3o%20facial.png)
![Foto com uma imagem do rosto](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/inputs/foto%20perfil.jpg)
![Recurso analisando a imagem](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/outputs/resultado%20detec%C3%A7%C3%A3o%20de%20rosto%20foto%20perfil.png)
![Recurso mostrando que identificou que havia um rosto na imagem](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/outputs/rosto%20detectado.png)
![Foto com 4 pessoas](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/inputs/WhatsApp%20Image%202024-03-30%20at%2012.48.43%20(1).jpeg)
![Recurso mostrando que identificou 4 rostos na foto](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/outputs/resulatado%20de%20detec%C3%A7%C3%A3o%20facil%20multipla.png)

# Extração de texto de imagens
O próximo recurso utilizado foi o de extração de texto de imagens, é um recurso como se fosse um scanner vamos dizer assim, onde voce coloca uma imagem e ele busca extrair o texto dela, seja um arquivo impresso ou até mesmo escrito a mão.

Para utilizar esse recurso no portal, vá no menu **Optical character recognition**, e em seguida em **Extract text from images**
![](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/ocr.png)
![](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/extra%C3%A7%C3%A3o%20de%20texto%20de%20imagens.png)

Nessa opção voce tambem pode usar imagens de exemplo do próprio portal ou da sua galeria.
![Usando o OCR](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/usando%20o%20ocr.png)
![Recurso extraindo texto de uma imagem](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/outputs/resultado%20de%20extra%C3%A7%C3%A3o%20de%20texto.png)


# Recurso de legenda para imagens
o ultimo recurso utilizado foi de geração de legendas para imagens, um recurso muito legal para questões de acessibilidade, pois funciona como um texto alternativo para imagens, onde o recurso analisa a imagem e gera uma legenda de descrição sobre ela.

Para usar esse recurso, vá no menu **Image analysis**, e em seguida em **Add captions to images**
![](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/recurso%20de%20adicionar%20legendas%20em%20imagem.png)

Assim como nos outros recursos, voce pode usar imagens de exemplo do portal ou da galeria
![Imagem de um Tigre branco em uma floresta](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/outputs/usando%20recurso%20de%20legenda%20em%20imagem.png)
![Foto de duas crianças em uma praça próximos a uma árvore](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/outputs/recurso%20de%20legenda%20em%20foto.png)


# Excluindo grupo de recurso
Pode paracer algo sem importancia, mas é recomendado que após não utilizar mais os recursos, voce excluir o grupo de recursos, para que o mesmo não consuma créditos da sua conta ou até mesmo gere gastos, caso voce não esteja mais no período gratuito de testes e ja tenha usado os 200 dólares concedidos ao criar uma conta nova. Então deixei aqui tambem um resumo de como excluir um grupo de recursos.

Para isso, no [Portal azure](https://portal.azure.com/), selecione o grupo de recursos que voce criou, e em seguida marque-o e clique em **Excluir o grupo de recursos**.
![](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/grupo%20de%20recursos.png)
![](https://github.com/henriquesoaresjr/Visao-Computacional-Com-AzureML/blob/main/prints-auxiliares/excluindo%20grupo%20de%20recursos.png)

# Conclusão
Essa foi uma atividade que me deu muita satisfação realizar, pois IA é algo que tenho muita vontade estudar, e ver tudo que ela é capaz de fazer é impressionante, e quero cada vez mais buscar conhecimento sobre isso, pois é algo que desperta meu interesse de conhecimento.
Deixo abaixo alguns links de referência caso alguem queira saber mais sobre tudo isso que foi feito nessa atividade descrita aqui neste repositório.

 - [Detecção de rosto no Visual Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html)
 - [Detecção de Texto em uma imagem no Visual Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html)
 - [Analise de imagem no Visual Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html)





