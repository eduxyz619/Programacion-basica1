## Programacion-basica1
python

----
# Garcia Alcantara Eduardo
# Tutorial de Python.

### Que es Anaconda?
![Anaconda_Logo](https://user-images.githubusercontent.com/52559127/60705355-8eee2700-9ecc-11e9-9047-74890250b61b.png)

Anaconda es un distribucion libre y abierta de los lenguajes Python, utilizada en ciencia de datos, y aprendizaje automotico. Esto incluye procesamiento de grandes volumenes de informacion, analisis predictivo y computos cientificos. Esta orientado a simplificar el despliegue y administracion de los paquetes de software.


#### Instalacion de Anaconda.

Python en una computadora es bastante sencillo de intalar, en este caso en la escuela en donde tome el curso utilizamos Anaconda que es una distribucion de python. Aunque solo esta disponible en su idioma natal que es el ingles, esta distribucion incluye multitud de utilidades que nos facilitaron el trabajo y es ideal para empezar la programacion ya que su diseno y su forma de interactuar es muy sencilla. Para instalar, solo tienes que descargar la version de Anaconda Python que sea compatible con tu sistema operativo este se realiza desde la misma web de Anaconda Python.

Una vez instalado, sigue los siguientas pasos:

    >1. Abrir el buscador de tu computador.
    >2. Abrir la carpeta "Anaconda(64-bits)".
    >3. Hacer click en "Anaconda Prompt" o "Spider" que son los dos compiladores que anaconda maneja.
    
![python](https://user-images.githubusercontent.com/52559127/60709697-b0541080-9ed6-11e9-98f5-58299533029c.PNG)
    

### Operadores

TIPOS DE DATOS BASICOS...

En python los tipos de datos basicos se dividen en diferentes tipos de datos como pueden ser el numero 3 (entero o integer), el numero 1.55 (punto flotante o float) y tambien tiene la posibilidad de hacer un numero 2+j (complejos o complex).

Para poder conocer el tipo de dato de una variables usaremos la instruccion type"()".
Otro tipo de dato basico en PYTHON son las cadenas de texto, por ejemplo, "Buenas noches"(cadena de texto o string).

Como se puede notar a diferencia de muchos otros lenguajes de programacion en PYTHON no se declara el tipo de variable al crearla.

Para resumir en PYTHON se puede representar numeros enteros, reales, y complejos. Los numeros enteros son aquellos numeros positovos o negativos que no tienen desimales. En la mayor parte de las maquinas las variables enteras ("int") pueden almacenar numeros de -2^31 a 2^31 en una plataforma de 32 bits y en plataformas de 64 bits el rango es de -2^63 a 2^63.

Los numeros flotantes son los que cuentan con decimales. En PYTHON se expresan mediante el tipo "float" se puede representar numeros desde -2^64 a 2^64.

Los numeros complejos son aquellos que tienen una parte imaginaria. Para definir una variable compleja se utiliza en termino "complex".

   
![operadores](https://user-images.githubusercontent.com/52559127/60710358-1f7e3480-9ed8-11e9-9324-032e394ecdbe.PNG)


Un ejemplo de esto puede ser el siguiente:

    print('Programa para calcular area')
    Largo=float(input('Ingresa el largo de la habitacion:'))
    Ancho=float(input('Ingrese el ancho de la habitacion:'))


    print('El Largo de tu habitacion es:', Largo, 'metros','\n',
    'El ancho de tu habitacion es:' ,Ancho,'metros','\n', 
    'El area de tu habitacion es:',Largo*Ancho,'metros cuadrados')
    
![ejemplo ope](https://user-images.githubusercontent.com/52559127/60710934-5e60ba00-9ed9-11e9-995e-f649542e58ff.PNG)

   

### Ciclo For.
En pyhton "for" se le conoce como un ciclo que se repidete hasta un cierto numero de n veces, lo que lleva a que alguna operacion se repitar el numero de veces que se a puesto en el ciclo.

            variable = secuencia  
            secuencia = ["uno", "dos", "tres"]  //estos son elementos
            for elemento in secuencia:
            ____print(elemento)                //4 esopacios 

Y los resultados seran:

           uno
           dos
           tres

Lo que se observa en lo anterior es que se declara un rango que sera lo que se repita.

Un ejemplo del ciclo "for" puede ser el siguiente:

    for precio in range(4,201,5):
    precio=(precio+0.95)
    descuento = (precio*0.60)
    preciof=(precio-descuento)
    print(precio,'$','|',"{:.2f}".format(descuento),'|',"{:.2f}".format(preciof,'$'))

![ejemplo for](https://user-images.githubusercontent.com/52559127/60711508-b946e100-9eda-11e9-8b93-c80af2f47c4e.PNG)


### Modulo Turlte 
Hay muchos modulos en python que proveen caracteristicas muy utiles que podemos usar en nuestros propios programas. Algunos de estos tienen la funcion de enviar correos electronicos y algunos de estos pueden extraer y guardar informacion de paginas de webs. Para el manejo de graficos usaremos un modulo que permite crear figuras y patrones. El modulo que se usara permiten desarrollar nuestro pensamiento y aplicarlo en algun proyecto que se tenga.

Un ejemplo del modulo Turtle puede ser:

     import turtle
     ventana=turtle.Screen()
     alex=turtle.Turtle()
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     ventana.mainloop()
     
![ejemplo turtle](https://user-images.githubusercontent.com/52559127/60712750-53a82400-9edd-11e9-99a1-4ad3821f887c.PNG)
     

Tambien con este modul existe la posibilidad de ponerle una figura en lugar de una flecha y tambien se puede elegir el color del fondo que uno quiera.

    a=input('Escoje un color de los siguientes para la ventana: brown chocolate 
    coral red pink purple blue green yellow black :')

    import turtle
    ventana=turtle.Screen()
    ventana.bgcolor(a)
    ventana.title("wassa")

    kary=turtle.Turtle()
    kary.shape("turtle")
    kary.color("blue")
    kary.pensize(10)
    kary.forward(100)
    kary.left(120)
    kary.forward(100)
    ventana.mainloop() 
    
    
![turtle color](https://user-images.githubusercontent.com/52559127/60713188-36278a00-9ede-11e9-8e41-604075b6be2d.PNG)


Con este modulo se puede realizar tambien circulos o diferentes formar, por ejemplo:  

    
    import turtle

    def dibujar_cuadro(tur,d):
    for i in range(4):
        tur.forward(d)
        tur.left(90)

    ventana=turtle.Screen()
    ventana.bgcolor("red")
    ventana.title("salvenme")

    loki=turtle.Turtle()
    tobillo=turtle.Turtle()
    dibujar_cuadro(loki, 50)
    dibujar_cuadro(tobillo, 200)

    ventana.mainloop()
    
![ejemplo tur1](https://user-images.githubusercontent.com/52559127/60713600-0331c600-9edf-11e9-86ae-b4b8f904d69d.PNG)
    


El modulo turtle tiene una funcion algo perculiar que pueda hacer que una imagen se mueve en una ventana y un ejemplo de esto es el siguiente:

   
    import turtle 

    ventana = turtle.Screen()
    ventana.setup(500,500)
    ventana.tracer(0)
    ventana.addshape("mario_frog_render_2.gif")


    mario = turtle.Turtle()
    mario.speed(100000)
    mario.shape("mario_frog_render_2.gif")

    mario.penup()
    mario.goto(-350,0)

    while True :
    ventana.update()
    mario.forward(0.01)

    ventana.mainloop()
    
![mario move](https://user-images.githubusercontent.com/52559127/60713988-b4386080-9edf-11e9-9061-2851a1368e44.PNG)
    
    
### Funciones 

Una funcion es un fragmento de codigo con un nombre asociado que realiza una serie de tareas y devuelve un valor. Ademas de ayudarnos a programar y depurar dividiendo el programa en partes, las funciones tambien permiten reutilizar codigo sin nosotros utilizar demasiadas lineas.
     
	##definicion de una funcion
	def sonido():
	    print('click, click')
	##cuerpo principal del programa
	sonido()
  
Las Funciones ayudan al programador a dividir un problema en pequenas piezas que pueden ser reutilizadas. Tambien ayudan al programador a concentrarse en una pequena parte del programa a la vez. Como resultado el escribir funciones es una parte importante del desarrollo del sofware. 

En nuestro caso debemos aprender a:

	1. Definir una funcion para usarla despues.
	2. Pasar uno o mas valores a una funcion.
	3. Desarrollar un calculo complejo en una funcion.
	4. Regresar uno o mas resultados a una funcion.
	5. Llamar a una funcion que previamente hayamos definido.

Puede tambien colocarce el Modulo Turtle con algunos de los ciclos, como se muestra este, con Ciclo For:

    import turtle
    def dibujar_cuadro(tur,d):
    for i in ['red','purple','blue','yellow']:
        tur.color(i)
        tur.forward(d)
        tur.left(90)

    ventana=turtle.Screen()
    ventana.bgcolor("black")
    ventana.title("salvenme")

    loki=turtle.Turtle()
    tobillo=turtle.Turtle()
    dibujar_cuadro(loki, 50)
    dibujar_cuadro(tobillo, 200)

    ventana.mainloop()
    
![tur color](https://user-images.githubusercontent.com/52559127/60714815-6290d580-9ee1-11e9-8112-6719791c80df.PNG)
    

Incluso, con el mismo ciclo, puedes cambiar el angulo y el tamano de las figuras.


    import turtle

    def dibujar_multiples_cuadros(tur,d):
    for i in ['red','purple','hotpink','blue']:
        tur.color(i)
        tur.forward(d)
        tur.left(90)

    ventana = turtle.Screen()
    ventana.bgcolor('black')
    ventana.title('funciones')

    alex= turtle.Turtle()
    alex.pensize(3)

    d= 20
    for i in range(15):
    dibujar_multiples_cuadros(alex,d)
    d= d + 10
    alex.forward(10)
    alex.right(18)


    ventana.mainloop()
    
![cuadro en aumen](https://user-images.githubusercontent.com/52559127/60715119-ee0a6680-9ee1-11e9-9d76-932cae8e292b.PNG)
    

Tambien es capaz de realizar una secuencia de cuadro del mismo tamano pero separados:

    import turtle


    def dibujar_cuadro_seguir(tur, p):
    for i in range(4):
        tur.forward(20)
        tur.left(90)
    

    ventana=turtle.Screen()
    ventana.bgcolor('black')
    ventana.title('funciones')

    alex=turtle.Turtle()
    alex.pencolor('white')
    alex.pensize(5)
    alex.speed(2)

    p=30

    for i in range(5):
    dibujar_cuadro_seguir(alex, 5)

    alex.penup()
    alex.setpos(p,0)
    alex.pendown()
    p=p+30

    ventana.mainloop()
    
![cuadro cuadri](https://user-images.githubusercontent.com/52559127/60715335-6113dd00-9ee2-11e9-9424-cbb008a34f7f.PNG)
    
Como se muestra este modulo es capaz de realizar cualquier clase de figura, cualquier secuencia de la misma
y tambien el aumento o decremento de la misma, es un modulo muy util al que su unica limitante es al
imaginacion del programador.


### Programacion Ambientada a Objetos.

Al principio del curso se comento que Python es un lenguaje multiparadigma en el que se podia trabajar con programacion estructurada, como vio en los ejemplos anteriores o con programacion orientada a objetos el cual es muy util para la programacion ya que esto nos ayuda a realizar un programa mas especializado, utlizando un numero menor de lineas de codigo 
ya que se pueden utilizar unos terminos llamasdos: objetos y clases.

#### OBJETOS:

Un objetos es una entidad que agrupa un estado y una funcionalidad relacionada. El estado del objeto se define a traves de variables llamadas atributos.



#### CLASES:

Una clase no es mas que una plantilla pueden ser definidos uno o mas objetos, al referirse a clase se puede agrupar datos que van a pertenecer a la clase principal.
Esto se podria entender como un arbol y sus consecuentes ramas.

Por ejemplo:

    class Coche(object):
        def __init__(self,gasolina):
            self.gasolina = gasolina
        def arrancar(self):
            if self.gasolina > 0:
                print('Arranca')
            else:
                print('No Arranca')
        def conducir(self):
            if self.gasolina > 0:
                self.gasolina = self.gasolina - 1
                print('Quedan ', self.gasolina,' litros')
            else:
                print('No se mueve')
    vocho = Coche(5)
    tsuru = Coche(3)

    vocho.arrancar()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir() 
    
![clases vocho](https://user-images.githubusercontent.com/52559127/60715968-dfbd4a00-9ee3-11e9-8856-b304a49fc481.PNG)
    

Pero no solo puedes poner algo en com�n, como un carro, si no tambi�n puedes hacer que el programa detecte si es o no, una figura, como por ejemplo un triangulo.

    class Triangulo(object):
        def __init__(self,angulo1,angulo2,angulo3):
            self.angulo1 = angulo1
            self.angulo2 = angulo2
            self.angulo3 = angulo3
        def ChecarAngulo(self):
            if self.angulo1+self.angulo2+self.angulo3 == 180:
                print('Es un triangulo')
            else:
                print('No es un triangulo')
    miTriangulo=Triangulo(90,30,60)
    miTriangulo.ChecarAngulo()

![clas tri](https://user-images.githubusercontent.com/52559127/60716097-2ad75d00-9ee4-11e9-8cc5-adffc039c254.PNG)

Como conclusion se llega a que python es una herramienta muy versatil que la pueden utilizar desde los principiantes
hasta los programadores mas avanzador, ya que su versatilidad es muy buena ademas de que es multiplataforma y eso es lo que lo hace destacar ademas de que la comunidad de python siempre esta trabajando en actualizaciones y en funciones para facilitar 
el trabajo a realizar.
