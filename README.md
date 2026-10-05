## Disección de un Campo Profundo MultiLongitud de Onda

Al observar una región específica del cielo —en este análisis, un campo ecuatorial centrado en las coordenadas **RA: 135.5°, Dec: 0.5°** con un radio de $0.5^\circ$— se obtiene una estructura tridimensional compleja. En un mismo parche del firmamento coexisten fuentes de naturaleza muy diversa: desde estrellas locales pertenecientes a la Vía Láctea, hasta galaxias distantes y cuásares impulsados por agujeros negros supermasivos.

Para clasificar cada fuente luminosa y caracterizar la región de forma integral, se requiere la combinación de diferentes longitudes de onda y catálogos astronómicos.
A continuación, se presenta la integración de los resultados de ambos pipelines de procesamiento y el análisis físico que fundamenta este enfoque multilongitud de onda.

## 1. Integración del Espectro Óptico e Infrarrojo para una Visión Completa del Universo

El estudio del universo mediante una sola región del espectro electromagnético ofrece una visión sesgada o incompleta. Integrar datos ópticos (como Gaia, $G$) con datos infrarrojos (como AllWISE, $W_1$) es fundamental por tres razones físicas principales:

* **Extinción y Dispersión por Polvo Interestelar:** El gas y el polvo presentes en los medios de formación estelar, discos protoplanetarios, núcleos galácticos y toros de cuásares dispersan y absorben eficientemente la radiación en longitudes de onda cortas (óptico/UV). Debido a que la dispersión disminuye inversamente con la longitud de onda, la radiación infrarroja logra atravesar estas densas nubes de polvo. Sin la banda infrarroja, estos objetos permanecerían completamente ocultos u oscurecidos.
* **Corrimiento al Rojo Cosmológico ($Redshift, z$):** La luz emitida en el óptico o ultravioleta por fuentes extremadamente lejanas (como cuásares primitivos o galaxias lejanas) viaja a través de un espacio-tiempo en expansión. Durante su trayecto, su longitud de onda se estira hasta llegar a la Tierra desplazada hacia el infrarrojo. El óptico por sí solo no permite detectar estos objetos con alto $redshift$.
* **Poblaciones de Objetos Fríos y Térmicos:** Objetos de baja temperatura —como enanas rojas, enanas marrones, estrellas en formación y envolventes de polvo circunestelar— emiten la mayor parte de su radiación en el infrarrojo. Un catálogo estrictamente óptico subestimaría masivamente estas poblaciones dentro del campo profundo.

---

## 2. Complementariedad entre Gaia (Astrometría/Cinemática) y SDSS (Espectroscopía)

Para resolver la ambigüedad de un punto de luz puntual y determinar si se trata de una estrella cercana de la Vía Láctea o de un Cuásar (Agujero Negro Supermasivo activo) a distancias cosmológicas, se combinan los datos astrométricos de Gaia con los espectroscópicos de SDSS (SkyServer).

### Gaia: Astrometría y Cinemática
Gaia analiza el comportamiento geométrico y el movimiento del objeto en el plano del cielo:

* **Paralaje ($\varpi$):** Mide la distancia geométrica. Una estrella dentro de la galaxia presentará un paralaje medible ($\varpi > 0.05\text{ mas}$). Para un cuásar a miles de millones de años luz, el paralaje es físicamente nulo ($\varpi \approx 0\text{ mas}$, dentro del margen de ruido instrumental).
* **Movimiento Propio ($\mu$):** Mide la velocidad angular en el plano del cielo. Las estrellas cercanas muestran un desplazamiento detectable a lo largo de los años ($\mu > 0\text{ mas/año}$). Un cuásar está tan distante que su movimiento en el cielo es imperceptible ($\mu \approx 0\text{ mas/año}$), sirviendo incluso de punto de referencia inercial fijo en el cielo.

### SDSS (SkyServer): Espectroscopía y Perfil Electromagnético
Mientras Gaia analiza el movimiento angular, SDSS descompone la luz del objeto para analizar su física interna:

* **Redshift Espectroscópico ($z$) y Velocidad Radial:** A diferencia del movimiento propio en el cielo, la velocidad de alejamiento radial se mide mediante el desplazamiento hacia el rojo de las líneas espectrales en SDSS. Un $redshift$ elevado ($z > 0.1$) confirma inequívocamente que la fuente se encuentra fuera de nuestra galaxia.

| Parámetro / Herramienta | Estrella Cercana (Vía Láctea) | Agujero Negro Supermasivo / Cuásar |
| :--- | :--- | :--- |
| **Paralaje ($\varpi$) [Gaia]** | Detectable ($\varpi > 0.05\text{ mas}$) | Nulo ($\varpi \approx 0\text{ mas}$) |
| **Movimiento Propio ($\mu$) [Gaia]** | Detectable ($\mu > 0\text{ mas/año}$) | Inexistente ($\mu \approx 0\text{ mas/año}$) |
| **Redshift ($z$) [SDSS]** | Compatible con $z \approx 0$ | Elevado ($z \gg 0$) |

### Veredicto Combinado
Un objeto puntual en el cielo que muestre paralaje y movimiento propio **nulos en Gaia**, combinado con un espectro en **SDSS** dominado por líneas de emisión anchas con un **alto corrimiento al rojo ($z$)**, queda categorizado sin ambigüedad como un **cuásar distante** y no como una estrella de la Vía Láctea.
