
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

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/mute.png)
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#0. Soy un ser humano, tengo un computador, y éste está conectado a internet

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/irc.png)
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#1. Entrar en el canal de IRC: [`http://irc.w3.org`](http://irc.w3.org)
???
`#testing` es **público** y **en inglés**.

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/github.png)
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#2. Crear una cuenta en GitHub: [`https://github.com`](https://github.com)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/web-platform-tests.png)
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#3. Ir al proyecto *TTWF*: [`https://github.com/w3c/web-platform-tests`](https://github.com/w3c/web-platform-tests)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/fork.png)
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#4. Hacer un *fork* propio: [`https://github.com/`*usuario*`/web-platform-tests`](https://github.com/usuario/web-platform-tests)

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#5. Installar Git y Python **2.7**
### `$ sudo apt-get install git`
### `$ sudo apt-get install python2.7`
???
**Not** Python `3.x`.

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#6. Installar *html5lib*
### `$ sudo apt-get install python-html5lib`
.center[o bien]
### `$ pip install html5lib`
???
**Not** Python `3.x`.

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#7. Installar Node.js (no es imprescindible)
### `$ sudo apt-get install nodejs`

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#8. Añadir algunas entradas al archivo `/etc/hosts`

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

\#9. *Clonar* tu *fork* del proyecto
### `$ git clone`<br />`git@github.com:`*usuario*`/`<br />`web-platform-tests.git`
.center[o bien]
### `$ git clone`<br />`https://github.com/`*usuario*`/`<br />`web-platform-tests.git`

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#10. Actualizar los *submódulos* de Git
### `$ cd web-platform-tests`
### `$ git submodule update --init --recursive`

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#11. Generar el *manifiesto* para los *tests*, `MANIFEST.json`
### `$ cd web-platform-tests`
### `$ python tools/scripts/manifest.py`

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#12. Lanzar el servidor web, *wptserve*
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

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/test-runner.png)
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

\#13. ¡Probar! [`http://web-platform.test:8000/tools/runner/index.html`](http://web-platform.test:8000/tools/runner/index.html)

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
[`http://w3.org/TR`](http://w3.org/TR)

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/tr.png)
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

df

---

background-image: url(//raw.githubusercontent.com/tripu/events/master/2014-11-28_Granada-Spain_UGR_W3C-TTWF/img-ttwf/tr-filtered.png)
.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# foo

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# foo

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# foo

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# foo

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# foo

---

.watermark[IRC `#testing`&nbsp;&nbsp;&nbsp;&nbsp;&mdash;&nbsp;&nbsp;&nbsp;&nbsp;Twitter `\#w3cugr`]

# Lista de distribución
## `public-test-infra@w3.org`
### Para [suscribirse](mailto:public-test-infra-request@w3.org?subject=subscribe): <br /> `public-test-infra-request@w3.org`
### Archivo de mensajes: [`http://lists.w3.org/Archives/Public/`<br />`public-test-infra/`](http://lists.w3.org/Archives/Public/public-test-infra/)

---

class: center, middle

# Gracias

