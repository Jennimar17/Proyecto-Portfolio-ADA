### Comentarios Generales

Jenni, queria en primer lugar comentar qué lindo quedó tu portfolio. Está lleno de detalles hermosos, se nota que lo hiciste con pasión y mucho cuidado. Me encanta cómo te quedaron las tarjetas, qué lindo detalle hacerlas redondas. Los gradientes en el fondo del footer y la cita son tambien un agregado fantástico. La paleta de colores, la tipografia, todo quedó perfecto para reflejate y demostrar que hiciste tuyo este trabajo. 

En algunas de las cosas que cambiaste también te escapaste de las consignas, y si bien lo resolviste muy bien a nivel visual y código, tengo que contemplar que no todo lo que pedimos está cumplido. Es importante cumplir requerimientos, y aunque no dudo que vayas a hacerlo a nivel laboral, le doy importancia porque hay algunas cosas que agregamos específicamente porque queríamos ver cómo las resolvían (por darte un ejemplo sencillo, no es casual que haya seis tarjetas de conocimientos alineadas al centro, pero siete de proyectos alineadas a la vez al centro y con flex-start). Lo mismo con la barra de navegacion tirada hacia la derecha. De esas cosas, creo que la que produciria un mayor impacto visual en tu web sea ajustarse a un ancho para la frase. 

Tu responsive funciona muy bien, pero tenes algunos problemas que en general estan causados por darle un width de 100% a las cosas. Si le decimos a un elemento: "tenes que medir el 100% del ancho de tu contenedor", pero ademas le agregamos padding o margin, el elemento va a medir 100% + el ancho que le hayas dado. Ese es el motivo por el cual en celulares y tablets tu portfolio fuerza un scroll horizontal (por eso se ve una barra blanca al costado). Eso ocurre tanto en el footer como en la barra de navegacion: ambos tienen width 100% con padding entonces terminan siendo mas grandes que el body. En el caso del footer en las resoluciones más pequeñas, tenes ademas el problema de que el texto de los links es muy ancho y termina rebalsando. Achicar el tamaño de texto o darle flex-wrap lo solucionaría. 

- Usas muchos <br> para estilar. Esto no se considera buena practica. El primer motivo es porque en general representa una violacion del principio de separacion de responsabilidades: al usar <br> para dar un estilo (que las cosas se pongan una debajo de la otra), dejamos los estilos en el HTML en lugar de estar en su lugar, que es CSS. Por otro lado, eso a veces te provoca problemas. Mira por ejemplo como se ve tu frase en una resolucion de 768px: algunas palabras hacen un salto de linea, otras no, y el efecto no es bueno. Es preferible dejar que los textos se acomoden solos, y en todo caso darle un width a su contenedor si deseamos que se ajusten a una medida, pero no forzar un salto de linea a menos que podamos controlarlo en todas las resoluciones. 

- Tus nombres de clases son excelentes, mucho mejores de lo que se espera de una desarrolladora con tu experiencia. Cumplis bien el requisito de que sean descriptivos en un sentido funcional: describir que es un elemento y qué hace, no necesariamente como se ve. Hay algunas excepciones, ocasionalmente usas el color o el contenido de una clase, pero en general lo manejas muy bien. Felicitaciones por eso. 

- No usas las etiquetas semanticas salvo excepciones. Hay muchos <div> que deberian ser secciones y muchos div que deberian ser article (las tarejtas de habilidades y proyectos). Te deje anotado tambien algo sobre el uso de los h1, h2, etc.  

- Tus imagenes no tienen su tamaño fijado por los estilos. Hoy no es tan importante, porque vos sabes cuanto miden tus imagenes y podes hacerlas todas del mismo tamaño. Pero es importante que te acostumbres a trabajar asumiendo que pueden ser de cualquier medida: eventualmente vamos a empezar a trabajar con imagenes que vienen de bases de datos, que no sabemos que tamaño o forma tendran. Es importante saber como "domesticarlas" desde el CSS para que una imagen con un tamaño inesperado no rompa todo nuestra web. 

- El identado y prolijidad de tu codigo, tanto HTML como CSS, es destacable. Tambien la buena organizacion de archivos, y la prolijidad de tu repo en github. Tu README es fantastico, y leer lo excelente de tus mensajes de commit, ver que usaste branches... Excelente! 

Dejo algunos comentarios generales sobre tu codigo. 
Sé que puedo ser un poco quisquillosa en las correcciones. No es la intención que sientas que hiciste un mal trabajo, porque no es así: tu trabajo es fantástico. Mi tarea es comentarte todo lo que vea para que sea más fantástico aún. 


### Nota final: 8

Nota desagregada: 
✅ Estructura correcta de documento HTML.
✅ Respeta la consigna 
✔️ Respeta el diseño dado --> con observaciones
✔️ Responsive funciona correctamente --> con observaciones
✅ Código bien indentado. 
✅ Comentarios que permiten mejorar la legibilidad del código.
✔️ Uso correcto de etiquetas semánticas --> con observaciones
✅ Buenos nombres de clases
✅ Reutilización de estilos.
✅ Código CSS ordenado.
✅ Commits con mensajes adecuados.
