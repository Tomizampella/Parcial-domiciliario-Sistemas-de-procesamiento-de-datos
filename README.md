# Parcial domiciliario Sistemas de procesamiento de datos
[![Arduino-Tinkercad-portada.jpg](https://i.postimg.cc/Y0BGdzHs/Arduino-Tinkercad-portada.jpg)](https://postimg.cc/wyFjvJ3X)


## 📌 Integrantes 
- Tomás Diaz Zampella
- Matias Ariel Espinoza 


## 📡 Proyecto: Contador de 0 a 99 con Display 7 Segmentos.
[![3-Parcial-Domiciliario-Tom-s-Diaz-Zampella-Matias-Ariel-Espinoza.png](https://i.postimg.cc/mZ977tsn/3-Parcial-Domiciliario-Tom-s-Diaz-Zampella-Matias-Ariel-Espinoza.png)](https://postimg.cc/3WKyTrWj)


## ✒️ Descripción
El proyecto tiene como objetivo principal controlar dos displays de siete segmentos y mostrar los dígitos en cada display mediante multiplexación.
Si la temperatura exdece los 60°, está programado para que el sistema deje de funcionar.
Si el valor obtenido de la fotoresistencia excede las 200 unidades, los displays se apagan. En este caso, el sistema sigue funcionando.

## 💻 Función principal
Esta función se encarga de encender y apagar los displays.

Recibe por parámetros el valor que se tiene que mostrar en el primer y segundo display,
el valor que recibe está en el rango de 0-9. Envía los valores a cada segmento para formar el valor recibido,
se prende el primer display por 10 milisegundos y se apaga para prender el segundo display.
Esto último se conoce como multiplexación.


~~~ C (lenguaje en el que esta escrito)
void cambiarDigito(int primerDisplay, int segundoDisplay)
{
  displayNumero(primerDisplay);
  prenderDisplay(0,1);
  delay(10);
  displayNumero(segundoDisplay);
  prenderDisplay(1,0);
  delay(10);
}
~~~

## 📎 Links al proyecto
- [PARTE 1](https://www.tinkercad.com/things/3eQHxpzXkG3-1-parcial-domiciliario-tomas-diaz-zampella-matias-ariel-espinoza/editel?sharecode=ypSkFAlVxz8CCWkG6LcxyhHqFCc8SA8E3nBFIqH_juo)
- [PARTE 2](https://www.tinkercad.com/things/idQBzp1n4vG-2-parcial-domiciliario-tomas-diaz-zampella-matias-ariel-espinoza/editel?sharecode=g2ZjkiPr0eq47HCZ0P13pLaRjIu89JchjH5iNrXDOg0)
- [PARTE 2 - MOTOR AFICIONADO](https://www.tinkercad.com/things/gtn53DXg2BA-motor-aficionado-2-parcial-domiciliario-matias-ariel-espinoza/editel?sharecode=VCqBtgo1uCyS3OyJ7Qv2V1KCP6h1yZ9XqhlZ7octDWY)
- [PARTE 3](https://www.tinkercad.com/things/3CbquSdnm1W-3-parcial-domiciliario-tomas-diaz-zampella-matias-ariel-espinoza/editel?sharecode=iCiOI8Y6yOOQxm8MKAIgOLWcLuSvbvYoXor7xEbxtDQ)

## 📚 Fuentes
- [DOCUMENTACION DE GITHUB](https://docs.github.com/es/enterprise-cloud@latest/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [DOCUMENTACION DE C++](https://www2.eii.uva.es/fund_inf/cpp/temas/1_introduccion/introduccion.html)



