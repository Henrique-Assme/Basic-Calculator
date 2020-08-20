# Basic-Calculator
This project is for my school discipline "programming of mobile devices", where I have to make a simple program and make a tutorial on how to create it.

# Primeiros passos
Primeiro, crie um novo projeto no Android Studio. Selecione a Empty Activity, de um nome ao seu projeto e selecione a linguagem Java.

Selecione os botões (Button) e as duas caixas de texto pra digitar os números (Number)

![Botões](https://user-images.githubusercontent.com/69920692/90811849-b768f880-e2fb-11ea-9e3f-31766dae82ea.PNG)
![Numeros](https://user-images.githubusercontent.com/69920692/90811859-b9cb5280-e2fb-11ea-88c5-d6498995a249.PNG)

Nesse caso, faremos uma calculadora com soma, subtração, multiplicação, divisão e um botão de limpar, utilizando 5 Buttons e 2 EditText de números. Personalize como quiser o seu layout e vamos continuar.

Na tela da direita, ligue os botões com a parte de cima da tela e vá ajustando como quiser. 
![Ajuste](https://user-images.githubusercontent.com/69920692/90813214-a28d6480-e2fd-11ea-9d99-2db2228f239c.PNG)

Basta clicar nessa bolinha e linkar com a bolinha do objeto de cima. Isso serve para, na hora de abrir o aplicativo, todos os os objetos não ficarem grudados na parte de cima da tela. Certifique-se de estar tudo ligado, direta ou indiretamente, ao topo da tela.

![Ajuste2](https://user-images.githubusercontent.com/69920692/90813541-20ea0680-e2fe-11ea-9043-26e7da42d3cd.PNG).

Agora vamos dar um id para cada botão e cada EditText. Sugiro colocar btnSomar, btnSubtrair, btnMultiplicar, btnDividir, btnLimpar, editTextNum1 e editTextNum2. Pode dar o nome que quiser, mas vou colocar esses nomes para ficar mais didático e sabermos o que é cada coisa. 
![Id](https://user-images.githubusercontent.com/69920692/90813871-948c1380-e2fe-11ea-8529-36ad71f231c4.PNG)

Vamos mudar também o texto que aparece nos botões, colocando +, -, *, / e Limpar. 
![Texto](https://user-images.githubusercontent.com/69920692/90814649-d073a880-e2ff-11ea-837e-4ffd58742165.PNG)

No fim, personalize seu layout como quiser.
![Layout](https://user-images.githubusercontent.com/69920692/90814814-0ca70900-e300-11ea-9716-da063eb7330e.PNG)

# Código

Declaramos as variáveis primeiro, atribuindo nomes para os editText e os Buttons. Além disso, criaremos 3 variávies do tipo Float e uma String que usaremos mais para frente.

![DeclararVariaveis](https://user-images.githubusercontent.com/69920692/90815204-b25a7800-e300-11ea-8c6b-67bdddab6dc6.PNG)

Dentro do método OnCreate, vamos dizer qual objeto do layout será atribuido para o que criamos acima. 
![OncreateVariaveis](https://user-images.githubusercontent.com/69920692/90815340-ee8dd880-e300-11ea-8452-e8b3a076e6be.PNG)

Criamos agora o método de OnClick para o botão somar. O if está verificando se os campos para digitar os números estão vazios. Caso um deles esteja, aparecerá um alerta para o usuário pedindo que ele digite um número para prosseguir. Caso os dois campos estejam preenchidos, o else servirá para a lógica de calcular a soma. Usamos as variáveis n1 e n2 para atribuir os valores digitados nos editText, atribuimos à variável result a soma n1+n2 e colocamos na variável message o valor de result convertido para string. Por fim, o Toast serve para fazer um Pop-up na tela, mostrando o resultado da soma.
![Somar](https://user-images.githubusercontent.com/69920692/90815873-c18df580-e301-11ea-9257-3c8a322bdd35.PNG)

Agora basta fazer o mesmo procedimento para os outros 3 botões, com um detalhe extra no botão dividir. Após atribuir os valores para n1 e n2, temos um if para verificar se o n2 é igual a 0, uma vez que sabemos que divisão por zero é indeterminado. 

![Operações](https://user-images.githubusercontent.com/69920692/90816027-fac66580-e301-11ea-8c3f-63b5cf1098fe.PNG)

Para finalizar, falta o botão de limpar que, ao ser clicado, limpará os números digitados para o usuário poder colocar outros números.

![Limpar](https://user-images.githubusercontent.com/69920692/90816228-50027700-e302-11ea-9e81-02f8981194c6.PNG)

# Testando

Agora que a calculadora está devidamente programada, basta testar e ver se tudo esá funcionando como deveria. Uma dica é tentar chamar alguem de fora para testar, pois os usuários são ótimos em achar falhas.
