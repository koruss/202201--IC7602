# 202201--IC7602
# Kenneth Corrales Lizano 2017151342

### La red Telefonica conmutada
Originalmente fue diseñada para transmitir la voz, consiste en 3 componentes principales:
1.	Circuitos locales (cables de par trenzado que van hacia las casas y las empresas).
2.	Troncales (fibra óptica digital que conecta a las oficinas de comunicación)
3.	Oficinas de conmutación (donde las llamadas pasan de un trocal a otro)

En el pasado, la transmisión en todo el sistema telefónico era analogico, la senial se enviaba como un voltaje eléctrico entre la fuente y el destino, sin embargo, gracias al crecimiento de la fibra óptica, la electrónica digital y los computadores, los troncales pasaron a manejarse de manera digital junto con los conmutadores, sin embargo, el circuito local se mantiene con tecnología analógica. Entre los beneficios de la tecnología digital destaca que es mas sencillo de manejar a través de los amplificadores puesto que no es necesario mantener las ondas, basta con que se pueda distinguir los 1 de los 0, por ende, es más económico y sencillo.
Cuando un computador desea enviar datos digitales sobre un alinea analógica de acceso telefónico es necesario convertir primero los datos a formato analógico para transmitirlos sobre el circuito local. El modem es el que realiza esta conversión, luego se convierten a digital en la oficina central para transmitirlo posteriormente por los troncales, efectivamente si del otro lado hay un computador es necesario realizar los mismos pasos a la inversa para obtener la información.
Ahora veamos rápidamente los problemas de las líneas de transmisión:
Atenuación: es la perdida de energía conforme la señal se propaga de X a Y  la perdida se expresa en términos de db por kilometro
Ruido: se refiere a energía evidentemente no deseada, que puede llevarnos al tercer problema llamado distorsión, además debido al flujo de electrones se origina el calentamiento térmico en los cableados y finalmente el ruido de impulso que se refiere a picos de energía que puede eliminar bits en casos de redes digitales
Distorsión: muy relacionado a los anteriores, se refiere problemas en la señal que modifican el flujo de información y provocan que la información enviada desde el emisor no sea la misma a la recibida por el receptor. 


El ancho de banda de un medio es el rango de frecuencias que atraviesa al medio con atenuación mínima, se mide en Hertzios
La tasa de baudios es la cantidad demuestras por segundo que se realizan. Cada muestra envía una porción de información, es decir, un símbolo. Por lo tanto, la tasa de baudios y la tasa de símbolos significan lo mismo
Los módems avanzados utilizan una combinación de técnicas de modulación con el propósito de trasnmitir muchos bits por baudio, además permiten el trafico en ambas direcciones al mismo tiempo  (dúplex total).

#### Troncales y multiplexion. 
En FDM el espectro de frecuencia se divide en bandas de frecuencia, y cada usuario posee exclusivamente alguna banda. En TDM los usuarios esperan su turno (en round-robin), y cada uno obtiene en forma periódica toda la banda durante un breve lapso de tiempo.
FDM-> Cuando se multiplexan muchos canales juntos, se asignan 4000 Hz a cada canal para
mantenerlos bien separados. Primero se eleva la frecuencia de los canales de voz, cada uno en unacantidad diferente, después de lo cual se pueden combinar, porque en ese momento no hay dos canales que ocupen la misma porción del espectro
TDM-> Se puede manejar completamente por medio de dispositivos digitales, sin embargo esto significa que se debe de covertir la senial analógica a digital mediante el codec.

### EL Sistema Telefónico Móvil 
Los teléfonos inalámbricos se dividen 2 categorías: los inalámbricos (tienen una estación base y un teléfono que trabaja a cierto rango de este), y los celular, estos han pasado por 3 generaciones distintas (voz analógica, voz digital, y voz y datos digitales). 
Los AMPS, la región geográfica se divide en celdas razón por la que se llama “celular”, los AMPS emplean 832 canales dúplex, compuesto por dos canales simplex desde 824 hasta 849 MHz, y 832 canales de recepción símplex desde 869 hasta 894 MHz. Cada uno de estos canales simplex es de 30 kHz de ancho; por lo tanto, AMPS usa FDM para separar los canales.
Los canales se dividen en cuatro categorías: 

1. Control (base a móvil) para administrar el sistema.
2. Localización (base a móvil) para avisar a usuarios móviles que tienen llamadas.
3. Acceso (bidireccional) para establecimiento de llamadas y asignación de canales.
4. Datos (bidireccional) para voz, fax o datos.
   
Si bien el D-AMPS es usado en EU y Japón, a nivel mundial se utiliza un sistema llamado GSM al igual que el D-AMPS utiliza multiplexión por división de frecuencia, los canales GSM son más anchos en comparación por lo tanto la tasa de datos por usuarios es mayor. El GSM tiene 124 pares de canales simplex de 200kHz, los radios GSM no pueden transmitir y recibir al mismo tiempo.
CDMA (Acceso Múltiple por división de código). En lugar de dividir el rango de frecuencia permitida en algunos cientos de canales estrechos, CDMA permite que cada estación transmita todo el tiempo a través de todo el espectro de frecuencia. Se utiliza la teoría de codificación para separar múltiples transmisiones simultáneas. CDMA no supone que las tramas que colisionan son totalmente distorsionadas. En su lugar, asume que se agregan múltiples señales en forma lineal.  Cada tiempo de bit se divide en M intervalos cortos llamados chips. Por lo general, hay 64 o 128 chips por bit.
Entre los sistemas 2.5 G se pueden mencionar el EDGE (Tasa de Datos Mejorada para la Evolución del GSM), que simplemente es GSM con más bits por baudio lo cual conlleva tanto a mejoras como a mayores problemas. EL GPRS que permite que las estaciones móviles envíen y reciban paquetes IP en una celda que se ejecuta en un sistema de voz.

### Televisión por cable 

Inicialmente llamada como televisión por antena comunal era una antena en una montaña con amplificadores que enviaban cableado a las casas. Eventualmente debido al crecimiento de este sistema los cables se empezaron a cambiar por fibra de ancho de banda alto HFC (Red Híbrida de Fibra Óptica y Cable Coaxial). Como la fibra posee mucho ancho de banda esta puede alimentar varios coaxiales.
El acceso al internet requiera un modem de cable es decir un dispositivo que tiene dos interfaces uno en el computador y otro en la red de cable.Al inicio habían muchas variaciones con respecto a los cables sin embargo posterior se adoptó el estándar DOCSIS. 
Ahora bien, el ADSL utiliza cable de par trenzado, en comparación con el cable existe un debate entre cual es mejor ya que si bien el cable es más veloz, se pierde mucho de ese poder en el envio de la información de los canales de TV. Además, la disponibilidad es otro tópico, no todos tienen cable sin embargo si ud si lo tiene conseguir internet es sencillo.
La conclusión es que ADSL y el cable son tan parecidos como diferentes. Ofrecen servicios
comparables y, conforme la competencia entre ellos se avive más, probablemente precios comparables.
