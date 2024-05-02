Hyperlinks, ou simplesmente "links", são elementos fundamentais da web, permitindo a navegação entre páginas, documentos ou outras destinações na internet.

Eles são definidos usando a tag `<a>` em HTML.

Aceita qualquer tipo de conteudo 

Vamos explorar os principais atributos desta tag e como eles são utilizados para criar diferentes tipos de links.


## Atributos da Tag `<a>`

#### Atributos Globais

Todos os elementos HTML, incluindo a tag `<a>`, podem receber atributos globais que incluem `id`, `class`, `style`, `title`, entre outros. Esses atributos são usados para adicionar identificação, classes para estilização via CSS, ou diretivas de estilo inline.

#### Atributo `href`

O atributo `href` (Hypertext REFerence) especifica a URL (Uniform Resource Locator) para onde o link aponta. Este é o atributo mais importante de um hyperlink, pois define seu destino. Ele pode ser usado de várias formas:

- **URL Absoluta:** Caminho completo para um recurso na internet. Ex.: `href="https://www.example.com"`.
  
- **URL Relativa:** Caminho relativo ao próprio site. Ex.: `href="/about"`.
  
- **Fragmento:** Link para um fragmento específico da mesma página ou de outra. Ex.: `href="#section2"`.
  
- **E-mail:** Inicia um cliente de e-mail para enviar um e-mail. Ex.: `href="mailto:example@example.com"`.
  
- **Telefone:** Inicia uma chamada de telefone em dispositivos compatíveis. Ex.: `href="tel:+1234567890"`.

#### Atributo `download`

Este atributo instrui o navegador a baixar o recurso apontado pelo `href` ao invés de navegar até ele. Se o atributo `download` é especificado sem valor, o nome do arquivo será o último segmento do caminho do `href`. Pode ser dado um valor para especificar o nome do arquivo baixado.

#### Atributo `target`

Define como o navegador deve abrir o link. Os valores comuns incluem:

- **`_self`:** Abre o documento no mesmo contexto/frame que o link foi clicado (comportamento padrão).
  
- **`_blank`:** Abre o documento em uma nova aba ou janela.
  
- **`_parent`:** Abre o documento no contexto pai.
  
- **`_top`:** Abre o documento no topo do conjunto de contextos de navegação.

### Exemplo de Código HTML com Hyperlinks

```html

	<a href="https://www.example.com" target="_blank">Visite nosso site</a>
	<a href="mailto:support@example.com">Envie um e-mail</a>
	<a href="tel:+1234567890">Ligue para nós</a>
	<a href="/docs/tutorial.pdf" download="Tutorial.pdf">Baixe o Tutorial</a>
	<a href="#top">Volte ao topo</a>
	
```


Este exemplo demonstra vários usos de hyperlinks em HTML, aplicando os atributos discutidos para criar links para websites, e-mails, telefones, downloads de arquivos e navegação interna.