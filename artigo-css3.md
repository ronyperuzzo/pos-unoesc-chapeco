#### Tarefa do artigo de CSS3
Seu artigo de revisão deverá abordar 10 funcionalidades de CSS3 que mais usa, que pesquisou, ou que achou interessante. Sobre cada uma dessas 10 funcionalidades, deverá apresentar o seguinte:
- Nome da funcionalidade;
- O que é ou o que faz a funcionalidade;
- Onde usar essa funcionalidade, em que contexto deve usar ela;
- Como usar essa funcionalidade, ou seja, sua sintaxe de utilização;
- Apresentar um exemplo de uso dessa funcionalidade.
- Referência de onde extraiu o conteúdo apresentado.

</br></br></br></br>
#### Unoesc Chapecó
#### Pós-graduação em Desenvolvimento Web, Cloud e dispositivos móveis - WebMob
#### Disciplina: HTML5+CSS3
#### Professor: Jean Carlo Nascimento
#### Acadêmico(a): Rony Remus Peruzzo
### Artigo de revisão de CSS3

##### Funcionalidade: border-radius
##### O que é?
A propriedade CSS3 border-radius destina-se a definir bordas arredondadas. O arredondamento das bordas é feito com declaração de dois valores CSS de medida; o primeiro define o eixo horizontal (rx) de 1/4 de uma elipse e o segundo o eixo vertical (ry). O quarto de elipse assim definida é convenientemente inserida no canto vivo do box arredondando-o. O diagrama a seguir esclarece o esquema de arredondamento.
##### Onde usar:
Em qualquer elemento que possui o atributo border.
##### Como usar:
```css
seletor {border-radius:
[ <length> | <percentage> ]{1,4} [ / [ <length> | <percentage> ]{1,4} ]?);
}
```
##### Exemplo de uso
A sintaxe geral para aplicar borda arredondada é mostrada a seguir.

```css
seletor {
  border-top-left-radius: rx ry;
  border-top-right-radius: rx ry;
  border-bottom-right-radius: rx ry;
  border-bottom-left-radius: rx ry;
}

```
##### Referencia:
[http://www.maujor.com/tutorial/interativo-css3/inc/borderradius.php](http://www.maujor.com/tutorial/interativo-css3/inc/borderradius.php)

##### Funcionalidade: Box shadow
##### O que é?
A propriedade CSS3 border-shadow destina-se a definir sombras em boxes ou qualquer tipo de elemento em sua página HTML usando apenas alguns códigos CSS.

##### Onde usar:
Em qualquer elemento que possui o atributo shadow.
##### Como usar:
```css
seletor { box-shadow: inset offsetX offsetY raioBlur spread cor; } 
```

##### Exemplo de uso
A sintaxe geral para aplicar as sombras é mostrada a seguir.

```html
<html>
<head>
  <title>Box-shadow em CSS3</title>
</head>
<body>
  <div id="sombra">
    <p>Esta é uma camada com sombra criada com CSS 3.</p>
  </div>
</body>
</html>
```
```css
#sombra{
  box-shadow: 5px 5px 0 #333;
  -webkit-box-shadow: 5px 5px 0 #333;
  -moz-box-shadow: 5px 5px 0 #333;
}
  
```
##### Referencia:
[http://www.maujor.com/tutorial/interativo-css3/inc/boxshadow.php](http://www.maujor.com/tutorial/interativo-css3/inc/boxshadow.php)
[http://www.linhadecodigo.com.br/artigo/3633/entendendo-o-atributo-box-shadow-nas-css3.aspx#ixzz3p3qtCVP2](http://www.linhadecodigo.com.br/artigo/3633/entendendo-o-atributo-box-shadow-nas-css3.aspx#ixzz3p3qtCVP2)




























