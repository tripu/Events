
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

  .remark-slide-content {
    background-size: contain;
  }

  .remark-slide-content .watermark {
    position: absolute;
    bottom: 12px;
    left: 20px;
    opacity: 0.5;
  }

</style>

class: center, middle

# **IRC** <br /> [`http://irc.w3.org`](http://irc.w3.org) <br /> canal&nbsp;&nbsp;&nbsp;&nbsp;`#testing`
# &nbsp;
# **Twitter** <br /> [`#w3cugr`](https://twitter.com/search?f=realtime&q=%23w3cugr&src=typd)
???
Publicaré la presentación en GH.

---

class: center, middle
# *Testing The Web Forward*
![Logo](//raw.githubusercontent.com/tripu/events/master/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img/w3c-logo.png)
## Antonio Olmo Titos
.center[[`@tripu`](https://twitter.com/tripu)]

.center[[`antonio@w3.org`](mailto:antonio@w3.org)]
???
Soy `tripu` en redes sociales **y en el IRC**; preguntad por ahí.

Tenéis mi tarjeta, y pegatinas, aquí al lado.

---

background-image: url("/Events/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/mute.png")
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#0. Soy un ser humano, tengo un computador, y éste está conectado a internet

---

background-image: url("/Events/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/irc.png")
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#1. Entrar en el canal de IRC: [`http://irc.w3.org`](http://irc.w3.org)
???
`#testing` es **público** y **en inglés**.

---

background-image: url("/Events/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/github.png")
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#2. Crear una cuenta en GitHub: [`https://github.com`](https://github.com)

---

background-image: url("/Events/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/web-platform-tests.png")
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#3. Ir al proyecto *TTWF*: [`https://github.com/w3c/web-platform-tests`](https://github.com/w3c/web-platform-tests)

---

background-image: url("/Events/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/fork.png")
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#4. Hacer un *fork* propio: [`https://github.com/`*usuario*`/web-platform-tests`](https://github.com/usuario/web-platform-tests)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#5. Instalar y configurar Git
### `$ sudo apt-get install git`
### `$ git config --global user.name '`*usuario*`'`
### `$ git config --global user.email '`*email*`'`
### `$ git config --global`<br />`  push.default upstream`

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#6. Instalar Python **2.7**
### `$ sudo apt-get install python2.7`
???
**Not** Python `3.x`.

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#7. Installar *html5lib*
### `$ sudo apt-get install python-html5lib`
.center[o bien]
### `$ pip install html5lib`
???
**Not** Python `3.x`.

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#8. Installar Node.js (no es imprescindible)
### `$ sudo apt-get install nodejs`

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#9. Añadir algunas entradas al archivo `/etc/hosts`

```bash
127.0.0.1    localhost
127.0.1.1    yeager

# The following lines are desirable for IPv6 capable hosts
::1          ip6-localhost ip6-loopback
fe00::0      ip6-localnet
ff00::0      ip6-mcastprefix
ff02::1      ip6-allnodes
ff02::2      ip6-allrouters

# web-platform-tests:
127.0.0.1     web-platform.test
127.0.0.1     www.web-platform.test
127.0.0.1     www1.web-platform.test
127.0.0.1     www2.web-platform.test
127.0.0.1     xn--n8j6ds53lwwkrqhv28a.web-platform.test
127.0.0.1     xn--lve-6lad.web-platform.test
```

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#10. *Clonar* tu *fork* del proyecto
### `$ git clone --recursive`<br />`git@github.com:`*usuario*`/`<br />`web-platform-tests.git`
.center[o bien]
### `$ git clone --recursive`<br />`https://github.com/`*usuario*`/`<br />`web-platform-tests.git`

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#11. Confirmar que tenemos los *submódulos* de Git

Si clonaste con `--recursive`, tu directorio `resources/` tendrá archivos, y no tienes que hacer nada.

En caso contrario:
### `$ cd web-platform-tests`
### `$ git submodule update --init --recursive`

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#12. Configurar *remote*/*upstream*
### `$ cd web-platform-tests`
### `$ git checkout master`
### `$ git remote add upstream https://github.com/w3c/`<br />`web-platform-tests.git`

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#13. Generar el *manifiesto* para los *tests*, `MANIFEST.json`
### `$ cd web-platform-tests`
### `$ python tools/scripts/manifest.py`

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#14. Lanzar el servidor web, *wptserve*
### `$ cd web-platform-tests`
### `$ python serve.py`

```bash
DEBUG:web-platform-tests:Route pattern: ^/tools/runner/(.*)$
DEBUG:web-platform-tests:Route pattern: ^/(.*\.py)$
INFO:web-platform-tests:Starting http server on web-platform.test:8000
DEBUG:web-platform-tests:Route pattern: ^/serve\.py$
DEBUG:web-platform-tests:Route pattern: ^/tools/(.*)$
DEBUG:web-platform-tests:Route pattern: ^/tools/runner/update\_manifest\.py$
DEBUG:web-platform-tests:Route pattern: ^/tools/runner/(.*)$
INFO:web-platform-tests:Starting http server on web-platform.test:56857
INFO:WebSocketServer:Create socket on: (2, 1, 6, '', ('127.0.0.1', 54971))
INFO:WebSocketServer:Bind on: (2, 1, 6, '', ('127.0.0.1', 54971))
INFO:WebSocketServer:Listen on: (2, 1, 6, '', ('127.0.0.1', 54971))
```

Si hay conflictos con los puertos:

`$ sudo service apache2 stop`

o bien, editar `config.default.json` y cambiar el puerto `8000` a otro libre.

---

background-image: url("/Events/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/test-runner.png")
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#15. ¡Probar! [`http://web-platform.test:8000/tools/runner/index.html`](http://web-platform.test:8000/tools/runner/index.html)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Proyectos relacionados: *wptserve*
[`https://github.com/w3c/wptserve`](https://github.com/w3c/wptserve)
* Servidor web autosuficiente
* Escrito en Python
* Se ejecuta en local
* Permite controlar el lado del servidor al ejecutar los *tests*

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Proyectos relacionados: <br /> *wptrunner* y *webdriver*
[`https://github.com/w3c/wptrunner`](https://github.com/w3c/wptrunner)

[`http://wptrunner.readthedocs.org`](http://wptrunner.readthedocs.org/en/latest/)

[`https://github.com/w3c/webdriver`](https://github.com/w3c/webdriver)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Proyectos relacionados: *testharness.js*
[`https://github.com/w3c/testharness.js`](https://github.com/w3c/testharness.js)
* Biblioteca JavaScript
* Diseñada para hacer pruebas a bajo nivel en el navegador
* Permite expresar *asertos* lógicos
* Puede usarse síncrona o asíncronamente

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Proyectos relacionados: *testharness.js*

```html
<script type="text/javascript" src="testharness.js"></script>
<script type="text/javascript" src="testharnessreport.js"></script>
```

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Proyectos relacionados: *testharness.js*

```html
<!DOCTYPE html>
<html>

  <head>
    <title>Example testharness.js Tests</title>
    <script type="text/javascript" src="testharness.js"></script>
    <script type="text/javascript" src="testharnessreport.js"></script>

    <script type="text/javascript">
      test(function() {
        assert_equals(document.body,
          document.getElementsByTagName("body")[0]));
      }, "document.body test");
      var t = async_test("Load event fires");
      onload = t.step_func(function() {t.done()});
    </script>

  </head>

  <body>
    <div id="log"></div>
  </body>

</html>
```

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Proyectos relacionados: *testharness.js*
## Tutorial breve:
[`https://github.com/w3c/testharness.js/blob/master/docs/api.md`](https://github.com/w3c/testharness.js/blob/master/docs/api.md)
## Tutorial detallado:
[`https://darobin.github.io/test-harness-tutorial/docs/using-testharness.html`](https://darobin.github.io/test-harness-tutorial/docs/using-testharness.html)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Proyectos relacionados: *csswg-test*
[`https://github.com/w3c/csswg-test`](https://github.com/w3c/csswg-test)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# ¿Y qué demonios queremos probar?

## La *Plataforma Web Abierta*

### El trabajo de estos *working groups*:
* *HTML WG*
* *Web Apps WG*
* *Device APIs WG*
* *Web Apps Security WG*

&hellip;entre otros.

---

background-image: url("/Events/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/tr.png")
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

[`http://w3.org/TR`](http://w3.org/TR)

---

background-image: url("/Events/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/tr-filtered.png")
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

[`http://w3.org/TR/tr-groups-stds`](http://w3.org/TR/tr-groups-stds)

---

background-image: url("/Events/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/html5.png")
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

[`http://w3.org/TR/html5`](http://w3.org/TR/html5)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# ¿Cómo se lee un estándar del W3C? (I)
* Lee atentamente **el principio**: *abstract* y *TOC*
* Entiende el **tipo** de *spec* (el &laquo;perfil&raquo;), y lo que implica
* Fíjate en las distintas **versiones**, y cómo están enlazadas entre sí
* [Presta atención a los **verbos**](http://www.ietf.org/rfc/rfc2119.txt): *must [not]* → *should [not]* → *may [not]*
* Fíjate en la diferencia entre lo que es **vinculante**, y lo que no: <br /> *normativo* y *no-normativo* (o *informativo*)
???
*No-normativo*: las traducciones, por ejemplo.

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# ¿Cómo se lee un estándar del W3C? (II)
* Confirma el significado de **siglas** (ej. *RCF*) y **definiciones** formales (*interoperability report*)
* Aprende a leer **BNF**, **DTD** y [**WebIDL**](http://www.w3.org/TR/WebIDL/)
* *UA* ≃ ***User Agent*** ≃ el navegador
* **Estable** (`www.w3.org/…`) vs. **en desarrollo** (`dev.w3.org/…`)
* Y sobre todo, recuerda que no deberías estar leyéndolo **tú**&hellip; ;¬)

[*How to read W3C specs*](http://alistapart.com/article/readspec)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Cómo encontrar los *tests* que te interesan
* Se usan los *shortname* de las *specs* (los de la URL)
* Máximo 3 niveles de directorios

Si no lo encuentras, usa Node.js:

```bash
$ cd web-platform-tests
$ nodejs tools/scripts/id2path.js [id]
```

En cualquier caso, ¡recuerda que puede que no exista!
???
Ejemplo: *Web Applications WG*, *Web Storage*, *Disk space*.

Resultado: el directorio está vacío (no hay *tests*), pero además ni siquiera se refiere a la *spec* que buscábamos.

Reto: escribir un *test* para [`http://w3.org/TR/webstorage/#disk-space`](http://w3.org/TR/webstorage/#disk-space)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Hay distintos tipos de *tests*
1. [Manuales](http://testthewebforward.org/docs/manual-test.html), en los que es necesaria intervención del usuario
1. [*Reftests*](http://testthewebforward.org/docs/reftests.html), en los que el usuario debe comparar dos resultados
1. [JavaScript con *testharness.js*](http://testthewebforward.org/docs/testharness.html), completamente automáticos

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Tipos de *tests*, nº 1: manuales
Completamente abiertos a la imaginación del programador <br /> (y a los límites de la inteligencia humana)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Tipos de *tests*, nº 2: *reftests*
* Siempre pares de archivos: *asunto*`.html` y *asunto*`-ref.html`
* Los resultados de *renderizar* ambos deben ser idénticos
* El usuario es responsable de decidir si el *test* pasa o no, *a ojímetro*

```html
<!DOCTYPE html>
<meta charset="utf-8">
<title>BDO element dir=rtl</title>
<link rel="help"
  href="http://www.whatwg.org/specs/web-apps/current-work/#the-bdo-element">
<meta name="assert"
  content="BDO element's DIR content attribute renders well with 'rtl'.">
<link rel="match" href="test-bdo-001.html">
<p>Pass if you see WAS displayed below.</p>
<bdo dir="rtl">SAW</bdo>
```

```html
<!DOCTYPE html>
<meta charset="utf-8">
<title>HTML Reference File</title>
<p>Pass if you see WAS displayed below.</p>
<p>WAS</p>```

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Tipos de *tests*, nº 3: <br /> JavaScript con *testharness.js*
 * [Documentación de la API de *testharness.js*](http://testthewebforward.org/docs/testharness-library.html)
 * [Cómo usar *testharness.js* en tus *tests*](http://testthewebforward.org/docs/testharness-idlharness.html)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Es mejor empezar con una plantilla
[`http://testthewebforward.org/docs/test-templates.html`](http://testthewebforward.org/docs/test-templates.html)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Cómo enviar tus *tests* al proyecto
Básicamente, siguiendo el modelo de GitHub

*Fork* → *branch* → *commit* → *PR*

[`http://testthewebforward.org/docs/submission-process.html`](http://testthewebforward.org/docs/submission-process.html)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Consultar el estado actual de los *tests*
[`http://w3c-test.org/`](http://w3c-test.org/)

---

background-image: url("/Events/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/prs.png")
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

[`https://github.com/w3c/web-platform-tests/pulls`](https://github.com/w3c/web-platform-tests/pulls)

---

background-image: url("/Events/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/issues.png")
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

[`https://github.com/w3c/web-platform-tests/issues`](https://github.com/w3c/web-platform-tests/issues)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Lista de distribución
## `public-test-infra@w3.org`
### Para [suscribirse](mailto:public-test-infra-request@w3.org?subject=subscribe): <br /> `public-test-infra-request@w3.org`
### Archivo de mensajes: [`http://lists.w3.org/Archives/Public/`<br />`public-test-infra/`](http://lists.w3.org/Archives/Public/public-test-infra/)

---

class: center, middle

# Gracias
