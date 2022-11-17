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

# O código acima é um código que tem como finalidade a mudança de contraste e brilho da imagem inicial inserida pelo professor.
Explicando linha por linha o funcionamento do código temos que:

1 - img_in = cv2.imread('t1.jpg',0) 
#Primeiro temos uma leitura e um salvamento de imagem. O caso cv2.imread('t1.jpg',0) que é uma leitura literal da imagem a partir dos arquivos disponíveis no computador. E o caso img_in = cv2.imread... que é responsável por salvar os dados da imagem lida pelo programa dentro da variável img_in para utilização posterior.

2 - a = -1
    b =  1
#São declarações dos valores das variáveis a e b. Que nesse caso foram declaradas dessa forma para facilitar qualquer mudança desejada pelo programador tanto no contraste quanto no brilho da imagem, facilitando bastante o processo de manipulação do estado final da imagem.
    
3 - img_out = a*img_in + b
# Neste caso temos a declaração de que img_out é igual a a*img_in+b. Ou seja, aqui há a primeira manipulação propriamente dita da imagem inicial, usando o valor a e b para fazer essa manipulação. No caso aqui há uma manipulação parcial, que só é completada com o comando de número 4.

4 - img_out = np.array(img_out, dtype = np.uint8)
# "np.array é o carray utilizando a biblioteca numpy, que neste caso é abreviada como "np" por fins de facilidade de digitação e manipulação, porque "np" é muito mais fácil de se manipular do que "numpy". 












O conceito de morfologia na computação está principalmente relacionado ao processo de transformação de imagens por de transformações que são denominadas como transformações morfológicas.

Visto que todas as imagens geradas por computadores e tenham como base os pixels são na realidade um conjunto de matrizes trabalhando juntas para criar essas imagens, a um nível computacional, ou seja, relativo à programação, lógica e software que processa alguma imagem. As transformações morfológicas são transformações pautadas na lógica computacional por meio da manipulação seletiva das matrizes que geram as imagens. Por exemplo, a erosão, que é considerada um dos métodos básicos de transformação morfológica, utiliza uma lógica bem simples, a partir de dois inputs, chamados de imagem original e kernel, que eu particularmente prefiro chamar de molde. Há uma comparação entre esses dois inputs, e se as mesmas posições do molde não estiverem de acordo na imagem original, essas posições são “erodidas” ou apagadas. Por exemplo, se a posição 50 da imagem original for igual a 1,  e todos os pixels abaixo do kernel, ou molde, for diferente de 1, na imagem final ou produto morfológico,  a posição 50 será igual a 0. Ocorrendo assim a perda de um pixel, nesse caso. O mesmo processo sendo aplicado a todas as posições e comparando as duas imagens de entrada representam esse processo morfológico que chamamos de “erosão”.

Um processo similar ocorre para outros morfológicos, por exemplo a dilatação é basicamente o oposto da erosão. Ocorrendo um ganho de pixels no produto final se qualquer um dos pixels abaixo do kernel for igual a 1. 

A erosão e a dilatação, apesar de serem as formas consideradas mais básicas da morfologia computacional, representam a base das transformações morfológicas, sendo a maioria das outras transformações morfológicas variantes dos processos de erosão e dilatação, em alguns casos inclusive fazendo uso das duas em conjunto.
Então, os processos de morfologia são processos que fazem grande uso da lógica, mais especificamente da lógica booleana, e de operadores lógicos para tornar tudo isso possível. Além disso, a aplicabilidade da morfologia é muito grande, sendo algo muito utilizado por exemplo em filtros de imagens, mudanças de resolução, e até mesmo construção de imagens propriamente ditas. 




