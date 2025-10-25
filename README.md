## Gestión de Pilas y Colas con POO + Simulación de Navegador e Impresora

Este proyecto implementa estructuras de datos Pila (LIFO) y Cola (FIFO) utilizando Programación Orientada a Objetos (POO) en Python. Además, incluye dos simulaciones prácticas:

Navegador Web → Usa pilas para ir Atrás y Adelante entre páginas.

Impresora Compartida → Usa una cola para gestionar documentos en espera de impresión.

## Estructuras Implementadas
## 1. Clase Pila (Pila)

Representa una estructura LIFO (Last In, First Out).

Método	Descripción
apilar(elemento)	Agrega un elemento a la parte superior.
desapilar()	Retira el último elemento ingresado.
cima()	Devuelve el elemento superior sin eliminarlo.
esta_vacia()	Verifica si la pila está vacía.
mostrar()	Muestra los elementos de la pila.

## Uso real: Historial de navegación del navegador.

## 2. Clase Cola (Cola)

Representa una estructura FIFO (First In, First Out).

Método	Descripción
encolar(elemento)	Agrega un elemento al final de la cola.
desencolar()	Retira el primer elemento agregado.
frente()	Devuelve el primer elemento sin retirarlo.
esta_vacia()	Verifica si la cola está vacía.
mostrar()	Muestra los elementos en espera.

## Uso real: Sistema de impresión compartida.

## Simulaciones Incluidas
A. Navegador Web (NavegadorWeb)

Utiliza dos pilas:

atrás → Guarda las páginas anteriores.

adelante → Guarda las páginas que se pueden restaurar.

actual → Página que se está visualizando.

Comandos clave:

Acción	Método
Visitar una página	navegar("pagina")
Retroceder	ir_atras()
Adelantar	ir_adelante()
## B. Impresora Compartida (ImpresoraCompartida)

Utiliza una cola para almacenar documentos en espera.

Acción	Método
Enviar documento	agregar_documento("archivo")
Imprimir	imprimir()
Ver documentos en espera	mostrar_cola()
## Ejemplo de Ejecución (Incluido en el Código)
nav = NavegadorWeb()
nav.navegar("Google")
nav.navegar("YouTube")
nav.ir_atras()
nav.ir_adelante()

imp = ImpresoraCompartida()
imp.agregar_documento("Trabajo.pdf")
imp.imprimir()
