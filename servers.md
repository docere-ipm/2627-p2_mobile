# 🏉🏒🥅⚽ APIS Públicas Deportivas (Datos Reales)

A continuación se lista una selección de servicios API para consultar
información deportiva, organizados de menor a mayor complejidad de
configuración. La lista no es exhaustiva, puedes elegir uno o varias
de las opciones mostradas o alguna otra que no se muestra aquí.


## 1. TheSportsDB (datos reales sin registro)

Es una base de datos multideporte colaborativa tipo wiki. Es una opción
rápida e intuitiva.

  * **Tipo de API:** REST / JSON.
  
  * **Gratuita / Coste:** 100% Gratuita para desarrollo y educación.
  
  * **Autenticación:** **No requiere registro ni, API Key** para
    pruebas de desarrollo (utiliza la clave de pruebas pública).
  
  * **Formatos de respuesta:** JSON con resultados de partidos, ligas,
    equipos, eventos en vivo y escudos/imágenes.
  
  * **Ejemplo de petición directa:**
  
```text
# Obtener los próximos eventos de la liga id=4328
https://www.thesportsdb.com/api/v1/json/3/eventsnext.php?id=4328

```

  * **Ventaja:** Cero configuración inicial,



## 2. Football-Data.org (datos profesionales de fútbol)

API enfocada exclusivamente al fútbol profesional (LaLiga, Premier
League, Champions League, etc.) con estadísticas en tiempo real.

  * **Tipo de API:** REST / JSON.
  
  * **Gratuita / Coste:** Plan gratuito holgado (hasta 10
    peticiones/minuto, adecuado para la app móvil).
  
  * **Autenticación:** Requiere registro gratuito para obtener un
    *Token* (`X-Auth-Token` en la cabecera HTTP).
  
  * **Formatos de respuesta:** Marcadores en directo, clasificaciones,
    resultados históricos y detalles de equipos.


  * **Ventaja:** Aporta un nivel de realismo avanzado y permite probar
    escenarios complejos de sincronización de datos.



## 3. API-Sports / API-Football (vía RapidAPI)

Una de las APIs más completas del mercado para múltiples deportes
(fútbol, baloncesto, fórmula 1, béisbol).

  - **Tipo de API:** REST / JSON.
  
  - **Gratuita / Coste:** Plan gratuito de 100 peticiones diarias.
  
  - **Autenticación:** Requiere registro gratuito en RapidAPI para
    obtener la `X-RapidAPI-Key`.
  
  - **Formatos de respuesta:** Datos extremadamente detallados
    (estadísticas de jugadores, alineaciones, cuotas, incidentes
    minuto a minuto).



---

# 🛠️ Alternativas Simuladas (Mocks en la Nube de "Cero Configuración")

También existen herramientas que nos permiten simular el
comportamiento de un servidor real y son útiles para evitar los
límites de peticiones de las APIs reales o para controlar las
respuestas durante la ejecución de las pruebas.


## 4. JSONPlaceholder / My-JSON-Server (by Typicode)

Permite subir un archivo `db.json` con los datos de partidos simulados
al propio repositorio de GitHub de la aplicación y convertirlo al
instante en un servidor REST en la nube.

  - **Tipo de API:** REST completa (soporta `GET`, `POST`, `PUT`, `DELETE`).
  
  - **Gratuita / Coste:** 100% Gratuita.
  
  - **Autenticación:** **Sin autenticación.**
  
  - **Ventaja:** Cero mantenimiento. Escribes tus propios partidos de
    prueba en un archivo JSON en GitHub y obtienes una URL pública tipo
    `[https://my-json-server.typicode.com/usuario/repo/eventos](https://my-json-server.typicode.com/usuario/repo/eventos)`.

  - **Ventaja:** Control absoluto sobre la estructura de los datos.


## 5. Mockapi.io

Plataforma visual online para crear endpoints de prueba en pocos
clics.

  - **Tipo de API:** REST / JSON.
  
  - **Gratuita / Coste:** Plan gratuito con hasta 1 proyecto y
    múltiples recursos.
  
  - **Autenticación:** **Sin autenticación para las peticiones de la app.**
  
  - **Ventaja:** Permite generar datos aleatorios de deportes
    fácilmente y emular retardos de red (*latency*) para probar los
    estados de carga en Flutter.





