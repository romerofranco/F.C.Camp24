**_ Este es un README con motivos descriptivos, solo para saber que comandos se usaron paso a paso para armar el formulario y saber tambien que funcion cumple y tienen tanto internos como externos. _**
**Va desde el paso 1 hasta el paso 65**

**Step 1**
Bienvenido al proyecto de formulario de registro. Comience anadiendo la declaracion !DOCTYPE html en la parte superior del documento para que el navegador sepa que tipo de documento lee.

**Step 2**

- Abajo del DOCTYPE, anade un elemento html con un atributo lang establecido a "en" , para que tengas espacio para comenzar a poner codigo.

**Step 3**

- A continuacion, agrega las etiquetas de apertura y cierre de las etiquetas head y body dentro del elemento html.

**Step 4**
-anade un title y un elemento meta dentro del elemento head. Dale a tu proyecto el titulo de Registration Form y anade un titulo charset con el valor utf-8 a tu elemento meta

**Step 5**

- anida un elemento link dentro del elemento head. Dale un atributo _rel_ con el valor _stylesheet_ y un atributo _href_ con el valor _styles.css_ esta es la forma de contectar el html con el css.

**Step 6**
-Dentro del body, proporciona un contexto de encabezado para el contenido, agregando un h1 con el texto Registration Form

**Step 7**
-Debajo del encabezado, utilice el siguiente texto dentro de un elemento de parrafo para animar a los usuarios a registrarse.

**Step 8**
-La unidad vh significa viewport height (altura de pantalla) y es relativa al 1% de la altura (height) de la pantalla. Esto le hace relativa a la altura de la pantalla/ventana grafica.
-Es hora de engalanar el proyecto con un poco de CSS. Comienza estableciendo para body la propiedad width a 100%, y la propiedad height a _100vh_.

**Step 9**
-Ahora, deshazte de la barra de desplazamiento horizontal, estableciendo el margin por defecto del body anadiendo algunos navegadores a 0.

**Step 10**
-Eso es mejor.Ahora, haz que el fondo sea facil de ver, cambiando el body background-color a #1b1b32. Luego, para ver el texo, cambia el color a #f5f6f7.

**Step 11**
-Como sugiere el titulo, estas creando un formulario. Por lo tanto, despues del elemento p inserta un form con un atributo action apuntando a *https://register-demo.freecodecamp.org*

**Step 12**
-El atributo _method_ especifica como enviar datos de formulario a la direccion URL especificada en el atributo _action_. Los datos del formulario se pueden enviar a traves de una solicitud _GET_ como parametros de URL (con _method="get"_) o mediante una solicitud _POST_ como datos en el cuerpo de la solicitur con (_method="post"_). Establezca el atributo _method_ para enviar los datos del formulario a traves de una solicitud _post_.

**Step 13**

- Como el formulario tiene tres secciones distintas, agrega tres elementos _fieldset_ dentro del elemento form.

**Step 14**
-El primer _fieldset_ contendra los campos de nombre, email y contrasenia. Empieza agregando cuatro elementos _label_ al primer _fieldset_.

**Step15**
-Agrega el siguiente texto a los elementos _label_:
-Enter your First Name.
-Enter your Last Name.
-Enter your Email.
-Create a New Password.

**Step 16**
-La unidada rem significa root(raiz) em, y es relativa al tamanio de fuente del elemento html.
Como los elementos label por defecto son inline, se muestran todos juntos en la misma linea, haciendo dificil su lectura. Para mostrarselos en diferentes lineas, anade _display:block_ al elemento label, y dale a la propiedad margin un valor de _0.5rem 0_, para darles un poco de separacion.

**Step 17**
-Anida un elemento input dentro de cada label. Asegurate de agregar cada input despues del texto del label, e incluye un espacio despues de los dos puntos

**Step 18**
-Siguiendo las mejores practicas de accesibilidad, vincule los elementos _input_ y los elementos _label_ utilizando el atributo _for_.

- Utiliza _first-name_,_last-name_,_email_ y _new-password_ como valores para los respectivos atributos _id_ .
- _(EL label lleva el for y el input el id)_

**Step 19**
-Especificar el atributo _type_ de un elemento de formulario es importante para que el navegador sepa que tipo de datos debe esperar. Si el _type_ no esta especificado, el navegador utilizara por defecto _text_.

-Da a los dos primeros elementos _input_ un atributo _type_ de _text_, al tercero un atributo _type_ de _email_ y al cuarto un atributo _type_ de _password_.

-El type _email_ solo permite correos electronicos con _@_ y un _.(punto)_ en el domino. El type _password_ oculta la entrada, y adviertesi el sitio no utiliza HTTPS

**Step 20**
-El primer elemento _input_ con un _type_ de _submit_ se establece automaticamente para enviar a su elemento _form_ padre mas cercano.

- Para manejar el envio del formulario, despues del ultimo elemento _fieldset_ agrega un elemento _input_ con el atributo _type_ establecido en _submit_ y el atributo _value_ establecido en _submit_.

**Step 21**
-En este punto, deberias poder enviar el formulario.Sin embargo, puede notar que no pasa casi nada. Para hacer el formulario mas interactivo agrega el atributo _required_ a los elementos _input_ en el primer _fieldset_.
-Ahora, si intentas enviar el formulario sin rellenar los campos requeridos, vera un mensaje de error.

**Step 22**
-Algunos valores del atributo _type_ vienen con una validacion de formulario incorporada. Por ejemplo, _type="Email"_ requiere que el valor sea un direccion de correo electronico valida.

-Agrega validacion personalizada al elemento _input_ de contrasenia, agregando un atributo _minlenght_ con un valor de 8. De este modo se evita que se envien entradas de menos de 8 caracteres.

**Step 23**

- Con el _type="password"_ puedes usar el atributo _pattern_ para definir una expresion regular que la contrasena debe coincidir para ser considerada valida.

-Agrega un atributo _pattern_ al elemento _input_ de contrasena para requerir que la entrada coincida con : _[a-z0-5]{8,}_ .

**Step 24**

- Pasemos a la siguiente parte del formulario de registro. Esta seccion pedira el tipo de cuenta que el usuario esta creando.
  Empieza agregando dos elementos _label_ al segundo _fieldset_.

**Step 25**
-Los usuarios podran elegir entre _Personal_ o _Bussines_.
-Para ello, dentro de cada uno de los dos primeros elementos _label_, agrega un elemento _input_ con _type="radio"_

**Step 26**
-Dentro de cada elemento _label_ correspondiente, e inmediatamente despues del elemento _input_, agrega un espacio y agregar el siguiente texto :
Persona
Bussines

**Step 27**
-Solo quieres que se pueda seleccionar un input de radio a la vez. Sin embargo, el formulario no sabe que los inputs de radio estan relacionadas.

- Para relacionarlos , dales el mismo atributo _name_ con un valor de _account-type_. Ahora, no es posible seleccionar ambos inputs de radio al mismo tiempo.

**Step 28**
-Por ahora, los usuarios pueden enviar el formulario sin seleccionar los inputs de tipo radio. Aunque anteriormente usamos el atributo _required_ para indicar que un input es obligatorio, en este caso, anadir _required_ a ambos inputs no funcionara, ya que transmitira informacion incorrecta a los usuarios.

-Para resolver esto, puedes proporcionar contexto de lo que se necesita, anadiendo un elemento (legend) con el texto _Account type (required)_ antes de los elementos _label_ dentro del segundo _fieldset_. Despues anade un atributo _checked_ al input con el texto _Personal_ para asegurarse de que el formulario se envia con datos requeridos.

**Step 29**
-Siga las mejores practicas de accesibilidad vinculando los elementos _input_ y los elementos _label_ en el segundo _fieldset_.
-Utiliza _personal-account_ y _bussines-account_ como valores respectivos para los atributos _id_.

**Step 30**

- Debe confirmar que el usuario ha leido los terminos y condiciones (terms and conditions).
  -anade un elemento _label_.Dentro del nuevo elemento _label_, agrega un elemento _input_ con un atributo _type_ con el valor _checkbox_. Haz que este elemento _input_ sea requerido (required) para que los usuarios no puedan registrarse sin leer los terminos y condiciones.
  -anade un atributo _id_ y un atributo _for_ y dales el valor _terms-and-conditions_ para accesibilidad.

**Step 31**

- Anade el texto _I accept the terms and conditions_ inmediatamente despues del elemento del _input_ en la _label_ recien anadida. Despues, vincula el texto _Terms and conditions_ al siguiente enlace. *https://www.freecodecamp.org/news/terms-of-service/*

**Step 32**
-Pasando al final _fieldset_. Que pasa si quisiera permitir que un usuario suba una foto de perfil?.
-Bueno, el _input_ con tipo _file_ permite eso. Agrega un _label_ con el texto _Upload a profile picture:_ y anidaun _input_ aceptando la carga del archivo.

**Step 33**
-anade otro _label_ despues de la primera, con el texto _Input your age (years):_ . Luego, anida un _input_ con el _type_ de _number_.
-A continuacion, anade un atributo _min_ al _input_ con un valor de _13_ porque los usuarios menores de 13 anos no deben registrarse. Ademas,los usuarios probablemente no superen la edad de 120; agregue un atributo _max_ con un valor de _120_.
-Ahora, si alguien intenta enviar el formulario con valores fuera del rango, aparecera una advertencia, y el formulario no enviara.

**Step 34**
-Anadir un menu desplegable al formulario es facil con el elemento _select_. El elemento _select_ es un contenedor para un grupo de elementos _option_, y el elemento _option_ actua como una etiqueta para cada opcion desplegable. Ambos elementos requieren etiquetas de cierre.

- Comienza anadiendo un elemento _select_ debajo de los dos elementos _label_. Luego anida 5 elementos _option_ dentro del elemento _select_

**Step 35**
-Nida el elemento _select_ (con sus elementos _option_) dentro de _label_ con el texto _How did you hear about us?_. El texto debe venir antes del elemento _select_.

**Step 36**
-Las opciones desplegables estan actualmente vacias. Para darles contenido, agregue el siguiente texto a cada elemento subsecuente de _option_:
-(Select one)
-freecodecamp News
-freecodecamp YouTube Channel
-freecodecamp Forum
-Other.

**Step 37**
-Enviar el formulario con una opcion seleccionada no enviaria un valor util al servidor. Por lo tanto, cada elemento _option_ necesita que se le de un atributo _value_. Sin el cual, el contenido de texto del _option_ sera enviado al servidor.
-Dale al primer _option_ un _value_ de _""_, y a los elementos _option_ subsecuentes atributos _value_ del 1 al 4.

**Step 38**
-El elemento _textarea_ actua como un elemento _input_ de tipo _text_, pero viene con la ventaja anadida de poder recibir texto de varias lineas, y un numero inicial de filas y columnas.

-Los usuarios podran registrarse con una biografia. Agregar un _label_ con el texto _Provide a bio_ al final del _fieldset_. Agrega un elemento _textarea_ dentro del elemento _label_. Tenga en cuenta que el elemento _textarea_ requiere una etiqueta de cierre.

**Step 39**
-Vincule los elementos de formulario aplicables y con sus elementos _label_.
-Utiliza _profile-picture_,_age_,_referrer_ y _bio_ como valores para los respectivos atributos _id_.

**Step 40**
-El _textarea_ aparece demasiado pequeno. Para darle un tamano inicial puedes agregar los atributos _rows_ y _cols_.
-Agrega un tamano inicial de 3 filas (rows) y 30 columnas (columns)

**Step 41**
-Para dara los campistas una idea de lo que deben poner en su biografia, se utiliza el atributo _placeholder_. El _placeholder_ acepta un valor de texto, que se muestra hasta que el usuario empieza a escribir.
-Dale al _textarea_ un _placeholder_ de _I like coding on the beach..._

**Step 42**

- Con envio de formularios, es útil y buena práctica proporcionar a cada elemento de la tabla de envío un atributo "name".
  Este atributo se utiliza para identificar el elemento en el envio del formulario.
  **Step 43**
- El HTML para el formulario de registro esta terminado. Ahora, podemos mejorar la apariencia. Empecemos cambiando la fuenta a Tahoma, y el tamanio de fuente a 16px.

**Step 44**
-Centra los elementos h1 y p dandoles un margin de 1em auto. Luego, alinea su texto en el center(centro) tambien.
-Recuerda que para usar dos elementos en una misma llave se lo separa por una coma y un espacio en este caso seria
H1,p {...} . Para alinear el texto usamos text-align.

**Step 45**
-Centra el elemento form, dandole un margin de 0 auto. Luego, fija su tamanio un ancho maximo de 500px , y un ancho minimo de 300 px. En medio de ese rango, permite que tenga un width de 60vw.

**Step 46**
-Elimina el border, y agrega un relleno de 2em solo en la parte superior e inferior de cada fieldset. Asegurate de eliminar el padding izquierdo y derecho.

**Step 47**
-Para dar a los elementos Fieldset un poco de separacion, seleccionalo y dales un border-bottom de 3px solid #3b3b4f (importante para serparalos entre ellos)

**Step 48**
-El borde del ultimo elemento fieldset se ve un poco fuera de lugar. Puedes seleccionar el ultimo elemento de un tipo especifico utilizando la pseudo-clase CSS "last-of-type", de esta manera: p:last-of-type{...}. Esto seleccionara el ultimo elemento p. Cree un nuevo selector que apunte al ultimo elemento fieldset y establezca su border-bottom a none.

**Step 49**
-Seria mas estetico que el texto del label apareciera encima de los elementos del formulario. Selecciona todos los elementos input,textarea y select, y haz que ocupen todo el ancho de sus elementos padre. Ademas, agrega 10px de margin a la parte superior de los elementos seleccionados. Establece los otros margenes a 0

**Step 50**
-Para que el segundo fieldset, quieres que el texto del input y el label aparezcane en la misma linea. Empieza por dar a los elementos input en el segundo fieldset una clase inline

**Step 51**
-Selecciona solo los elementos .inline y dales un width de unset. Esto eliminara la regla anterior que establece que todos los input tengan un width: 100%

**Step 52**
-Agrega un poco de espacio entre los elementos .inline y el texto del label, dando un margin dereche de 0.5em. Ademas, establece todos los demas margenes a 0.

**Step 53**
-Si te fijas bien, te daras cuenta de que los elementos .inline estan demasiado arriba en la linea. Para combatir esto, establezca la propiedad vertical-align a middle.

**Step 54**
-Para hacer que los elementos input y textarea se mezclen con el tema de fondo, establece su backround-color a #0a0a23. Luego, dales un borde de un 1px, que sea de estilo solid y sea de un color #0a0a23.

**Step 55**
-Actualmente, si escribes en los elementos input o textarea, no podras ver el texto. Ademas, su altura es demasiado pequenia para ser facil de usar. Arregla esto, esctableciendo el color a #ffffff, y estableciendo su min-height a 2em.

**Step56**
-Quieres que el elemento select siga teniendo un fondo blanco, pero ahora no tiene el mismo min-height que los elementos input y textarea. Mueve la propiedad min-height y el valor para que los tres tipos de elementos tengan el mismo valor min-height, y el select siga teniendo un fondo blanco.

**Step57**
-Para dar estilo al boton de envio puede utilizar un selector de atributos (attribute), que selecciona un elemento basado en el valor del atributo dado. Aqui hay un ejemplo:
input[name="Password"]
-Lo anterior selecciona los elementos input con un atributo name con el valor password. Ahora, utiliza el selector de atributos para dar estilo al boton de envio con un display de block, y un width de 60%.

**Step58**
-Con un display de block el boton de envio se situa al ras del bode izquierdo de su padre. Utiliza la misma tecnica utilizada para centrar el form para centrar el boton de envio.

**Step 59**
-Para que el boton de envio se vea mas en linea con el resto del formulario, dale el mismo height que los otros campos(2em). Ademas,aumenta el font-size a 1.1rem.

**Step 60**
-Para hacer que el boton de envio aparezca de forma mas distintiva, dale un background-color de #3b3b4f, y un border-color de white.

**Step 61**
-Por ultimo, para el boton de envio, si quieres separarlo del fieldset anterior, y ajustar su ancho para que nunca sea inferior a 300px. Cambia la propiedad margin para incluir 1em en la parte superior e inferior, dejando los margenes derecho y izquierdo en auto. A continuacion ajuste la anchura como se ha descrito anteriormente.

**Step 62**
-La mayoria de los navegadores inyectan sus propias propiedades y valores CSS por defecto para los diferentes elementos. Si te fijas bien, podras notar que el input de archivo es mas pequenio que los otros elementos input de texto. Por defecto, se da un padding de 1px 2px a los elementos input en los que puedes escribir. Usando otro selector de atributos, estiliza el input con un type de file para que tenga el mismos relleno que los otros elementos input.

**Step 63**

- Hablando de padding, el boton de envio se encuentra en la parte inferior del elemento form. Agrega 2em de padding solo a la parte inferior del form.

**Step 64**
-Haz que el input del texto terms and conditions sea de tipo inline aniadiendo la clase apropiada en HTML.

**Step 65**

- Por ultimo, cambia el color del texto del enlace terms and conditions a #dfdfe2 aniadiendo un nuevo selector en el codigo CSS.

_BIEN HECHO!! Ha completado la parte final del proyecto de practica del Registration Form _
