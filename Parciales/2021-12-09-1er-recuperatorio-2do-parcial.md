# 1er Recuperatorio del 2º Parcial — 09/12/2021

[Enunciado original (PDF)](Aula%20Virtual/2021-12-09%20-%201er%20Recuperatorio%202do%20Parcial.pdf) · [Resolución del profesor (PDF)](Aula%20Virtual/2021-12-09%20-%201er%20Recuperatorio%202do%20Parcial%20-%20Resoluci%C3%B3n.pdf) · Temas: hilos paralelos, autoinductancia e inductancia mutua, anillo con corriente, corriente alterna.

Cada ejercicio tiene un botón **Solución** con la respuesta y, adentro, un botón **Solución paso a paso**. Los resultados coinciden con la resolución del profesor.

Volver al [índice de parciales](README.md).

**DATO:** μ<sub>0</sub>=4π x 10<sup>-7</sup> Tm/A.

---

### Ejercicio 1

Dos alambres paralelos infinitos, separados por una distancia de 8 cm, están circulados por corrientes I<sub>1</sub>=1 A e I<sub>2</sub>, respectivamente. El campo magnético generado por los alambres se anula a una distancia de 2 cm del primero, en la región externa a los dos alambres. **a)** Determine I<sub>2</sub>. **b)** Halle el campo magnético en el punto medio entre ambos alambres. **c)** Una carga q=6 μC pasa por el punto del ítem anterior con una velocidad de módulo 4 x 10<sup>4</sup> m/s y dirección coincidente con la de los hilos. Determine el módulo de la fuerza sobre la carga.

<details>
<summary><b>Solución</b></summary>

<details>
<summary>Solución paso a paso</summary>

**Paso 1 — Sentidos (ítem a).** En la región **externa** los campos solo se cancelan si las corrientes son **opuestas**. El punto está a 2 cm del hilo 1 y a 10 cm del hilo 2:

$$\frac{\mu_0I_1}{2\pi\cdot0{,}02} = \frac{\mu_0I_2}{2\pi\cdot0{,}10} \quad\Rightarrow\quad I_2 = 5I_1 = 5\ \text{A}$$

**Paso 2 — Punto medio (ítem b).** Con corrientes opuestas, entre los hilos los campos se suman. Cada hilo está a 4 cm:

$$B = \frac{\mu_0}{2\pi}\left(\frac{I_1}{0{,}04} + \frac{I_2}{0{,}04}\right) = 2\times10^{-7}\cdot\frac{6}{0{,}04}\ \text{T} = 30\ \mu\text{T}$$

(Con I₁ hacia arriba y $\hat k$ saliente, el profesor obtiene $\vec B = -30\ \mu\text{T}\ \hat k$.)

**Paso 3 — Fuerza (ítem c).** La velocidad es paralela a los hilos y el campo es perpendicular a ellos, así que $\vec v\perp\vec B$:

$$F = qvB = 6\times10^{-6}\cdot4\times10^4\cdot30\times10^{-6}\ \text{N} = 7{,}2\times10^{-6}\ \text{N}$$

</details>

**Respuesta:** a) $I_2 = 5$ A (sentido opuesto a I₁); b) $|\vec B| = 30\ \mu$T; c) $|\vec F| = 7{,}2\ \mu$N

</details>

---

### Ejercicio 2

Un solenoide de radio 2 cm y longitud 60 cm tiene arrolladas 3000 vueltas de alambre. **a)** Determine el coeficiente de autoinducción del solenoide. Justifique la fórmula utilizada. **b)** Se dispone al solenoide de forma coaxial con otro solenoide de la misma longitud, radio 3 cm y 2000 vueltas de alambre. ¿Cuál es la inductancia mutua? Justifique la fórmula utilizada.

<details>
<summary><b>Solución</b></summary>

<details>
<summary>Solución paso a paso</summary>

**Paso 1 — Justificación.** El solenoide es mucho más largo que su radio (60 cm frente a 2 cm): vale la aproximación de solenoide infinito, $B = \mu_0\dfrac{N}{\ell}I$ uniforme en su interior.

**Paso 2 — Autoinductancia (ítem a).** $LI = \phi = NBA$:

$$L = \mu_0\frac{N^2}{\ell}\pi R^2 = 4\pi\times10^{-7}\cdot\frac{3000^2}{0{,}6}\cdot\pi\cdot(0{,}02)^2\ \text{H} = 23{,}69\ \text{mH}$$

**Paso 3 — Mutua (ítem b).** El campo del solenoide **exterior** ($B_2 = \mu_0N_2I_2/\ell$) es uniforme dentro de él y atraviesa la sección del **interior**, $\pi R_1^2$:

$$M = \frac{N_1B_2\pi R_1^2}{I_2} = \frac{\mu_0N_1N_2\pi R_1^2}{\ell}$$

Se usa el radio del solenoide **interior** (el menor).

$$M = \frac{4\pi\times10^{-7}\cdot3000\cdot2000\cdot\pi\cdot(0{,}02)^2}{0{,}6}\ \text{H} = 15{,}79\ \text{mH}$$

</details>

**Respuesta:** a) $L = 23{,}69$ mH; b) $M = 15{,}79$ mH

</details>

---

### Ejercicio 3

Un anillo de radio 6 cm transporta una corriente de 0,2 A. Si el módulo del campo en un punto situado sobre su eje y a distancia D de su centro es 0,285 μT, determine el módulo del campo en un punto sobre ese mismo eje y a distancia 3D del centro del anillo.

<details>
<summary><b>Solución</b></summary>

<details>
<summary>Solución paso a paso</summary>

**Paso 1 — Despejar D.** De $B_0 = \dfrac{\mu_0IR^2}{2(R^2 + D^2)^{3/2}}$:

$$D^2 = \left(\frac{\mu_0IR^2}{2B_0}\right)^{2/3} - R^2$$

$$\frac{\mu_0IR^2}{2B_0} = \frac{4\pi\times10^{-7}\cdot0{,}2\cdot0{,}0036}{2\cdot0{,}285\times10^{-6}} = 1{,}587\times10^{-3}\ \text{m}^3 \quad\Rightarrow\quad D^2 = 0{,}01361 - 0{,}0036 = 0{,}0100\ \text{m}^2$$

$$D = 10\ \text{cm}$$

**Paso 2 — Campo en 3D.**

$$B = \frac{\mu_0IR^2}{2[R^2 + (3D)^2]^{3/2}} = \frac{9{,}048\times10^{-10}}{2\cdot(0{,}0936)^{3/2}}\ \text{T} = 1{,}58\times10^{-8}\ \text{T}$$

</details>

**Respuesta:** $D = 10$ cm y $|\vec B(3D)| = 0{,}0158\ \mu$T

</details>

---

### Ejercicio 4

Se conecta una bobina L en serie con una resistencia R, un capacitor C=60 μF y un generador de alterna a 80 Hz. La lectura del amperímetro es de 3 A, y la tensión eficaz medida en los extremos de la bobina es 120 V. **a)** Determine R y L, y justifique si el circuito es capacitivo o inductivo. **b)** Calcule el factor de potencia y la frecuencia de resonancia. **c)** ¿Existe un capacitor que pueda reemplazar al que se encuentra en el circuito sin que cambie el factor de potencia? En caso afirmativo, determínelo. En caso negativo, justifique.

<details>
<summary><b>Solución</b></summary>

<details>
<summary>Solución paso a paso</summary>

**Paso 1 — L.** $V_L = X_LI$:

$$X_L = \frac{120}{3}\ \Omega = 40\ \Omega \qquad L = \frac{X_L}{\omega} = \frac{40}{160\pi}\ \text{H} = 79{,}6\ \text{mH}$$

**Paso 2 — Tipo de circuito.** $X_C = \dfrac{1}{160\pi\cdot60\times10^{-6}} = 33{,}16\ \Omega < X_L$: **inductivo**.

**Paso 3 — R.** ⚠️ El enunciado no da la tensión del generador ni otro dato que fije R. La resolución del profesor usa $Z = 12{,}12\ \Omega$, que corresponde a $R = 10\ \Omega$. Se sigue con ese valor.

**Paso 4 — Factor de potencia y resonancia (ítem b).**

$$Z = \sqrt{R^2 + (X_L - X_C)^2} = \sqrt{100 + 6{,}84^2}\ \Omega = 12{,}12\ \Omega \qquad \cos\phi = \frac RZ = 0{,}825$$

$$f_R = \frac{1}{2\pi\sqrt{LC}} = \frac{1}{2\pi\sqrt{0{,}0796\cdot60\times10^{-6}}}\ \text{Hz} = 72{,}8\ \text{Hz}$$

**Paso 5 — Otro capacitor (ítem c).** El factor de potencia depende de $|X_L - X_C|$. Se mantiene si la reactancia neta cambia de signo con el mismo módulo:

$$X'_C - X_L = X_L - X_C \quad\Rightarrow\quad X'_C = 2X_L - X_C = 46{,}84\ \Omega \qquad C' = \frac{1}{160\pi\cdot46{,}84}\ \text{F} = 42{,}5\ \mu\text{F}$$

Con $C'$ el circuito pasa a ser capacitivo, pero con el mismo factor de potencia.

</details>

**Respuesta:** a) $L = 79{,}6$ mH, inductivo ($X_L = 40\ \Omega > X_C = 33{,}16\ \Omega$); R no surge de los datos del enunciado (la resolución usa $R = 10\ \Omega$); b) $\cos\phi = 0{,}825$, $f_R = 72{,}83$ Hz; c) sí: $C' = 42{,}5\ \mu$F

</details>
