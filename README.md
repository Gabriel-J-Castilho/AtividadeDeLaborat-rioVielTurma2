# AtividadeDeLaboratorioVielTurma2


#contraste e brilho
img_in = cv2.imread('t1.jpg',0)
#altere os valores tanto de a quanto de b

a = -1 
b = 1

img_out = a*img_in + b

img_out = np.array(img_out, dtype = np.uint8)

cv2_imshow(img_in)
cv2_imshow(img_out)

O conceito de morfologia na computação está principalmente relacionado ao processo de transformação de imagens por de transformações que são denominadas como transformações morfológicas.

Visto que todas as imagens geradas por computadores e tenham como base os pixels são na realidade um conjunto de matrizes trabalhando juntas para criar essas imagens, a um nível computacional, ou seja, relativo à programação, lógica e software que processa alguma imagem. As transformações morfológicas são transformações pautadas na lógica computacional por meio da manipulação seletiva das matrizes que geram as imagens. Por exemplo, a erosão, que é considerada um dos métodos básicos de transformação morfológica, utiliza uma lógica bem simples, a partir de dois inputs, chamados de imagem original e kernel, que eu particularmente prefiro chamar de molde. Há uma comparação entre esses dois inputs, e se as mesmas posições do molde não estiverem de acordo na imagem original, essas posições são “erodidas” ou apagadas. Por exemplo, se a posição 50 da imagem original for igual a 1,  e todos os pixels abaixo do kernel, ou molde, for diferente de 1, na imagem final ou produto morfológico,  a posição 50 será igual a 0. Ocorrendo assim a perda de um pixel, nesse caso. O mesmo processo sendo aplicado a todas as posições e comparando as duas imagens de entrada representam esse processo morfológico que chamamos de “erosão”.

Um processo similar ocorre para outros morfológicos, por exemplo a dilatação é basicamente o oposto da erosão. Ocorrendo um ganho de pixels no produto final se qualquer um dos pixels abaixo do kernel for igual a 1. 

A erosão e a dilatação, apesar de serem as formas consideradas mais básicas da morfologia computacional, representam a base das transformações morfológicas, sendo a maioria das outras transformações morfológicas variantes dos processos de erosão e dilatação, em alguns casos inclusive fazendo uso das duas em conjunto.
Então, os processos de morfologia são processos que fazem grande uso da lógica, mais especificamente da lógica booleana, e de operadores lógicos para tornar tudo isso possível. Além disso, a aplicabilidade da morfologia é muito grande, sendo algo muito utilizado por exemplo em filtros de imagens, mudanças de resolução, e até mesmo construção de imagens propriamente ditas. 




