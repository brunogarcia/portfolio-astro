---
template: BlogPost
title: "Preprocesadores CSS: estado actual y comparativa"
publishDate: "2011-12-11T18:16:00+01:00"
description: "De un tiempo a esta parte, han salido al mercado una serie de preprocesadores CSS, algunos muy buenos, otros regulares y otros muchos mueren por el camino."
tags: ["css", "less", "sass", "stylus"]
---

De un tiempo a esta parte, han salido al mercado una serie de [preprocesadores CSS](https://www.google.com/search?q=CSS+Preprocessor/), algunos muy buenos, otros regulares y otros muchos (como siempre sucede con este tipo modas) mueren por el camino, ya sea por desidia de los propios desarrolladores o quizás por falta de una comunidad que les respalde y aliente constantemente.

Si me tengo que quedar con tres, serían (en orden de preferencia):
[LESS](https://lesscss.org/), [SASS](https://sass-lang.com/) y
[Stylus](https://learnboost.github.com/stylus/)

Las dos primeras son desarrollos muy maduros y se pueden utilizar sin
problemas en cualquier proyecto profesional. Además cuentan con
comunidades muy activas que las van mejorando y puliendo poco a poco.

### Pero… ¿es para mí?

No voy a listar aquí todas las virtudes de [LESS](https://lesscss.org/) o
[SASS](https://sass-lang.com/), ya existen muchos artículos con [buenos
ejemplos y explicaciones
detalladas](https://coding.smashingmagazine.com/2011/09/09/an-introduction-to-less-and-comparison-to-sass "An Introduction To LESS, And Comparison To Sass").
Y la documentación de cada uno de ellos es bastante amplia.

Si eres nuevo/a en el mundo de los preprocesadores CSS, deberías
quedarte con dos ideas muy concretas:

- **Reducirás considerablemente el tiempo de desarrollo**, ya que
  escribirás menos código y este será de más calidad. Échale un ojo a
  las [reglas anidadas](https://lesscss.org/#-nested-rules) y a los
  [mixins](https://lesscss.org/#-mixins). Son las mas vistosas y
  fáciles de entender e implementar en cualquier desarrollo.
- **Tu flujo de trabajo cambiará a mejor**, podrás trabajar en local
  con archivos _less_ y le darás al usuario un _css_ limpio y
  minizado. Si quieres ampliar este punto, te recomiendo leer [LESS,
  lessphp & minify](https://blog.garciaechegaray.com/2011/12/07/less-lessphp-minify.html)

### Comparativa entre SASS y LESS

A continuación os muestro una comparativa a día de hoy (Diciembre 2011).

<table class="tables">
    <thead>
        <tr>
            <th>Características</th>
            <th>SASS</th>
            <th>LESS</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Repositorio</td>
            <td><a href="https://github.com/nex3/sass">Github SASS</a></td>
            <td><a href="https://github.com/cloudhead/less.js)">Github LESS</a></td>
        </tr>
        <tr>
            <td>Desarrolladores</td>
            <td>
                <ul>
                    <li><a href="https://www.twitter.com/hcatlin">Hampton Catlin</a></li>
                    <li><a href="https://twitter.com/#!/nex3">Nathan Weizenbaum</a></li>
                    <li><a href="https://twitter.com/#!/chriseppstein">Chris Eppstein</a></li>
                </ul>
            </td>
            <td>
                <a href="https://twitter.com/cloudhead">Alexis Sellier</a>
            </td>
        </tr>
        <tr>
            <td>Github antiguedad</td>
            <td>2006</td>
            <td>2010</td>
        </tr>
        <tr>
            <td>Github versión</td>
            <td>3.1.11</td>
            <td>1.1.5</td>
        </tr>
        <tr>
            <td>Github Watchers</td>
            <td>680</td>
            <td>3251</td>
        </tr>
        <tr>
            <td>Github Forks</td>
            <td>81</td>
            <td>405</td>
        </tr>
        <tr>
            <td>Lenguajes soportados</td>
            <td>Ruby</td>
            <td>
                <ul>
                    <li><a href="https://leafo.net/lessphp/">PHP</a></li>
                    <li><a href="https://github.com/asual/lesscss-servlet">Java</a></li>
                    <li><a href="https://www.dotlesscss.org">.NET</a></li>
                    <li><a href="https://search.cpan.org/~drinchev/CSS-LESSp-0.86/lib/CSS/LESSp.pm">Perl</a></li>
                    <li><a href="https://github.com/cloudhead/less.js">Javascript</a></li>
                </ul>
            </td>
        </tr>
        <tr>
            <td>Librerías complementarias</td>
            <td>
                <ul>
                    <li><a href="https://haml-lang.com/">HAML</a></li>
                    <lI><a href="https://compass-style.org/">Compass</a></lI>
                </ul>
            </td>
            <td>
              <ul>
                  <li><a href="https://jade-lang.com/">Jade</a></li>
                  <li><a href="https://lesselements.com/">LESS Elements</a></li>
                  <li><a href="https://markdotto.com/bootstrap/">Preboot.less</a></li>
                </ul>
            </td>
        </tr>
   </tbody>
</table>

---

Me ha sorprendido la **diferencia de watchers y forks** entre ambos
proyectos en Github, siendo claro ganador LESS. Todo esto a pesar de que
SASS tiene más antigüedad y triplica el número de desarrolladores.

Mi teoría es que en la comunidad _"no-ruby"_ hemos estado esperando
mucho tiempo algo similar a SASS, y ahora que por fin la tenemos hemos
ido de cabeza a disfrutar de ella.

Otro punto importante es que **la filosofía SASS ha calado como algo
evidente y necesario** en la comunidad web. Si has trabajado muchos años
con CSS, entenderás lo revolucionario que es poder utilizar variables,
funciones y reglas anidadas. Antes simplemente no había manera de
hacerlo.

Otra circunstancia: los proyectos web son cada vez más complejos y
amplios. La planificación y mantenimiento de CSS monstruosas es demasido
compleja, algo de lo que muchos de nosotros nos habíamos quejado pero
lamentablemente no sabíamos como atacar.

Hemos tenido suerte y todo ha venido rodado, paralelamente han nacido
nuevas metodologías y buenas prácticas en el mundo front-end. A destacar
[OOCSS](https://es.scribd.com/doc/60772875/OOCSS-Version-anotada-janogarcia),
[Responsive
Design](https://www.alistapart.com/articles/responsive-web-design/) y los
todavía infravalorados [frameworks
CSS](https://speckyboy.com/2011/11/17/15-responsive-css-frameworks-worth-considering/).

Y digo que hemos tenido suerte, porque no le sacaríamos todo el
potencial a OOCSS sin un buen preprocesador que actué como cimiento. A
fin de cuentas un [Objeto CSS reutilizable e
independiente](https://github.com/stubbornella/oocss/wiki) es más
sencillo de concebir y programar con una simple regla anidada. Por otra
parte, destacados frameworks CSS (por ejemplo: [Bootstrap de
Twitter](https://twitter.github.com/bootstrap/), [Golden Grid
System](https://goldengridsystem.com/), [320 and
Up](https://stuffandnonsense.co.uk/projects/320andup/) o
[Perkins](https://p.erkins.com/)) ya vienen de fábrica con su propio
archivo _less_ o _scss_, dejando claro que es la forma más adecuada y
eficiente de trabajar, independientemente de modas o buzz pasajeros.

### PHP: CMS y Frameworks

Si alguna comunidad ha sabido sacarle partido a LESS a sido PHP. Puedes
encontrar una implementación en prácticamente cualquiera de sus diversos
CMS y frameworks de desarrollo. Para muestra un botón:

- [Compilador PHP](https://leafo.net/lessphp/)
- [Drupal](https://drupal.org/project/less)
- [Wordpress](https://wordpress.org/extend/plugins/wp-less)
- [Symfony](https://www.symfony-project.org/plugins/sfLESSPlugin)
- [Yii](https://www.yiiframework.com/extension/less)
- [CakePHP](https://github.com/Phally/less)

Si tu lenguaje de programación favorito es PHP, tienes butaca preferente
en el mundo de los preprocesadores CSS, ¿a qué estas esperando?.

### IDE de desarrollo

Lamentablemente los programas para trabajar con LESS son aún escasos.

En modo multiplataforma tenemos
[PHPStorm](https://www.jetbrains.com/phpstorm/) o
[WebStorm](https://www.jetbrains.com/webstorm/), ambas de JetBrains,
creadores del famoso IntelliJ. Destacar que también tienen soporte
nativo para [CoffeeScript](https://jashkenas.github.com/coffee-script),
SASS y una decena de nuevas tecnologías. Si a esto le sumas su bajo
precio (87€ y 61€ respectivamente) entonces se convierten en la mejor
opción a día de hoy.

Si eres fan de Dreamweaver ni te molestes, actualmente no tienen soporte
ni parece que lo vaya a tener a medio o largo plazo. Quizás es una buena
excusa para actualizar tu entorno de desarrollo :)

Y si eres un Apple Boy, tienes [Espresso /
CSSEdit](https://macrabbit.com/espresso).

### Compiladores

Una mala idea es utilizar el [compilador
javascript](https://github.com/cloudhead/less.js), ya que sobrecargas tu
página con (otra) librería de 36 Kb. Aunque si quieres jugar un poco y
realizar pruebas rápidas te puede valer.

Casi mejor si compilas desde local con una app, por ejemplo:
[SimpleLess](https://wearekiss.com/simpless) (multiplataforma) o
[LESS.app](https://incident57.com/less/) (Mac).

Pero definitivamente la mejor opción es compilar directamente desde
servidor:

- [LESS PHP](https://leafo.net/lessphp/)
- [LESS Java](https://github.com/asual/lesscss-servlet)
- [LESS .NET](https://www.dotlesscss.org)
- [LESS
  Perl](https://search.cpan.org/~drinchev/CSS-LESSp-0.86/lib/CSS/LESSp.pm)

### Resumen

Creo que los desarrolladores front-end hemos gastado ya demasiado tiempo
con tonterías del tipo: hacks IE, maquetación al pixel, maquetación sin
tablas y el sexo de los ángeles (HTML5 vs. Flash).

Cuando lo realmente importante es aplicar conceptos del tipo
[orientación a
objetos](https://www.slideshare.net/stubbornella/object-oriented-css),
[DRY](https://coding.smashingmagazine.com/2011/11/07/the-future-of-css-embracing-the-machine/)
y la [escalabilidad
real](https://37signals.com/svn/posts/3003-css-taking-control-of-the-cascade)
de nuestras hojas de estilo. Y creo sinceramente que LESS es una pieza
fundamental en este nuevo entorno.

### ¿Y sobre SASS?

Soy consciente que no he profundizado en SASS. Lamentablemente no es mi
especialidad, ya que los proyectos en los que trabajo como
[freelance](https://garciaechegaray.com/) son casi 100% PHP.

Si quieres ampliar información, la mejor presentación que he leído
últimamente es: [Sass & Compass: The future of stylesheets
now.](https://speakerdeck.com/u/imathis/p/sass-compass-the-future-of-stylesheets-now)
