
<style type="text/css">

  ul, li {
    line-height: 150%;
  }

  li {
    padding-top: 0.5em;
  }

  .remark-slide-container:nth-child(1) .remark-slide-number,
  .remark-slide-container:nth-child(2) .remark-slide-number,
  .remark-slide-container:last-child .remark-slide-number {
    visibility: hidden;
  }

  .remark-slide-content .watermark {
    position: absolute;
    bottom: 12px;
    left: 20px;
    opacity: 0.5;
  }

</style>

class: center, middle

# **IRC** <br /> [`http://irc.w3.org`](http://irc.w3.org) <br /> canal&nbsp;&nbsp;&nbsp;&nbsp;`#w3cuc3m`
# &nbsp;
# **Twitter** <br /> [`#w3cuc3m`](https://twitter.com/search?f=realtime&q=%23w3cuc3m&src=typd)
???
Soy `tripu`; podéis preguntarme por ahí.

Publicaré la presentación en GH.

---

class: center, middle
# La *Plataforma Web Abierta* y los *MOOCs*
## Seminario &laquo;Tecnologías para la educación online&raquo;
![Logo](//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/w3c-logo.png)
### Antonio Olmo Titos

---

.watermark[`\#w3cuc3m`]

# Sobre mí
* Estudié **ingeniería informática** en la **Universidad de Granada**.
* He trabajado para **8 empresas**; en **5 ciudades** de **3 países**.
* Soy **programador web** en el [equipo de sistemas](http://www.w3.org/People/domain/systeam) del [W3C](http://www.w3.org/).
* Me interesan el ***software* libre**, los **sistemas abiertos**, los **estándares**, **GNU/Linux**, la **web**, **JavaScript**, la **usabilidad**, las **interfaces de usuario** y en general el código que se puede *ver*.

.center[[`@tripu`](https://twitter.com/tripu)]

.center[[`antonio@w3.org`](mailto:antonio@w3.org)]
???
Ahora estoy en Tokio.

Soy `tripu` en redes sociales **y en el IRC**; preguntad por ahí.

Tenéis mi tarjeta, y pegatinas, aquí al lado.

---

.watermark[`\#w3cuc3m`]

# De qué vamos a hablar
* Breve introducción al **W3C** y a sus estándares.
* La ***Plataforma Web Abierta***.
* **HTML[5]** y otras tecnologías relacionadas.
* La web y los ***MOOCs***.
* **Herramientas y recursos** para *MOOCs*.
* &hellip;y cualquier otra cosa que surja.

---

.watermark[`\#w3cuc3m`]

# El W3C

*&laquo;In October 1994, [Tim&nbsp;Berners-Lee](http://www.w3.org/People/Berners-Lee/) founded the [World Wide Web Consortium (W3C)](http://www.w3.org/) at the Massachusetts Institute of Technology.&raquo;* [[fuente](http://www.w3.org/Consortium/facts#history)]

* Internacional.
* Sin ánimo de lucro.
* Financiada a través de:
 * Cuotas de empresas miembro.
 * Donaciones.
* Comprometida con una web:
 * Abierta.
 * Interoperable.
 * Agnóstica.
 * Duradera.
???
Ejemplos: URL's eternas, *vendor neutrality*.

Primer estándar: PNG.

---

class: center, middle
.watermark[`\#w3cuc3m`]

# Diez cosas que (quizá) no sabías <br /> sobre el W3C y sus estándares <!--  -->

---

class: center, middle
.watermark[`\#w3cuc3m`]

# 1. El W3C no existe

---

class: center, middle
.watermark[`\#w3cuc3m`]

# 2. W3C &ne; W3Schools

---

class: center, middle
.watermark[`\#w3cuc3m`]

# 3. El W3C está en España
&hellip;y en muchos sitios más.

[`http://w3c.es`](http://w3c.es)

---

class: center, middle
.watermark[`\#w3cuc3m`]

# 4. Muchas empresas diminutas <br /> también están en el W3C
???
401 empresas miembro.

---

class: center, middle
.watermark[`\#w3cuc3m`]

# 5. El W3C es una organización pequeña
???
83 *empleados*.

---

class: center, middle
.watermark[`\#w3cuc3m`]

# 6. El W3C es una organización abierta
&hellip;y lo es cada vez más.

---

class: center, middle
.watermark[`\#w3cuc3m`]

# 7. La parte legal es **muy** importante

---

class: center, middle
.watermark[`\#w3cuc3m`]

# 8. La gente del W3C <br /> **no** trabaja *haciendo estándares*

---

class: center, middle
.watermark[`\#w3cuc3m`]

# 9. Los estándares no se redactan <br /> (solamente) <br /> para programadores y diseñadores
???
&hellip;sino para un público mucho más reducido.

---

class: center, middle
.watermark[`\#w3cuc3m`]

# 10. Los estándares son más interesantes <br /> cuando aún no son estándares

---

class: center, middle
.watermark[`\#w3cuc3m`]

[`http://www.w3.org/TR/`](http://www.w3.org/TR/)

---

.watermark[`\#w3cuc3m`]

# La *Plataforma Web Abierta*
*&laquo;Una serie de tecnologías que ofrecen la posibilidad de una Web mucho más rica, ágil y fácil de usar para las personas, además de dotarla de mecanismos para permitir transformarla en una gran base de datos distribuida.&raquo;* [[fuente](http://www.w3c.es/Eventos/2013/DiaW3C/)]

*&laquo;The collection of open (royalty-free) technologies which enables the Web. Using the Open Web Platform, everyone has the right to implement a software component of the Web without requiring any approvals or waiving license fees.&raquo;* [[fuente](https://www.w3.org/wiki/Open_Web_Platform)]
???
***Platform***: ¡casi un SO!

***Open***: de vital importancia.

OWP = formatos + APIs

Videoconferencia, jugar en tiempo real, maquetar periódicos digitales en árabe&hellip;

DOM, rich editing, DB, presentation, App Cache, XHTML, HTML modules.

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/html5-logo.png)
.watermark[`\#w3cuc3m`]

---

.watermark[`\#w3cuc3m`]

# HTML5: ¿qué hay de nuevo?
* Sintaxis simplificada
* Integración de MathML y SVG
* Añadidos nuevos elementos y atributos
* Eliminados viejos elementos y atributos
* Añadidas APIs nuevas para *scripting*

---

.watermark[`\#w3cuc3m`]

# HTML5: nuevos elementos
* `<video>` y `<audio>`
* `<canvas>`
* `<ruby>`
* `<article>`, `<section>`, `<header>`&hellip;
* `<details>`, `<progress>`&hellip;

---

.watermark[`\#w3cuc3m`]

# HTML5: la historia
* HTML5 es un estándar (*recommendation*) desde hace apenas un mes.
* Se ha trabajado en él durante *años*.
* HTML5 es un estándar muy grande.
* &hellip;y aún así, no engloba un montón de tecnologías que asumimos que son &laquo;HTML5&raquo;.
???
* *CSS3* (no)
* *WebSocket* (sí)
* *Canvas 2D* (sí)
* *WebGL* (no)
* *SVG* (no)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/html5-diagram.png)
.watermark[`\#w3cuc3m`]
???
* *CSS3* (no)
* *WebSocket* (sí)
* *Canvas 2D* (sí)
* *WebGL* (no)
* *SVG* (no)

---

.watermark[`\#w3cuc3m`]

# HTML5: APIs relacionadas
* *Canvas 2D Context API*
* WebGL (*canvas 3D API*)
* *Web Storage API*
* *Indexed DB API* (noSQL)
* *Web Workers*
* *WebSocket*

---

class: center, middle
.watermark[`\#w3cuc3m`]

# Desafíos del estándar
## Inclusión y consenso <br /> vs. <br /> agilidad

---

class: center, middle
.watermark[`\#w3cuc3m`]

# Desafíos del estándar
## *Bleeding edge* <br /> vs. <br /> conservadurismo
???
Ejemplo: API para computación cuántica (PFC vs. web pública).

---

class: center, middle
.watermark[`\#w3cuc3m`]

# En definitiva
Para un estudiante (y también para un profesional), <br /> la web es una plataforma ideal:

**Gratuita**

**Abierta**

**Colaborativa**

**Bien documentada**

**Rica en prestaciones**

**Con inmensa difusión**

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/css.png)
.watermark[`\#w3cuc3m`]

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/web-annotation.png)
.watermark[`\#w3cuc3m`]

[`http://w3.org/annotation`](http://w3.org/annotation)
???
Ya conocéis un recurso, y lo estáis usando: IRC.

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/validators.png)
.watermark[`\#w3cuc3m`]

[`http://w3.org/QA/Tools`](http://w3.org/QA/Tools)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/html-validator1.png)
.watermark[`\#w3cuc3m`]

[`http://validator.w3.org`](http://validator.w3.org)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/html-validator2.png)
.watermark[`\#w3cuc3m`]

[`http://validator.w3.org/nu`](http://validator.w3.org/nu)&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;[`https://validator.nu`](https://validator.nu)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/lists.png)
.watermark[`\#w3cuc3m`]

[`http://w3.org/Mail`](http://w3.org/Mail)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/groups.png)
.watermark[`\#w3cuc3m`]

[`http://w3.org/Consortium/activities.html`](http://w3.org/Consortium/activities.html)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/projects.png)
.watermark[`\#w3cuc3m`]

[`http://w3.org/Status`](http://w3.org/Status)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/gh.png)
.watermark[`\#w3cuc3m`]

[`https://github.com/w3c`](https://github.com/w3c)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/caniuse.png)
.watermark[`\#w3cuc3m`]

[`http://caniuse.com`](http://caniuse.com)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/caniuse-video.png)
.watermark[`\#w3cuc3m`]

[`http://caniuse.com`](http://caniuse.com)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/caniuse-hyphenation.png)
.watermark[`\#w3cuc3m`]

[`http://caniuse.com`](http://caniuse.com)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/diveintohtml5.png)
.watermark[`\#w3cuc3m`]

[`http://diveintohtml5.info`](http://diveintohtml5.info)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/html5rocks-articles.png)
.watermark[`\#w3cuc3m`]

[`http://html5rocks.com`](http://html5rocks.com)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/html5rocks-resources.png)
.watermark[`\#w3cuc3m`]

[`http://html5rocks.com`](http://html5rocks.com)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/mdn.png)
.watermark[`\#w3cuc3m`]

[`https://developer.mozilla.org`](https://developer.mozilla.org)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-12-02_Leganés-Spain_UC3M_W3C-MOOCs/img/webplatform.png)
.watermark[`\#w3cuc3m`]

[`http://webplatform.org`](http://webplatform.org)

---

class: center, middle

# Gracias

