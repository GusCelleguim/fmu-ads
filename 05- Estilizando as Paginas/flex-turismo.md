Me explique como funciona cada parde desse codigo e crie comentarios em linhas que vc achar importante explicar 

```html

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex Turismos</title>
    <link rel="stylesheet" href="./style.css">
</head>
<body>
    <header>
        <div class="flex-container menu">
            <div><h1>FlexTurismos</h1></div>
            <ul class="list-items">
                <li><a href="#quem-somos">Quem somos</a></li>
                <li><a href="#servicos">Serviços</a></li>
                <li><a href="#planos">Planos</a></li>
        </div>
            </ul>
    </header>

    <div class="flex-container apresentação">
        <div class="texto-apresentação">
            <h1>Flex <br>Turismos</h1>
            <p>O melhor serviço para você!</p>
            <a href="" class="btn">Saiba Mais!</a>
        </div>

        <div>
            <div><img src="./images/0-main.png" alt="banner de apresentação"></div>
        </div>
    </div>

    <div class="flex-container apresentação" id="quem-somos">
        <div>
            <h2>Quem somos</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur, corrupti!</p>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quos, officia magnam numquam optio expedita possimus aliquid facere. Enim, tenetur laboriosam animi temporibus blanditiis aliquid sint cum quibusdam reiciendis alias eaque!</p>
        </div>
        <div>
            <div><img src="./images/1-quem-somos.png" alt="balcão de atendimento"></div>
        </div>
    </div>

    <div class="container-externo">
        <div class="flex-container" id="serviços">
            <div>
                <h2>Serviços</h2>
            </div>

            <div class="lista-serviços">
                <div class="item-serviço">
                    <div><img src="./images/icon-2.png" alt="hospedagens"></div>
                    <p>Hospedagens</p>
                    <a href="#">Comprar Agora</a>
                </div>

                <div class="item-serviço">
                <div><img src="./images/icon-1.png" alt="pacote de viagens"></div>
                <p>Pacotes de viagens</p>
                <a href="#">Comprar Agora</a>
                </div>

                <div class="item-serviço">
                    <div><img src="./images/icon-3.png" alt="roteiros personalizados"></div>
                    <p>Roteiros personalizados</p>
                    <a href="#">Comprar Agora</a>
                </div>
            </div>
        </div>
    </div>

    <div class="flex-container" id="planos">
        <div><h2>Planos</h2></div>

        <div class="list-planos">
            <div class="item-plano">
                <h3>Plano 1</h3>
                <hr>
                <ul>
                    <li>Suporte 24h</li>
                    <li>Serviços de quarto</li>
                    <li>Guia turístico</li>
                </ul>
                <a href="#" class="btn">Saiba Mais!</a>
            </div>
    
            <div class="item-plano">
                <h3>Plano 2</h3>
                <hr>
                <ul>
                    <li>Suporte 24h</li>
                    <li>Serviços de quarto</li>
                    <li>Guia turístico</li>
                    <li>Roteiro de trilhas</li>
                    <li>Serviço personalizado</li>
                </ul>
                <a href="#" class="btn">Saiba Mais!</a>
            </div>
    
            <div class="item-plano">
                <h3>Plano 3</h3>
                <hr>
                <ul>
                    <li>Suporte 24h</li>
                    <li>Serviços de quarto</li>
                    <li>Guia turístico</li>
                    <li>Roteiro de trilhas</li>
                    <li>Serviço personalizado</li>
                    <li>Área Vip</li>
                </ul>
                <a href="#" class="btn">Saiba Mais!</a>
            </div>
        </div>
    </div>

    <footer>
        <div class="flex-container">
            <p>&copy; 2021 CSS
            <p>Desenvolvido por: Bryan Patucci</p>
        </div>
    </footer>
</body>
</html>



```


```CSS

*{

margin: 0;
padding: 0;
font-family: arial;
}

  

ul{
list-style: none; /* Remove os marcadores de lista */
margin: 0;
padding: 0;
}

  

ul li a{
text-decoration: none; /* Remove o sublinhado dos links */ 
color: white; /* Define a cor do texto dos links como branco */
}

  

div img{
display: block; /* Faz a imagem se comportar como um bloco, quebrando a linha */ width: 100%; /* Ajusta a largura da imagem para ocupar 100% do seu contêiner */
}

.flex-container { display: flex; 
/* Define o display para flex, permitindo layout flexível */ 
max-width: 992px; /* Largura máxima do contêiner */ 
margin: auto; /* Centraliza o contêiner na página */ 
width: 100%; /* A largura é ajustada para ocupar 100% */ 
min-width: 320px; /* Largura mínima do contêiner */ 
}

  

header{
height: 100px; color: white;
/* Define a cor do texto do cabeçalho como branco */
background-color: #122a57; /* Cor de fundo do cabeçalho */
display: flex; align-items: center; /* Alinha verticalmente os itens ao centro */
}

  

header .list-items{
display: flex; width: 100%; max-width: 260px; 
justify-content: space-between; 
/* Distribui o espaço igualmente entre os itens da lista */ 
align-items: center;
}

  

header .menu{
justify-content: space-between;
}

  

.apresenta{

height: 80vh; /* Altura baseada em 80% da altura da viewport */
align-items: center; justify-content: space-between; /* Espaçamento entre os elementos filhos */

}

  

.apresenta .texto-apresenta p{
font-weight: bold; /* Texto em negrito */
font-size: 20px; /* Tamanho da fonte */
}

  

.apresenta .texto-apresenta{;
min-height: 200px; /* Altura mínima do contêiner */ 
width: 100%
}

  

.texto-apresenta h1{

color: #122a57;

font-size: 48px;

margin-bottom: 10px;

}

  

.btn{

background-color: #122a57; /* Cor de fundo do botão */ color: white; text-align: center; border-radius: 30px; /* Bordas arredondadas */ width: 220px; /* Largura do botão */ display: block; text-decoration: none; height: 50px; /* Altura do botão */ line-height: 50px; /* Altura da linha igual à altura do botão, centralizando o texto verticalmente */ margin-top: 20px; /* Margem acima do botão */

}

  

#quem-somos{

height: 50vh;

align-items: center;

justify-content: space-between;

}

  

#quem-somos h2{

font-size: 32px;

color: #122a57;

display: flex;

}

  

#quem-somos h2::before{

content: "";

height: 40px;

width: 5px;

margin-right: 5px;

background-color:#122a57;

position: relative;

margin-bottom: 20px;

}

  

#quem-somos p{

margin-bottom: 10px;

width: 90%;

}

  

#quem-somos img{

min-width: 470px;

}

  

.container-externo{

background-color:#122a57;

width: 100%;

}

  

#serviços{

flex-direction: column;

padding: 50px 0 80px 0;

}

  

#serviços h2{

color: white;

font-size: 32px;

margin-bottom: 20px;

}

  

.lista-serviços{

display: flex;

justify-content: space-between;

}

  

.lista-serviços .item-serviço{

text-align: center;

}

  

.item-serviço a{

width: 220px;

background-color: white;

border-radius: 30px;

height: 50px;

text-align: center;

line-height:50px;

text-decoration: none;

margin-top: 30px;

color:#122a57;

padding: 10px 15px;

font-weight: bolder;

}

  

.item-serviço p{

margin-top: 20px;

font-weight: bold;

font-size: 18px;

color: white;

}

  

.item-serviço img{

width: 80%;

margin: auto;

}

  

#planos{

flex-direction: column;

min-height: 100vh;

}

  

#planos h2{

font-size: 32px;

padding-top: 50px;

  

}

  

.list-planos{

display: flex;

align-items: flex-end;

justify-content: space-between;

}

  

.item-plano{

padding: 10px;

flex: 1;

border: 5px solid #122a57;

margin-right: 20px;

max-width: 240px;

}

  

.item-plano .btn{

margin: auto;

margin-bottom: 20px;

}

  

.item-plano h3{

margin-top: 10px;

text-align: center;

font-size: 24px;

display: flex;

flex-direction: column;

}

  

hr{

margin: auto;

margin-top: 10px;

margin-bottom: 10px;

align-items: center;

width: 80%;

height: 2px;

background-color: #122a57;

}

  

.item-plano ul{

margin-bottom: 10px;

margin-left: 30px;

list-style:disc;

padding: 10px 20px;

display: flex;

flex-direction: column;

}

  

footer{

height: 70px;

background-color: #122a57;

display: flex;

align-items: center;

}

  

footer .flex-container{

justify-content: space-between;

color: white;

}

  

/*mobile */

  

@media(max-width: 992px){

.flex-container{

flex-direction: column;

}

  

.apresentação{

flex-direction: column-reverse;

}

  

.apresentação .texto-apresentação{

margin: auto;

width: 100%;

}

  

#quem-somos{

flex-direction: column-reverse;

}

  

#quem-somos img{

visibility: hidden;

}

  

.lista-serviços{

flex-direction: column;

}

  

.item-serviço img{

width: 50%;

margin: auto;

}

  

.list-planos{

flex-direction: column;

align-items: flex-start;

margin-bottom: 20px;

}

  

.list-planos .item-plano{

max-width: 90%;

margin: auto;

width: 100%;

margin-bottom: 20px;

}

}
```