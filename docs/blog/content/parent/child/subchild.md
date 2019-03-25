---
title: "Debilidades de los web generators"
date: 2019-03-25T02:10:46-06:00
draft: true
---
Código C#

```c#
public void Hello(){
    Console.WriteLine("Hello world");
}
```
Desventajas:<br></br>
<body>Mientras que las ventajas de las páginas estáticas ya mencionadas, como la velocidad de entrega o el elevado factor de seguridad, no son nada desdeñables, hay razones importantes que explican por qué un static site generator no es apropiado para proyectos de gran envergadura. Ante todo hay que mencionar los enormes esfuerzos de mantenimiento: trabajar con un generador no solo requiere amplios conocimientos sobre Markdown, HTML, etc., sino que carece de numerosos automatismos que se dan por supuestos en los sistemas de gestión de contenidos y en los sistemas de creación modular de páginas web. Algunas de las desventajas derivadas de la utilización de static website generators son:
Ausencia de contenidos en tiempo real: los static site generators no ofrecen posibilidades para generar contenidos dinámicos (sugerencias, actualización de precios, búsqueda de texto completo, etc.). Los elementos que se adaptan automáticamente a los usuarios correspondientes evaluando los datos en tiempo real solo se llevan a cabo por otras vías, p. ej., con ayuda de scripts del lado del cliente (sobre todo JavaScript). Estos plantean, sin embargo, posibles brechas de seguridad que implican riesgos tanto para las páginas web como para sus visitantes. Además, muchos usuarios bloquean JavaScript y otros lenguajes de script en sus navegadores, por lo que los contenidos correspondientes permanecen ocultos. 
Uso laborioso de datos de entrada de usuario (user input): otro problema de la falta de scripts del lado del servidor y de bases de datos se hace patente cuando, en algunas situaciones, los proyectos web deben facilitar entradas de usuario como, por ejemplo, en un formulario de contacto. Si quieres integrar este tipo de elementos a una página estática, tendrás que recurrir inevitablemente a JavaScript o a servicios de proveedores externos. La plataforma DISQUS puede utilizarse, por ejemplo, para agregar comentarios a proyectos elaborados con generadores de páginas web (incluida la moderación y la gestión de spam), pero este servicio también recurre a JavaScript. El ya mencionado repositorio GitHub Pages ofrece, además, una función de comentarios que está estrechamente relacionada con el control de las versiones y cuyo análisis se realiza del lado del servidor. En cualquier caso, la inversión de trabajo y tiempo necesaria para desarrollar tales componentes de usuario son, en comparación, muy elevados.
Ausencia de una interfaz de usuario estándar: los static website generators no vienen de fábrica con una interfaz en la que puedan añadirse nuevos contenidos o en la que los ya existentes puedan adaptarse o eliminarse. Los editores WYSIWYG ayudan a escribir el código Markdown necesario y a visualizar a priori el resultado mediante la función de vista previa, pero no evitan que los archivos creados tengan que cargarse manualmente en el servidor. Este proceso es especialmente difícil de entender para los redactores con conocimientos básicos sobre código y estructura de la página web, por lo que su uso conllevará más tiempo que, por ejemplo, en el caso de un CMS como WordPress.
En resumen, se puede decir que los proyectos basados en páginas estáticas presentan desventajas sobre todo en cuanto a la actualidad, las modificaciones y la interacción del usuario. Si:
se revisan los contenidos regularmente, 
se añaden funcionalidades a posteriori, 
se procesan los datos de los usuarios o
se realizan modificaciones ópticas en cualquier momento e incluso con conocimientos mínimos,
las soluciones como los page builders o los sistemas de gestión de contenidos se anteponen a los web page generators.</body>
