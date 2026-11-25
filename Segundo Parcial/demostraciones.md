# Demostraciones de los atajos del 2º Parcial

Práctica: demostrar cada uno de los [10 atajos del formulario](formulario.md#los-10-atajos) partiendo solo de las leyes. Al final hay tres demostraciones más que se pidieron en parciales.

**Cómo usarlo.** Leer el enunciado y la línea "Partí de", y hacer la demostración en papel. Si te trabás, abrir **Pista**. Al terminar, comparar con **Demostración**.

Lo único que se supone sabido:

| Ley | Fórmula |
|---|---|
| Biot-Savart | $d\vec B = \dfrac{\mu_0 I}{4\pi}\ \dfrac{d\vec l\times\vec r}{r^3}$, con $\vec r$ del elemento de cable al punto P |
| Ampère | $\displaystyle\oint\vec B\cdot d\vec l = \mu_0 I_{enc}$ |
| Fuerza magnética | $\vec F = q\ \vec v\times\vec B$ |
| Faraday | $\mathcal E = -\dfrac{d\phi}{dt}$, $\ \phi = \displaystyle\iint\vec B\cdot d\vec A$ |
| Inductancia | $N\phi = LI$, $\ \mathcal E = -L\dfrac{dI}{dt}$ |
| Capacitor | $q = Cv$ |
| Gauss | $\displaystyle\oint\vec E\cdot d\vec A = \frac{Q_{enc}}{\varepsilon_0}$, $\ V = \displaystyle\int\vec E\cdot d\vec l$ |
| Alterna | $v_L = L\dfrac{di}{dt}$, $\ v = ZI$ con $Z = R + j(X_L - X_C)$ |

Orden sugerido: primero 1, 2 y 4 (los imprescindibles), después el resto.

Volver al [índice de parciales](README.md).

---

## 1. Tramo recto

**Demostrá** que un tramo recto de cable con corriente $I$ produce en un punto P a distancia $d$ de su recta

$$B = \frac{\mu_0 I}{4\pi d}\left[\frac{x}{\sqrt{x^2 + d^2}}\right]_{x_1}^{x_2} = \frac{\mu_0 I}{4\pi d}(\mathrm{sen}\ \beta_2 - \mathrm{sen}\ \beta_1)$$

donde $x_1$ y $x_2$ son las posiciones de los extremos medidas desde el pie de la perpendicular trazada desde P. Deducí de ahí el hilo infinito $\dfrac{\mu_0 I}{2\pi d}$, el semi-infinito con P frente a su extremo $\dfrac{\mu_0 I}{4\pi d}$, y que si P está sobre la prolongación del tramo $B = 0$.

**Partí de:** Biot-Savart.

<details>
<summary>Pista</summary>

Poné el cable sobre el eje $x$ con el origen en el pie de la perpendicular, y P en $(0, d)$. Escribí $d\vec l$ y $\vec r$ en componentes y hacé el producto vectorial. La integral sale con $x = d\tan u$.

</details>

<details>
<summary>Demostración</summary>

El elemento de cable en $(x, 0)$ es $d\vec l = dx\ \hat x$. El vector que va de él a P es $\vec r = (-x,\ d)$, de módulo $r = \sqrt{x^2 + d^2}$.

$$d\vec l\times\vec r = dx\ \hat x\times(-x\ \hat x + d\ \hat y) = d\ dx\ \hat z$$

(porque $\hat x\times\hat x = 0$ y $\hat x\times\hat y = \hat z$). Todos los elementos aportan en la misma dirección $\hat z$, así que alcanza con integrar el módulo:

$$B = \frac{\mu_0 I}{4\pi}\int_{x_1}^{x_2}\frac{d\ dx}{(x^2 + d^2)^{3/2}}$$

Con $x = d\tan u$: $dx = d\sec^2u\ du$ y $(x^2 + d^2)^{3/2} = d^3\sec^3u$. Entonces

$$\int\frac{d\ dx}{(x^2 + d^2)^{3/2}} = \int\frac{d\cdot d\sec^2u}{d^3\sec^3u}\ du = \frac1d\int\cos u\ du = \frac{\mathrm{sen}\ u}{d} = \frac{1}{d}\cdot\frac{x}{\sqrt{x^2 + d^2}}$$

(de $\tan u = x/d$ se tiene $\mathrm{sen}\ u = x/\sqrt{x^2 + d^2}$). Queda

$$B = \frac{\mu_0 I}{4\pi d}\left[\frac{x}{\sqrt{x^2 + d^2}}\right]_{x_1}^{x_2}$$

El corchete en cada extremo es el seno del ángulo $\beta$ con que P ve ese extremo, medido desde la perpendicular.

**Casos particulares.**

- *Hilo infinito:* $x_1\to-\infty$, $x_2\to+\infty$. El corchete da $1 - (-1) = 2$, así que $B = \dfrac{\mu_0 I}{2\pi d}$.
- *Semi-infinito con P frente a su extremo:* $x_1 = 0$, $x_2\to\infty$. El corchete da $1 - 0 = 1$, así que $B = \dfrac{\mu_0 I}{4\pi d}$.
- *P sobre la prolongación:* ahí $\vec r$ es paralelo a $d\vec l$ en todo el tramo, así que $d\vec l\times\vec r = \vec0$ y $B = 0$.

</details>

---

## 2. Arco centrado en P

**Demostrá** que un arco de radio $R$ y ángulo $\theta$ (en radianes), con corriente $I$, produce en su centro

$$B = \frac{\mu_0 I\theta}{4\pi R}$$

y deducí el campo de una espira circular en su centro, $\dfrac{\mu_0 I}{2R}$.

**Partí de:** Biot-Savart.

<details>
<summary>Pista</summary>

Todos los elementos del arco están a la misma distancia de P. ¿Qué ángulo forman $d\vec l$ y $\vec r$? Escribí $dl$ en función del ángulo.

</details>

<details>
<summary>Demostración</summary>

Cada elemento del arco está a distancia $r = R$ de P, y $d\vec l$ es tangente al arco, o sea perpendicular al radio. Entonces $\lvert d\vec l\times\vec r\rvert = dl\cdot R$, y todos los aportes apuntan en la misma dirección (perpendicular al plano del arco). Con $dl = R\ d\varphi$:

$$B = \frac{\mu_0 I}{4\pi}\int\frac{dl\cdot R}{R^3} = \frac{\mu_0 I}{4\pi}\int_0^\theta\frac{R\ d\varphi}{R^2} = \frac{\mu_0 I\theta}{4\pi R}$$

**Espira circular:** $\theta = 2\pi$, así que $B = \dfrac{\mu_0 I\cdot2\pi}{4\pi R} = \dfrac{\mu_0 I}{2R}$.

</details>

---

## 3. Anillo en su eje

**Demostrá** que un anillo de radio $R$ con corriente $I$ produce en un punto de su eje, a distancia $z$ del centro,

$$B = \frac{\mu_0 IR^2}{2(R^2 + z^2)^{3/2}}$$

dirigido a lo largo del eje.

**Partí de:** Biot-Savart.

<details>
<summary>Pista</summary>

Anillo en el plano $xy$ centrado en el origen, P en $(0, 0, z)$. Parametrizá el anillo con el ángulo $\varphi$: posición $R(\cos\varphi, \mathrm{sen}\ \varphi, 0)$. Escribí $d\vec l$ y $\vec r$ en componentes y hacé el producto vectorial completo. Al integrar en $\varphi$ de 0 a $2\pi$, ¿qué componentes sobreviven?

</details>

<details>
<summary>Demostración</summary>

Elemento en $R(\cos\varphi, \mathrm{sen}\ \varphi, 0)$:

$$d\vec l = R\ d\varphi\ (-\mathrm{sen}\ \varphi,\ \cos\varphi,\ 0) \qquad \vec r = P - \text{elemento} = (-R\cos\varphi,\ -R\ \mathrm{sen}\ \varphi,\ z)$$

y $r = \sqrt{R^2 + z^2}$, igual para todos los elementos. Producto vectorial:

$$(-\mathrm{sen}\ \varphi,\ \cos\varphi,\ 0)\times(-R\cos\varphi,\ -R\ \mathrm{sen}\ \varphi,\ z) = (z\cos\varphi,\ z\ \mathrm{sen}\ \varphi,\ R\ \mathrm{sen}^2\varphi + R\cos^2\varphi) = (z\cos\varphi,\ z\ \mathrm{sen}\ \varphi,\ R)$$

Entonces

$$\vec B = \frac{\mu_0 I}{4\pi r^3}\int_0^{2\pi}R\ (z\cos\varphi,\ z\ \mathrm{sen}\ \varphi,\ R)\ d\varphi$$

Las integrales de $\cos\varphi$ y $\mathrm{sen}\ \varphi$ en un período dan 0: las componentes perpendiculares al eje se cancelan. Queda solo la componente $z$:

$$B_z = \frac{\mu_0 I}{4\pi r^3}\cdot R^2\cdot2\pi = \frac{\mu_0 IR^2}{2r^3} = \frac{\mu_0 IR^2}{2(R^2 + z^2)^{3/2}}$$

**Control:** con $z = 0$ da $\dfrac{\mu_0 I}{2R}$, igual que la espira circular del atajo 2.

</details>

---

## 4. Solenoide

**Demostrá** que dentro de un solenoide largo con $n$ vueltas por metro y corriente $I$

$$B = \mu_0 nI$$

**Partí de:** Ampère, sabiendo que adentro el campo es uniforme y paralelo al eje, y afuera es despreciable.

<details>
<summary>Pista</summary>

Elegí como curva un rectángulo con un lado de largo $\ell'$ adentro, paralelo al eje, y el lado opuesto afuera. Analizá qué aporta cada uno de los cuatro lados y cuántas vueltas atraviesan el rectángulo.

</details>

<details>
<summary>Demostración</summary>

Curva: rectángulo con un lado de largo $\ell'$ dentro del solenoide y paralelo al eje, y el lado opuesto afuera.

- Lado de adentro: $\vec B\parallel d\vec l$ y $B$ constante, aporta $B\ell'$.
- Lado de afuera: $B\approx0$, aporta 0.
- Los dos lados perpendiculares al eje: adentro $\vec B\perp d\vec l$ y afuera $B\approx0$, aportan 0.

El rectángulo encierra $n\ell'$ vueltas, cada una con corriente $I$, así que $I_{enc} = n\ell' I$:

$$\oint\vec B\cdot d\vec l = B\ell' = \mu_0 n\ell' I \quad\Rightarrow\quad B = \mu_0 nI$$

</details>

---

## 5. Hilo y logaritmo

**Demostrá** las dos fórmulas con logaritmo:

**a)** Una espira rectangular en el mismo plano que un hilo infinito con corriente $I$, con lados de largo $c$ paralelos al hilo, ubicados a distancias $x_1$ y $x_2$ de él, tiene flujo

$$\phi = \frac{\mu_0 Ic}{2\pi}\ln\frac{x_2}{x_1}$$

**b)** Una barra de largo $\ell$, perpendicular al hilo, con su extremo más cercano a distancia $d$, que se mueve paralela al hilo con velocidad $v$, tiene entre sus extremos

$$\mathcal E = \frac{\mu_0 Iv}{2\pi}\ln\frac{d + \ell}{d}$$

**Partí de:** el campo del hilo infinito (atajo 1, o Ampère sobre una circunferencia), Faraday y la fuerza magnética.

<details>
<summary>Pista</summary>

**a)** El campo del hilo depende solo de la distancia al hilo. Tomá como elemento de área una franja paralela al hilo, donde $B$ es constante.

**b)** No hay circuito cerrado. Sobre cada carga de la barra actúa $q\ \vec v\times\vec B$, que hace de campo eléctrico. La fem es la integral de línea de ese campo a lo largo de la barra.

</details>

<details>
<summary>Demostración</summary>

**Campo del hilo.** Por simetría, $\vec B$ es tangente a las circunferencias centradas en el hilo y tiene el mismo módulo en cada una. Ampère sobre una circunferencia de radio $x$:

$$B\cdot2\pi x = \mu_0 I \quad\Rightarrow\quad B(x) = \frac{\mu_0 I}{2\pi x}$$

En el plano del hilo, $\vec B$ es perpendicular a ese plano.

**a)** El campo es perpendicular a la espira y constante en cada franja de largo $c$ y ancho $dx$, a distancia $x$ del hilo. Con $dA = c\ dx$:

$$\phi = \iint\vec B\cdot d\vec A = \int_{x_1}^{x_2}\frac{\mu_0 I}{2\pi x}\ c\ dx = \frac{\mu_0 Ic}{2\pi}\ln\frac{x_2}{x_1}$$

**b)** $\vec v$ es paralela al hilo y $\vec B$ es perpendicular al plano, así que $\vec v\perp\vec B$. Entonces $\vec v\times\vec B$ tiene módulo $vB$ y es perpendicular a los dos, o sea que apunta a lo largo de la barra. Integrando desde el extremo cercano ($r = d$) hasta el lejano ($r = d + \ell$):

$$\mathcal E = \int_d^{d + \ell}(\vec v\times\vec B)\cdot d\vec r = \int_d^{d + \ell}v\ \frac{\mu_0 I}{2\pi r}\ dr = \frac{\mu_0 Iv}{2\pi}\ln\frac{d + \ell}{d}$$

</details>

---

## 6. Barra que gira

**Demostrá** que una barra de largo $r_0$ que gira con velocidad angular $\omega$ alrededor de uno de sus extremos, en un campo uniforme $B$ perpendicular al plano de giro, tiene entre sus extremos

$$\mathcal E = \tfrac12B\omega r_0^2$$

Hacelo de dos formas: con la fuerza magnética y con Faraday.

**Partí de:** la fuerza magnética y Faraday.

<details>
<summary>Pista</summary>

*Con la fuerza:* ¿con qué velocidad se mueve el punto de la barra que está a distancia $r$ del eje?

*Con Faraday:* ¿qué área barre la barra en un tiempo $t$?

</details>

<details>
<summary>Demostración</summary>

**Con la fuerza magnética.** El punto a distancia $r$ del eje se mueve con $v = \omega r$, perpendicular a la barra. Como $\vec B$ es perpendicular al plano de giro, $\vec v\perp\vec B$ y $\vec v\times\vec B$ tiene módulo $\omega rB$, a lo largo de la barra:

$$\mathcal E = \int_0^{r_0}(\vec v\times\vec B)\cdot d\vec r = \int_0^{r_0}\omega rB\ dr = \tfrac12B\omega r_0^2$$

**Con Faraday.** En un tiempo $t$ la barra gira un ángulo $\omega t$ y barre un sector circular de área $\tfrac12r_0^2\omega t$. El flujo a través de esa área es $\phi = \tfrac12Br_0^2\omega t$ y

$$\mathcal E = \frac{d\phi}{dt} = \tfrac12B\omega r_0^2$$

</details>

---

## 7. Energía magnética

**Demostrá** que la energía guardada en una inductancia $L$ con corriente $I$ es

$$U = \tfrac12LI^2$$

y que, en un solenoide, eso es igual a $\dfrac{B^2}{2\mu_0}\cdot\text{volumen}$.

**Partí de:** la fem autoinducida $\mathcal E = -L\dfrac{di}{dt}$, y $B = \mu_0 nI$ y $L = \mu_0 n^2A\ell$ (atajo 4 y [demostración A](#a-autoinductancia-de-un-solenoide)).

<details>
<summary>Pista</summary>

Mientras la corriente crece de 0 a $I$, la fuente tiene que vencer la fem autoinducida. ¿Qué potencia entrega? Integrá esa potencia en el tiempo y hacé el cambio de variable a $i$.

</details>

<details>
<summary>Demostración</summary>

Para que la corriente crezca, la fuente tiene que vencer la fem autoinducida, de módulo $L\dfrac{di}{dt}$. La potencia que entrega es la tensión por la corriente:

$$P = L\frac{di}{dt}\cdot i$$

La energía es la integral de la potencia en el tiempo. Cambiando la variable a $i$ (que va de 0 a $I$):

$$U = \int L\ i\ \frac{di}{dt}\ dt = \int_0^IL\ i\ di = \tfrac12LI^2$$

**En un solenoide**, con $L = \mu_0 n^2A\ell$ y $B = \mu_0 nI$:

$$U = \tfrac12\mu_0 n^2A\ell\ I^2 = \frac{(\mu_0 nI)^2}{2\mu_0}A\ell = \frac{B^2}{2\mu_0}\cdot A\ell$$

y $A\ell$ es el volumen interior.

</details>

---

## 8. Energía de un capacitor

**Demostrá** que la energía guardada en un capacitor $C$ cargado a tensión $V$ es

$$U = \tfrac12CV^2 = \frac{Q^2}{2C}$$

y que una fuente de tensión fija $V$, al cargarlo desde cero, entrega $QV$: el doble de lo que queda guardado. La otra mitad se disipa en las resistencias.

**Partí de:** $q = Cv$, y que mover una carga $dq$ a través de una tensión $v$ cuesta $v\ dq$.

<details>
<summary>Pista</summary>

Durante la carga, la tensión del capacitor no es fija: depende de la carga que ya tiene. La de la fuente sí es fija.

</details>

<details>
<summary>Demostración</summary>

**Energía guardada.** Cuando el capacitor tiene carga $q$, su tensión es $v = q/C$. Llevar una carga $dq$ más cuesta $v\ dq$. Integrando de 0 a $Q$:

$$U = \int_0^Q\frac qC\ dq = \frac{Q^2}{2C} = \frac{(CV)^2}{2C} = \tfrac12CV^2$$

**Energía que entrega la fuente.** La fuente mantiene la tensión $V$ fija mientras pasa toda la carga:

$$W = \int_0^QV\ dq = QV = CV^2$$

La diferencia, $CV^2 - \tfrac12CV^2 = \tfrac12CV^2$, se disipa en las resistencias del circuito. No depende de cuánto valgan.

</details>

---

## 9. Eficaces y potencia

**Demostrá** que, con $v = V_0\ \mathrm{sen}\ (\omega t)$ e $i = I_0\ \mathrm{sen}\ (\omega t - \varphi)$:

**a)** El valor eficaz, $V_{EF} = \sqrt{\dfrac1T\displaystyle\int_0^Tv^2\ dt}$, es $V_{EF} = \dfrac{V_0}{\sqrt2}$.

**b)** La potencia media, $P = \dfrac1T\displaystyle\int_0^Tv\ i\ dt$, es $P = V_{EF}I_{EF}\cos\varphi = I_{EF}^2R$.

**Partí de:** $V_0 = ZI_0$ y $\cos\varphi = R/Z$ (módulo y argumento de $Z$).

<details>
<summary>Pista</summary>

**a)** $\mathrm{sen}^2u = \tfrac12(1 - \cos2u)$.

**b)** $\mathrm{sen}\ a\ \mathrm{sen}\ b = \tfrac12[\cos(a - b) - \cos(a + b)]$. Un coseno de $2\omega t$ promedia cero en un período.

</details>

<details>
<summary>Demostración</summary>

**a)** Con $T = 2\pi/\omega$:

$$V_{EF}^2 = \frac1T\int_0^TV_0^2\ \mathrm{sen}^2(\omega t)\ dt = \frac{V_0^2}{T}\int_0^T\frac{1 - \cos(2\omega t)}{2}\ dt = \frac{V_0^2}{T}\cdot\frac T2 = \frac{V_0^2}{2}$$

porque la integral de $\cos(2\omega t)$ en un período es 0. Entonces $V_{EF} = V_0/\sqrt2$, y lo mismo para la corriente.

**b)** Con $a = \omega t$ y $b = \omega t - \varphi$, se tiene $a - b = \varphi$ y $a + b = 2\omega t - \varphi$:

$$P = \frac{V_0I_0}{T}\int_0^T\frac{\cos\varphi - \cos(2\omega t - \varphi)}{2}\ dt = \frac{V_0I_0}{2}\cos\varphi$$

Como $\dfrac{V_0I_0}{2} = \dfrac{V_0}{\sqrt2}\cdot\dfrac{I_0}{\sqrt2} = V_{EF}I_{EF}$, queda $P = V_{EF}I_{EF}\cos\varphi$.

Reemplazando $V_{EF} = ZI_{EF}$ y $\cos\varphi = R/Z$:

$$P = ZI_{EF}\cdot I_{EF}\cdot\frac RZ = I_{EF}^2R$$

Solo la resistencia consume energía en promedio.

</details>

---

## 10. Capacitor cilíndrico

**Demostrá** que un capacitor formado por dos cilindros coaxiales de radios $a < b$ y largo $\ell$ tiene

$$C = \frac{2\pi\varepsilon_0\ell}{\ln(b/a)}$$

**Partí de:** Gauss, $V = \displaystyle\int\vec E\cdot d\vec l$ y $C = Q/V$.

<details>
<summary>Pista</summary>

Poné carga $\lambda$ por unidad de largo en el cilindro interior. Para el campo entre los cilindros, usá como superficie de Gauss un cilindro coaxial de radio $r$ y largo $\ell$.

</details>

<details>
<summary>Demostración</summary>

Sea $\lambda$ la carga por unidad de largo del cilindro interior ($Q = \lambda\ell$). Por simetría, entre los cilindros $\vec E$ es radial y depende solo de $r$. Superficie de Gauss: cilindro coaxial de radio $r$ ($a < r < b$) y largo $\ell$. Las tapas no aportan flujo porque $\vec E$ es paralelo a ellas:

$$E\cdot2\pi r\ell = \frac{\lambda\ell}{\varepsilon_0} \quad\Rightarrow\quad E = \frac{\lambda}{2\pi\varepsilon_0 r}$$

Diferencia de potencial entre los cilindros:

$$V = \int_a^b\frac{\lambda}{2\pi\varepsilon_0 r}\ dr = \frac{\lambda}{2\pi\varepsilon_0}\ln\frac ba$$

Entonces

$$C = \frac QV = \frac{\lambda\ell}{\dfrac{\lambda}{2\pi\varepsilon_0}\ln(b/a)} = \frac{2\pi\varepsilon_0\ell}{\ln(b/a)}$$

</details>

---

# Demostraciones que se pidieron en parciales

## A. Autoinductancia de un solenoide

**Demostrá** que un solenoide de $N$ vueltas, largo $\ell$ y sección $A$ tiene $L = \dfrac{\mu_0 N^2A}{\ell}$. Se pidió en [09/12/2021, Ej. 2a](2021-12-09-1er-recuperatorio-2do-parcial.md#ejercicio-2) ("justifique la fórmula utilizada").

**Partí de:** $N\phi = LI$ y el atajo 4.

<details>
<summary>Demostración</summary>

Por el atajo 4, con $n = N/\ell$, adentro $B = \mu_0\dfrac N\ell I$, uniforme. El flujo por cada vuelta es $\phi = BA$. Por la definición de $L$:

$$L = \frac{N\phi}{I} = \frac{N\cdot\mu_0\dfrac N\ell I\cdot A}{I} = \frac{\mu_0 N^2A}{\ell}$$

</details>

---

## B. Inductancia mutua de dos solenoides coaxiales

**Demostrá** que dos solenoides coaxiales de igual largo $\ell$, con $N_1$ y $N_2$ vueltas, tienen $M = \dfrac{\mu_0 N_1N_2A_{\text{menor}}}{\ell}$. Se pidió en [09/12/2021, Ej. 2b](2021-12-09-1er-recuperatorio-2do-parcial.md#ejercicio-2).

**Partí de:** $N_1\phi_{1\leftarrow2} = MI_2$ y el atajo 4.

<details>
<summary>Pista</summary>

El campo de cada solenoide existe solo dentro de él. ¿A través de qué área atraviesa las vueltas del otro?

</details>

<details>
<summary>Demostración</summary>

Sea 2 el solenoide exterior (área $A_2$) y 1 el interior (área $A_1 < A_2$). El campo del exterior, $B_2 = \mu_0\dfrac{N_2}{\ell}I_2$, es uniforme en todo su interior, así que atraviesa cada vuelta del solenoide 1 por toda su área $A_1$:

$$M = \frac{N_1\phi_{1\leftarrow2}}{I_2} = \frac{N_1\cdot\mu_0\dfrac{N_2}{\ell}I_2\cdot A_1}{I_2} = \frac{\mu_0 N_1N_2A_1}{\ell}$$

Calculado al revés da lo mismo. El campo del interior existe solo dentro de $A_1$, así que también atraviesa las vueltas del exterior solo por $A_1$. En los dos casos va el área **menor**.

</details>

---

## C. Espira rectangular en su centro

**Demostrá** que una espira rectangular de lados $a$ y $b$ con corriente $I$ produce en su centro

$$B = \frac{2\mu_0 I\sqrt{a^2 + b^2}}{\pi ab}$$

Se pidió en [20/11/2015, Ej. 1](2015-11-20-2do-parcial.md#ejercicio-1), para un rectángulo $a\times\sqrt3a$.

**Partí de:** el atajo 1.

<details>
<summary>Pista</summary>

Cada lado se ve desde su mediatriz, así que $x_1 = -x_2$. Los cuatro lados aportan en el mismo sentido.

</details>

<details>
<summary>Demostración</summary>

Un lado de largo $\ell$ visto desde su mediatriz a distancia $d$: por el atajo 1 con $x_1 = -\ell/2$, $x_2 = \ell/2$,

$$B_{lado} = \frac{\mu_0 I}{4\pi d}\cdot\frac{2\cdot\ell/2}{\sqrt{(\ell/2)^2 + d^2}} = \frac{\mu_0 I}{4\pi d}\cdot\frac{\ell}{\sqrt{(\ell/2)^2 + d^2}}$$

Desde el centro, $\sqrt{(a/2)^2 + (b/2)^2} = \tfrac12\sqrt{a^2 + b^2}$ para cualquier lado. Los dos lados de largo $a$ están a $d = b/2$, y los dos de largo $b$ a $d = a/2$. Con la corriente circulando, los cuatro aportan en el mismo sentido:

$$B = 2\cdot\frac{\mu_0 I}{4\pi(b/2)}\cdot\frac{a}{\tfrac12\sqrt{a^2 + b^2}} + 2\cdot\frac{\mu_0 I}{4\pi(a/2)}\cdot\frac{b}{\tfrac12\sqrt{a^2 + b^2}} = \frac{2\mu_0 I}{\pi\sqrt{a^2 + b^2}}\left(\frac ab + \frac ba\right)$$

$$= \frac{2\mu_0 I}{\pi\sqrt{a^2 + b^2}}\cdot\frac{a^2 + b^2}{ab} = \frac{2\mu_0 I\sqrt{a^2 + b^2}}{\pi ab}$$

</details>
