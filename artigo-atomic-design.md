#### Unoesc Chapecó
#### Pós-graduação em Desenvolvimento Web, Cloud e dispositivos móveis - WebMob
#### Disciplina: HTML5+CSS3
#### Professor: Jean Carlo Nascimento
#### Acadêmico(a): Rony Remus Peruzzo
### Artigo de revisão de Atomic Design

</br></br>

##### O que é?

  O Atomic Design é uma metodologia de desenvolvimento. Ou seja, um conjunto de práticas que auxiliam a criação de um projeto de sistemas de qualquer natureza, com uma coleção de regrinhas para facilitar, agilizar e organizar o trabalho de um designer ou desenvolvedor web.
  
##### Como funciona?

  A metodologia é baseada em 5 níveis hierárquicos, átomo, molécula, organismo, template e página. 
  
  ÁTOMO: Como o nome já sujere, são os menores elementos disponíveis na construção de um software. Os átomos são elementos isolados que não precisam de um contexto para existir. Pense em coisas soltas como labels, inputs, campos de formulário, botões, títulos, parágrafo, etc. Estes são os blocos básicos utilizados para construir elementos maiores.
  Exemplo: 
  
```html
<html>
<head>
  <title>Exemplo de átomos</title>
</head>
<body>
  <label for="nome" class="atomo-label" >Label é um átomo</label>
  <input type="text" class="atomo-input" name="email" value="input tb é um átomo">
  <input type=”button” class="atomo-button" value="Tb é um átomo"/>
</body>
</html>
```
```css
.atomo-label {
    min-width: 120px;
    display: inline-block;
    position:absolute;
    left:19px;
    margin-right:5px;
  }

.atomo-input {
  width: 300px;
  background-color:#f1ff00;
  position:absolute;
  left:95px;
  top:23px;
  width:225px;
}

.atomo-button {
    width: 300px;
    display: inline-block;
    float: left;
    border-style:dashed;
    position:absolute;
    bottom: 0.5em;
    right:10px;
    background-color:#f1ff00;
  }
```
 
  MOLÉCULA: Na ciência, o conceito de molécula é basicamente agrupamentos de dois ou mais átomos. Esse conceito pode ser usado perfeitamente na metodologia, onde podemos juntar os componentes (átomos) criando uma espécie de molécula com um propósito único. Por exemplo um label um campo de formulário e um botão não são uteis isoladamente, mas juntos podem cumprir uma função específica como realizar uma busca.
  Exemplo:
```html
<html>
<head>
  <title>Exemplo de molécula</title>
</head>
<body>
  <form class="molecula-form" actiton="/beers">
   
    <div class="molecula-cpf">
      <label class="atomo-label">CPF:</label>
      <input type="text" class="atomo-input" name="cpf">
      <input type=”button” class="atom-button" value="Pesquisar"/>
    </div>
    
    <div class="molecula-cnpj">
      <label class="atomo-label">CNPJ:</label>
      <input type="text" class="atomo-input" name="CNPJ">
      <input type=”button” class="atom-button" value="Pesquisar"/>
    </div>

  </form>
</body>
</html>
```
```css
.molecula-cpf {
  width: 100px;
  margin: 0 auto;
}

.molecula-cnpj {
  width: 150px;
  margin: 0 auto;
}
```

  ORGANISMO: Da mesma maneira que uma molécula é um conjunto de átomos, organismos são um conjunto de moléculas que quando agrupados tornam-se elementos que norteiam a navegação e a leitura do conteúdo nessa interface.
  Normalmente isto vai corresponder a uma seção do site como header, footer, sidebar, etc. Ao contrário das moléculas, os organismos podem ter diversos propósitos funcionando paralelamente. Um header, por exemplo, pode possuir elementos como logotipo, navegação, formulário de login, campo de busca, etc. E cada um deles realiza uma ação específica. 
  Exemplo: 
```html
<html>
<head>
  <title>Exemplo de organismo</title>
</head>
<body>
  <form class="molecula-form" actiton="/beers">
    <article>
      <div class='organism-salvar-cpf-cnpj'>
        
        <div class="molecula-cpf">
          <label class="atomo-label">CPF:</label>
          <input type="text" class="atomo-input" name="cpf">
          <input type=”button” class="atom-button" value="Pesquisar"/>
        </div>
          
        <div class="molecula-cnpj">
          <label class="atomo-label">CNPJ:</label>
          <input type="text" class="atomo-input" name="CNPJ">
          <input type=”button” class="atom-button" value="Pesquisar"/>
        </div>
        
        <input type=”button” class="atom-button" value="Salvar"/>
        
      </div>
    </article>
  </form>
</body>
</html>
```
```css
  .organism-salvar-cpf-cnpj {
    width: 100%;
  }
```

  TEMPLATE: Na fase de modelo, nós quebramos nossa analogia química para entrar em uma linguagem que faz mais sentido para a nossa produção final. Templates consistem principalmente de grupos de organismos costurados juntos para formar páginas. É aqui que começamos a ver o projeto tornando as coisas mais concretas. O template é a forma de dar um contexto para todos as etapas anteriores. Agora seu cliente já começa a visualizar como o produto final ira ficar. </br> 
  Exemplo:</br>
   ![Novo Repositório no Github](https://github.com/bradfrost/atomic-design/blob/master/images/content/template.png)
  
  
  PÁGINA: As páginas são instâncias específicas de templates. Aqui, o espaço reservado e indicado no template é substituído por um conteúdo representativo real, para dar a descrição exata do que o usuário irá ver.
  Se os átomos são os menores elementos do sistema a página por sua vez é o mais alto nível do produto final, é ondet tipicamente a maioria das pessoas envolvidas no processo, passar a maior parte do seu tempo pois é a parte mais tangível do sistema. </br>
  Exemplo: </br>
  ![Novo Repositório no Github](https://github.com/bradfrost/atomic-design/blob/master/images/content/page.png)
  

##### Por que usá-lo, quais seus benefícios?

  Atomic Design pode nos fornecer uma metodologia clara para a elaboração de sistemas, onde clientes e membros da equipe de criação são capazes entender melhor e mais rapidamente o contexto da aplicação planejada. Com a metodologia podemos ir do abstrato (átomos) ao concreto (páginas) dando coerência e escalabilidade enquanto mostra simultaneamente as os resultados em seu contexto final. 
  Pensando na equipe de planejamento e construção a metodologia trás vanagens como padronização, modularização, organização e definições claras de códigos fontes e material design. Com isso o resposável pelo projeto pode revesar/alocar membros da equipe sem problemas de dependência e centralização do conhecimento.
  Já os membros do time de design e do time do cliente conseguem visualizar melhor o sistema, sem necessariamente precisar ver todos os layouts salvos em .jpg em frente a eles.
  
##### Onde usá-lo?
  A aplicação da metodologia Atomic Design pode ser aplicada em qualquer projeto, seja ele web ou não, pois o a idéia de organizar seus código pensando no re-uso dos componentes e funcionalidades e importante em qualquer circunstância, desde pequenas aplicações ou sites até grandes e elaborados projetos, que neste caso fica extremamente importante aplicar a metodologia, visando claro, facilitar a etapa de projeto e construção mas também pensando no futuro, onde o trabalho feito já não é mais um projeto e sim uma aplicação concreta e que já possa receber possiveis manutenções para se adaptar as mudanças do mercado.
  
  
##### Referências

http://www.linhadecodigo.com.br/artigo/3557/customizando-formularios-com-css.aspx </br>
http://webnerd.com.br/dev/atomic-design-uma-nova-visao-sobre-o-design-na-web/ </br>
http://www.felipefialho.com/blog/2014/falando-em-organizacao-css/ </br>
http://pt.slideshare.net/suissapg/atomic-design-28724858 </br>
http://nomadev.com.br/atomic-design-por-que-usar/ </br>
http://nomadev.com.br/atomic-design-com-angularjs/ </br>
https://www.phase2technology.com/blog/your-frontend-methodology-is-all-of-them-atomic-design-patternlab/ </br>
http://tableless.com.br/o-que-e-design-atomic/ </br>
https://github.com/suissa
https://github.com/bradfrost/atomic-design/

  
  
