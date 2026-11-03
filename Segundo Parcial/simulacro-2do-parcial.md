# Simulacro del 2º Parcial (sin fecha)

[Enunciado original (Word)](Aula%20Virtual/Simulacro%202do%20Parcial.doc) · Temas: fuerza entre hilos y sobre una carga, fem en una bobina con B(t), energía y longitud de un solenoide, espira circular vs. espira cuadrada, bobina real con capacitor para corregir el factor de potencia.

Cada ejercicio tiene un botón **Solución** con la respuesta y, adentro, un botón **Solución paso a paso**. No hay resolución oficial de este examen: las soluciones son propias.

Volver al [índice de parciales](README.md).

La condición mínima para aprobar es haber resuelto correctamente el 50% de los problemas.

---

### Ejercicio 1

Dos conductores rectilíneos muy largos se encuentran ubicados paralelos al eje z, y a una distancia D=15 cm entre sí. Por ellos circulan corrientes de igual valor I. Los conductores se atraen con una fuerza por unidad de longitud de 2,5 N/m.
**a)** Determinar si las corrientes son paralelas o antiparalelas. Justificar.
**b)** Calcular I.
**c)** En un dado instante, una carga q=2 μC con velocidad **v** = 7,5 x 10<sup>5</sup> m/s **j** se encuentra ubicada a la izquierda del primer conductor, a distancia d=8 cm. Determinar la fuerza neta ejercida sobre la carga q (en módulo, dirección y sentido).

<details>
<summary><b>Solución</b></summary>

<details>
<summary>Solución paso a paso</summary>

**Paso 1 — Paralelas o antiparalelas (ítem a).** El hilo 1 genera en el hilo 2 un campo $B_1 = \mu_0I/(2\pi D)$. La fuerza sobre un tramo $\ell$ del hilo 2 es $\vec F = I\vec\ell\times\vec B_1$. Con corrientes del **mismo sentido** esa fuerza apunta hacia el hilo 1. Como se atraen, las corrientes son **paralelas**.

**Paso 2 — Valor de I (ítem b).**

$$\frac{F}{\ell} = \frac{\mu_0I^2}{2\pi D} \quad\Rightarrow\quad I = \sqrt{\frac{2\pi D\,(F/\ell)}{\mu_0}} = \sqrt{\frac{0{,}15\cdot2{,}5}{2\times10^{-7}}}\ \text{A} = 1369\ \text{A}$$

**Paso 3 — Geometría (ítem c).** Los hilos están sobre el eje x: el hilo 1 en $x = 0$ y el hilo 2 en $x = D$, ambos con corriente en $+\hat k$. Como el sentido no está dado, se elige así; abajo se ve que no cambia el resultado. La carga está en $x = -d$, sobre el eje x.

**Paso 4 — Campo en la carga.** Para un hilo según $\hat k$, $\vec B = \dfrac{\mu_0I}{2\pi r}\hat\varphi$. En un punto a la izquierda del hilo ($-\hat x$ desde el hilo), $\hat\varphi = \hat k\times(-\hat x) = -\hat y$. Los dos hilos están a la derecha de la carga, así que los dos dan campo en $-\hat y$:

$$\vec B = -\frac{\mu_0I}{2\pi}\left(\frac1d + \frac{1}{d + D}\right)\hat y = -2\times10^{-7}\cdot1369\left(\frac{1}{0{,}08} + \frac{1}{0{,}23}\right)\ \text{T}\ \hat y = -4{,}61\ \text{mT}\ \hat y$$

**Paso 5 — Fuerza.** $\vec F = q\vec v\times\vec B$, con $\vec v \parallel \hat y$ y $\vec B \parallel \hat y$:

$$\vec F = q\,v\hat y\times(-B\hat y) = \vec 0$$

Si las dos corrientes fueran en $-\hat k$, $\vec B$ apuntaría en $+\hat y$ y la fuerza seguiría siendo nula, porque la velocidad es paralela al campo.

</details>

**Respuesta:** a) Paralelas (se atraen); b) $I \approx 1369$ A; c) $\vec F = 0$, porque en la posición de la carga $\vec B$ ($\approx 4{,}61$ mT) es paralelo a $\vec v$ (ambos según $\hat j$)

</details>

---

### Ejercicio 2

Un alambre de longitud 5 m se enrolla para formar una bobina circular de área 2,21 x 10<sup>-3</sup> m<sup>2</sup>. La bobina es sumergida en un campo magnético perpendicular al plano que la contiene, y cuya intensidad varía en el tiempo según la ley:

B(t) = a t<sup>2</sup> + b t<sup>4</sup> [T],

donde a y b son coeficientes. Sabiendo que la resistencia de la bobina es de 5Ω, y que la corriente que circula por ella satisface I(t=1 s) = 0,3 A; I(t=2 s) = 0,05 A, determinar los valores de a y b.

<details>
<summary><b>Solución</b></summary>

<details>
<summary>Solución paso a paso</summary>

**Paso 1 — Número de vueltas.** Con el área se obtiene el radio y la longitud de cada vuelta:

$$r = \sqrt{\frac{A}{\pi}} = \sqrt{\frac{2{,}21\times10^{-3}}{\pi}}\ \text{m} = 2{,}652\ \text{cm} \qquad 2\pi r = 16{,}66\ \text{cm}$$

$$N = \frac{5\ \text{m}}{0{,}1666\ \text{m}} = 30\ \text{vueltas}$$

**Paso 2 — Fem y corriente.** El flujo concatenado es $N\phi = NA\,B(t)$, así que

$$|\mathcal E| = NA\frac{dB}{dt} = NA\,(2at + 4bt^3) \qquad I(t) = \frac{NA}{R}(2at + 4bt^3)$$

con $NA = 30\cdot2{,}21\times10^{-3} = 0{,}0663$ m². Las dos corrientes se toman con el mismo signo, tal como están dadas.

**Paso 3 — Sistema de ecuaciones.**

$$t = 1\ \text{s}:\quad 2a + 4b = \frac{0{,}3\cdot5}{0{,}0663} = 22{,}62$$

$$t = 2\ \text{s}:\quad 4a + 32b = \frac{0{,}05\cdot5}{0{,}0663} = 3{,}771$$

**Paso 4 — Resolución.** Se multiplica la primera por 2 ($4a + 8b = 45{,}25$) y se resta a la segunda:

$$24b = 3{,}771 - 45{,}25 \quad\Rightarrow\quad b = -1{,}728\ \text{T/s}^4$$

$$a = \frac{22{,}62 - 4b}{2} = \frac{22{,}62 + 6{,}913}{2} = 14{,}77\ \text{T/s}^2$$

**Verificación.** $I(1) = \tfrac{0{,}0663}{5}(29{,}54 - 6{,}91) = 0{,}30$ A ✓ y $I(2) = \tfrac{0{,}0663}{5}(59{,}07 - 55{,}30) = 0{,}05$ A ✓.

</details>

**Respuesta:** $N = 30$ vueltas; $a \approx 14{,}77$ T/s², $b \approx -1{,}73$ T/s⁴

</details>

---

### Ejercicio 3

Un solenoide muy largo de autoinducción L=8 x 10<sup>-6</sup> H transporta una corriente de 25 A.
**a)** Determinar la energía almacenada en el solenoide.
**b)** Sabiendo que el radio del solenoide es de 0,6 cm, y que la intensidad del campo magnético en su interior es B=7 x 10<sup>-4</sup> T, calcular la longitud del solenoide.
Dato: µ<sub>0</sub> = 4π x 10<sup>-7</sup> Tm/A.

<details>
<summary><b>Solución</b></summary>

<details>
<summary>Solución paso a paso</summary>

**Paso 1 — Energía (ítem a).**

$$U = \tfrac12LI^2 = \tfrac12\cdot8\times10^{-6}\cdot25^2\ \text{J} = 2{,}5\times10^{-3}\ \text{J}$$

**Paso 2 — Densidad de energía (ítem b).** En el interior el campo es uniforme, con $u = \dfrac{B^2}{2\mu_0}$, y ocupa un volumen $\pi R^2\ell$:

$$U = \frac{B^2}{2\mu_0}\pi R^2\ell \quad\Rightarrow\quad \ell = \frac{2\mu_0U}{B^2\pi R^2}$$

**Paso 3 — Cálculo.** $\pi R^2 = \pi(0{,}006)^2 = 1{,}131\times10^{-4}$ m²:

$$\ell = \frac{2\cdot4\pi\times10^{-7}\cdot2{,}5\times10^{-3}}{(7\times10^{-4})^2\cdot1{,}131\times10^{-4}}\ \text{m} = 113{,}4\ \text{m}$$

**Verificación (con L y n).** $n = \dfrac{B}{\mu_0I} = 22{,}28$ m⁻¹, y $L = \mu_0n^2\pi R^2\ell$ da $\ell = 113{,}4$ m ✓.

</details>

**Respuesta:** a) $U = 2{,}5$ mJ; b) $\ell \approx 113$ m

</details>

---

### Ejercicio 4

Una espira conductora circular de radio 2,5 cm transporta una corriente de 3 A. Una espira cuadrada de lado D transporta una corriente de 8 A.
**a)** Asigne un sentido de circulación a la corriente en la espira circular, y determine el valor del campo magnético (módulo, dirección y sentido) en su centro.
**b)** Calcular el valor de D para que en el centro de la espira cuadrada el campo magnético tenga una intensidad igual al triple de la intensidad del campo en el centro de la espira circular.
Dato: µ<sub>0</sub> = 4π x 10<sup>-7</sup> Tm/A.

<details>
<summary><b>Solución</b></summary>

<details>
<summary>Solución paso a paso</summary>

**Paso 1 — Espira circular (ítem a).** Por Biot-Savart, en el centro $B = \dfrac{\mu_0I}{2R}$:

$$B_c = \frac{4\pi\times10^{-7}\cdot3}{2\cdot0{,}025}\ \text{T} = 7{,}54\times10^{-5}\ \text{T} = 75{,}4\ \mu\text{T}$$

Con corriente en **sentido antihorario** (vista desde arriba de la hoja), el campo en el centro es perpendicular al plano de la espira y **saliente**. Con sentido horario sería entrante.

**Paso 2 — Espira cuadrada.** Cada lado de longitud D está a $D/2$ del centro y ve sus extremos a 45°:

$$B_{lado} = \frac{\mu_0I}{4\pi(D/2)}\cdot2\operatorname{sen}45^\circ = \frac{\sqrt2\,\mu_0I}{2\pi D} \qquad B_{cuad} = 4B_{lado} = \frac{2\sqrt2\,\mu_0I}{\pi D}$$

**Paso 3 — Condición (ítem b).** $B_{cuad} = 3B_c$:

$$D = \frac{2\sqrt2\,\mu_0I_{cuad}}{3\pi B_c} = \frac{2\sqrt2\cdot4\pi\times10^{-7}\cdot8}{3\pi\cdot7{,}54\times10^{-5}}\ \text{m} = 0{,}040\ \text{m}$$

</details>

**Respuesta:** a) $B = 75{,}4\ \mu$T, perpendicular al plano (saliente si la corriente circula en sentido antihorario); b) $D \approx 4{,}0$ cm

</details>

---

### Ejercicio 5

Un generador de alterna de frecuencia 50 Hz se conecta con una bobina cuya resistencia interna no es despreciable. La lectura del amperímetro es de 5 A, la potencia es de 100 W y el factor de potencia es 0,6.
**a)** Determine la inductancia L de la bobina.
**b)** Se desea conectar un capacitor en serie con la bobina, de tal modo que el nuevo factor de potencia sea 0,9. Determine dos valores posibles de C.

<details>
<summary><b>Solución</b></summary>

<details>
<summary>Solución paso a paso</summary>

**Paso 1 — Resistencia interna.** $P = I_{EF}^2R$, así que $R = \dfrac{100}{25}\ \Omega = 4\ \Omega$.

**Paso 2 — Impedancia y L (ítem a).**

$$Z = \frac{R}{\cos\varphi} = \frac{4}{0{,}6}\ \Omega = 6{,}667\ \Omega \qquad X_L = \sqrt{Z^2 - R^2} = 5{,}333\ \Omega$$

$$L = \frac{X_L}{2\pi f} = \frac{5{,}333}{100\pi}\ \text{H} = 16{,}98\ \text{mH}$$

**Paso 3 — Reactancia neta con factor 0,9 (ítem b).** R no cambia y la frecuencia tampoco:

$$Z' = \frac{R}{0{,}9} = 4{,}444\ \Omega \qquad |X_L - X_C| = \sqrt{Z'^2 - R^2} = 1{,}937\ \Omega$$

**Paso 4 — Las dos soluciones.**

- Circuito todavía inductivo: $X_C = X_L - 1{,}937 = 3{,}396\ \Omega$.
- Circuito capacitivo: $X_C = X_L + 1{,}937 = 7{,}271\ \Omega$.

$$C = \frac{1}{2\pi fX_C} \quad\Rightarrow\quad C_1 = \frac{1}{100\pi\cdot3{,}396}\ \text{F} = 937\ \mu\text{F} \qquad C_2 = \frac{1}{100\pi\cdot7{,}271}\ \text{F} = 438\ \mu\text{F}$$

</details>

**Respuesta:** a) $L \approx 17{,}0$ mH ($R = 4\ \Omega$); b) $C_1 \approx 937\ \mu$F (queda inductivo) o $C_2 \approx 438\ \mu$F (queda capacitivo)

</details>
