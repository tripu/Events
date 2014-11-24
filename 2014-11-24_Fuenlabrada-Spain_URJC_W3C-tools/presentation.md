
<style type="text/css">

  ul, li {
    line-height: 150%;
  }

  li {
    padding-top: 0.5em;
  }

  .remark-slide-container:nth-child(1) .remark-slide-number,
  .remark-slide-container:nth-child(2) .remark-slide-number,
  .remark-slide-container:nth-child(3) .remark-slide-number,
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

# **IRC** <br /> [`http://irc.w3.org`](http://irc.w3.org) <br /> canal&nbsp;&nbsp;&nbsp;&nbsp;`#w3c-urjc`
# &nbsp;
# **Twitter** <br /> [`#w3c-urjc`](https://twitter.com/search?f=realtime&q=%23w3c-urjc&src=typd)
???
Soy `tripu`; podéis preguntarme por ahí.

Publicaré la presentación en GH.

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/uk-flag.jpeg)

# Before we start&hellip;
## Quick question:
### *Would you be able to understand this talk, <br /> and to follow up with further questions or comments, <br /> **in English**?*
(Hint: you should!)

---

class: center, middle
# La *plataforma web abierta*, <br /> el futuro de la web, <br /> y por qué debería interesarte
![Logo](http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/w3c-logo2.png)
## Antonio Olmo Titos

---

.watermark[`\#w3c-urjc`]

# Sobre mí
* Estudié **ingeniería informática** en la **Universidad de Granada**.
* Acabé en 2.004; llevo diez años trabajando a tiempo completo.
* He trabajado para **9 empresas**; en **5 ciudades** de **3 países**.
* Soy **programador web** en el [equipo de sistemas](http://www.w3.org/People/domain/systeam) del [W3C](http://www.w3.org/).
* Me interesan el ***software* libre**, los **sistemas abiertos**, los **estándares**, **GNU/Linux**, la **web**, **JavaScript**, la **usabilidad**, las **interfaces de usuario** y en general el código que se puede *ver*.

.center[[`@tripu`](https://twitter.com/tripu)]

.center[[`antonio@w3.org`](mailto:antonio@w3.org)]
???
Ahora estoy en Tokio.

Soy `tripu` en redes sociales.

Tenéis mi tarjeta, y pegatinas, aquí al lado.

---

.watermark[`\#w3c-urjc`]

# De qué vamos a hablar
* El **W3C**: qué es &hellip;y qué **no** es.
* La ***plataforma web abierta***.
* **HTML** y otros estándares recientes e importantes.
* **Herramientas y recursos** que te pueden interesar.
* *Offtopic*: ideas para estudiantes de ingeniería españoles.
* &hellip;y cualquier otra cosa que surja.

---

.watermark[`\#w3c-urjc`]

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
.watermark[`\#w3c-urjc`]

# Diez cosas que (quizá) no sabías <br /> sobre el W3C y sus estándares <!--  -->

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 1. El W3C no existe

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 2. W3C &ne; W3Schools

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 3. El W3C está en España
&hellip;y en muchos sitios más.

[`http://w3c.es`](http://w3c.es)

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 4. Muchas empresas diminutas <br /> también están en el W3C
???
401 empresas miembro.

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 5. El W3C es una organización pequeña
???
83 *empleados*.

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 6. El W3C es una organización abierta
&hellip;y lo es cada vez más.

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 7. La parte legal es muy importante

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 8. La gente del W3C <br /> **no** trabaja *haciendo estándares*

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 9. Los estándares **no** se redactan para programadores y diseñadores web
&hellip;sino para un público mucho más reducido.

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 10. Los estándares son más interesantes <br /> cuando aún no son estándares

---

class: center, middle
.watermark[`\#w3c-urjc`]

http://www.w3.org/TR/
[`http://w3.org/Consortium/Recruitment`](http://w3.org/Consortium/Recruitment)

---

.watermark[`\#w3c-urjc`]

# La *Plataforma Web Abierta*
*&laquo;Una serie de tecnologías que ofrecen la posibilidad de una Web mucho más rica, ágil y fácil de usar para las personas, además de dotarla de mecanismos para permitir transformarla en una gran base de datos distribuida.&raquo;* [[fuente](http://www.w3c.es/Eventos/2013/DiaW3C/)]

*&laquo;The collection of open (royalty-free) technologies which enables the Web. Using the Open Web Platform, everyone has the right to implement a software component of the Web without requiring any approvals or waiving license fees.&raquo;* [[fuente](https://www.w3.org/wiki/Open_Web_Platform)]
???
***Platform***: ¡casi un SO!

***Open***: de vital importancia.

Videoconferencia, jugar en tiempo real, maquetar periódicos digitales en árabe&hellip;

DOM, rich editing, DB, presentation, App Cache, XHTML, HTML modules.

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/html5-logo.png)
.watermark[`\#w3c-urjc`]

---

.watermark[`\#w3c-urjc`]

# HTML5 y demás
* HTML5 es un estándar (*recommendation*) desde hace apenas un mes.
* Se ha trabajado en él durante *años*.
* HTML5 es un estándar muy grande.
* &hellip;y aún así, no engloba un montón de tecnologías que asumimos que son &laquo;HTML5&raquo;.

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/html5-diagram.png)
.watermark[`\#w3c-urjc`]

---

class: center, middle
.watermark[`\#w3c-urjc`]

# Desafíos del estándar
## Inclusión y consenso <br /> vs. <br /> agilidad

---

class: center, middle
.watermark[`\#w3c-urjc`]

# Desafíos del estándar
## *Bleeding edge* <br /> vs. <br /> conservadurismo
???
Ejemplo: API para computación cuántica (PFC vs. web púlica).

---

class: center, middle
.watermark[`\#w3c-urjc`]

# En definitiva
Para un profesional, o para un estudiante, <br /> la web es una plataforma ideal:

**Gratuita**

**Abierta**

**Colaborativa**

**Bien documentada**

**Rica en prestaciones**

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/css.png)
.watermark[`\#w3c-urjc`]

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/web-annotation.png)
.watermark[`\#w3c-urjc`]

[`http://w3.org/annotation`](http://w3.org/annotation)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/validators.png) <!--  -->
.watermark[`\#w3c-urjc`]

[`http://w3.org/QA/Tools`](http://w3.org/QA/Tools)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/html-validator1.png)
.watermark[`\#w3c-urjc`]

[`http://validator.w3.org`](http://validator.w3.org)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/html-validator2.png)
.watermark[`\#w3c-urjc`]

[`http://validator.w3.org/nu`](http://validator.w3.org/nu)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/lists.png)
.watermark[`\#w3c-urjc`]

[`http://w3.org/Mail`](http://w3.org/Mail)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/groups.png)
.watermark[`\#w3c-urjc`]

[`http://w3.org/Consortium/activities.html`](http://w3.org/Consortium/activities.html)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/projects.png)
.watermark[`\#w3c-urjc`]

[`http://w3.org/Status`](http://w3.org/Status)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/gh.png)
.watermark[`\#w3c-urjc`]

[`https://github.com/w3c`](https://github.com/w3c)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/caniuse.png)
.watermark[`\#w3c-urjc`]

[`http://caniuse.com`](http://caniuse.com)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/caniuse-video.png)
.watermark[`\#w3c-urjc`]

[`http://caniuse.com`](http://caniuse.com)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/caniuse-hyphenation.png)
.watermark[`\#w3c-urjc`]

[`http://caniuse.com`](http://caniuse.com)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/diveintohtml5.png)
.watermark[`\#w3c-urjc`]

[`http://diveintohtml5.info`](http://diveintohtml5.info)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/html5rocks-articles.png)
.watermark[`\#w3c-urjc`]

[`http://html5rocks.com`](http://html5rocks.com)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/html5rocks-resources.png)
.watermark[`\#w3c-urjc`]

[`http://html5rocks.com`](http://html5rocks.com)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/mdn.png)
.watermark[`\#w3c-urjc`]

[`https://developer.mozilla.org`](https://developer.mozilla.org)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/webplatform.png)
.watermark[`\#w3c-urjc`]

[`http://webplatform.org`](http://webplatform.org)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/whatwg.png)
.watermark[`\#w3c-urjc`]

[`https://whatwg.org`](https://whatwg.org)

---

background-image: url(http://localhost/events/2014-11-24_Fuenlabrada-Spain_URJC_W3C-tools/img/whatwg-html.png)
.watermark[`\#w3c-urjc`]

[`https://whatwg.org`](https://whatwg.org)

---

class: center, middle
.watermark[`\#w3c-urjc`]

# <code>&lt;/talk&gt;</code>
# &nbsp;
# <code>&lt;offtopic&gt;</code>

---

class: center, middle
.watermark[`\#w3c-urjc`]

# Seis ideas <br /> para estudiantes españoles de ingeniería

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 1. Make English your <br /> default work (or life!) language

---

class: center, middle
.watermark[`\#w3c-urjc`]

Júntate con los *guiris* (¡es divertido!). <!--  -->

Lee/escucha/escribe/busca en inglés primero.

Configura todos tus cacharros en inglés.

No lo estudies como si fuese una asignatura.

Vete de *Erasmus*.

Vete de *Erasmus*.

Vete de *Erasmus*.

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 2. Sacúdete los complejos españoles

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 3. Exprime a tus profesores <br /> (sobre todo a los buenos)

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 4. Sé ambicioso

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 5. Pierde el tiempo <br /> (con cabeza)

---

class: center, middle
.watermark[`\#w3c-urjc`]

# 6. Dedícate a esto sólo si te gusta <br /> (*razonablemente*)

---

class: center, middle

# Gracias

