HTML semântico é uma abordagem que envolve usar elementos HTML específicos para o significado que representam na estrutura da página, ao invés de usar elementos genéricos para todos os propósitos. Isso não apenas melhora a acessibilidade, mas também a legibilidade e a interpretação do conteúdo por buscadores e outros serviços.

### Por que devemos usar HTML semântico?

✔️ 1.  **Acessibilidade:** Usar HTML semântico melhora a acessibilidade do site, permitindo que tecnologias assistivas, como leitores de tela, naveguem e interpretem o conteúdo do site de maneira mais eficaz. Isso é crucial para usuários com deficiências visuais ou outras limitações.

✔️ 2. **Melhora na SEO (Search Engine Optimization):** Elementos semânticos ajudam os motores de busca a entender o contexto e a estrutura do conteúdo do site, o que pode melhorar o ranqueamento nas páginas de resultados de busca.

✔️ 3. **Facilidade de Manutenção:** Código com HTML semântico é mais fácil de ler e manter. Desenvolvedores podem entender rapidamente a estrutura e o propósito de cada parte do código, o que torna mais fácil a manutenção e futuras atualizações.

✔️ 4. **Compatibilidade entre Navegadores:** O uso de elementos semânticos garante uma melhor compatibilidade entre diferentes navegadores, ajudando a manter uma aparência consistente em diversas plataformas.

✔️ 5. **Melhor desempenho no carregamento da página:** Páginas estruturadas semanticamente tendem a ser mais leves e mais rápidas no carregamento, pois utilizam menos código e mais markup relevante.

### Exemplo de HTML Semântico

Vamos ver um exemplo simples que usa HTML semântico:

```html
<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemplo de HTML Semântico</title>
</head>
<body>

    <header> // cabeçario do documento 
        <nav> //navegação
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">Sobre</a></li>
                <li><a href="#services">Serviços</a></li>
            </ul>
        </nav>
    </header>
    
    <main> // Representa o conteúdo principal do documento. Deve ser único e central para o entendimento do documento.
    
        <article> // Define um componente independente do conteúdo que pode ser distribuído independentemente do restante do site, como um post de blog.
        
            <h1>Título do Artigo</h1>
            <p>Este é um exemplo de parágrafo em um artigo.</p>
            
            <section> // Define uma seção do documento em html  
                <h2>Subtítulo da Seção</h2>
                <p>Conteúdo da seção do artigo.</p>
            </section>
            
        </article>
        
    </main>
    
    <footer> // rodape dos documentos 
        <p>Direitos autorais © 2024. Todos os direitos reservados.</p>
    </footer>
    
</body>
</html>
```


HTML SEMANTICO:
![[Pasted image 20240502142257.png]]

HTML NÃO SEMANTICO :
![[Pasted image 20240502142335.png]]
