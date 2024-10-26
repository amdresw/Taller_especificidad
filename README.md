Taller de especificidad

Objetivo:
El objetivo del taller es que los participantes comprendan cómo funciona la especificidad en CSS y
aprendan a utilizarla de manera efectiva para resolver conflictos de estilos.


Parte 1: Introducción Teórica a la Especificidad

¿Qué es la especificidad?
La especificidad es un cálculo utilizado en CSS para decidir qué estilos aplicar a un elemento cuando hay conflictos entre diferentes reglas. El navegador utiliza esta medida para determinar cuál de las reglas tendrá prioridad, siguiendo un conjunto de puntos de acuerdo al tipo de selector utilizado.

La cascada en CSS decide el orden en que se aplican los estilos: primero los del navegador, luego los del usuario, y finalmente los del autor. Cuando varias reglas coinciden, se aplicará la regla con mayor especificidad o, si tienen la misma especificidad, la última en aparecer en el CSS.
Reglas de cálculo de especificidad

Selectores de ID: tienen un valor de 100 puntos.
Selectores de clase, atributos y pseudoclases (por ejemplo, :hover): asignan 10 puntos.
Selectores de elementos y pseudoelementos (como ::before y ::after): dan 1 punto.
La propiedad !important tiene la máxima prioridad, sobrescribiendo cualquier otra regla, independientemente de la especificidad.

Parte 2: Ejemplos Prácticos 
1. Ejemplo básico:
Demuestra cómo los diferentes selectores afectan la especificidad.


![styleRED](https://github.com/user-attachments/assets/2afac4e1-53ee-42c1-bffd-02f2e02815fe)


![Indexred](https://github.com/user-attachments/assets/c838cca4-91fe-4ffe-99a2-62c2269429bb)


El color del texto es rojo porque el selector de ID tiene prioridad sobre los selectores de clase y de etiqueta debido a su mayor especificidad.

3. Demostración de !important :
   
![styleblue](https://github.com/user-attachments/assets/5da5c6d4-6f80-412e-b5cf-bb6e8434adcc)


![indexblue](https://github.com/user-attachments/assets/cef991e7-cdfd-4c9b-8023-fc782324c739)


El color es azul, ya que !important tiene la máxima prioridad, sin importar la especificidad de otros selectores.

Parte 3: Ejercicios Prácticos

Ejercicio 1: Calculando la Especificidad

Dado el siguiente código, pide a los participantes que calculen la especificidad y determinen qué
estilos se aplicarán:


![image](https://github.com/user-attachments/assets/1d9bfa72-a150-4fed-95ff-21b1d8829c00)


Pregunta:

¿Qué color tendrá el título "h1" ?

- El título "h1" será rojo porque el selector ID tiene la mayor especifidad

Ejercicio 2: Resolviendo Conflictos de Especificidad

Modifica el siguiente código para que el párrafo tenga color amarillo, sin usar !important .
rta/


![image](https://github.com/user-attachments/assets/cccdd5aa-0032-4aab-b471-ea84d4c835b4)



Parte 4: Desafío Final 

Desafío: Diseñando una Página Completa con Estilos Conflictivos

Dales a los participantes un archivo HTML con múltiples elementos y clases, y pídeles que
agreguen estilos CSS para lograr un diseño específico. Deberán aplicar todo lo aprendido sobre
especificidad para resolver los conflictos y obtener el resultado correcto.


![image](https://github.com/user-attachments/assets/5eb863e6-3429-4d7a-aacd-a976c9a15f39)


Desafío CSS:

-El "h1" en el .header debe ser de color blanco. 

-El texto del "p" en .content debe ser rojo.

-El texto del "footer" debe ser gris.

![image](https://github.com/user-attachments/assets/fb1e2e1c-69b5-4ede-ad5f-849debb43d19)

![image](https://github.com/user-attachments/assets/72dddba8-ce91-4a44-92a0-0c392e3d89ea)



