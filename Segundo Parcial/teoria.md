# 2º Parcial — teoría para resolver los parciales

Guía de estudio orientada al examen: qué tipos de ejercicio se toman en el 2º Parcial (temas 5 a 7, y desde 2024 también capacitores), qué teoría hace falta para cada uno y cómo se resuelve paso a paso. Para el desarrollo completo de cada tema hay links a los resúmenes de [Magnetostática](../5%20-%20Magnetost%C3%A1tica/teoria.md), [Inducción](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md) y [Corriente alterna](../7%20-%20Corriente%20Alterna/teoria.md).

Volver al [índice de parciales](README.md) · Ver la [teoría del 1er Parcial](../Primer%20Parcial/teoria.md).

---

## Índice

0. [Mapa del parcial](#0-mapa-del-parcial)
1. [Sentidos: producto vectorial y regla de la mano derecha](#1-sentidos-producto-vectorial-y-regla-de-la-mano-derecha)
2. [Campo de hilos, arcos y espiras (Biot-Savart)](#2-campo-de-hilos-arcos-y-espiras-biot-savart)
3. [Hilos paralelos: campo nulo y fuerza entre hilos](#3-hilos-paralelos-campo-nulo-y-fuerza-entre-hilos)
4. [Fuerza sobre cargas y movimiento en un campo](#4-fuerza-sobre-cargas-y-movimiento-en-un-campo)
5. [Solenoides: campo, autoinducción, inductancia mutua y energía](#5-solenoides-campo-autoinducción-inductancia-mutua-y-energía)
6. [Flujo e inducción: ley de Faraday-Lenz](#6-flujo-e-inducción-ley-de-faraday-lenz)
7. [Fem de movimiento: barras](#7-fem-de-movimiento-barras)
8. [Corriente alterna: circuito RLC serie](#8-corriente-alterna-circuito-rlc-serie)
9. [Capacitores (desde 2024)](#9-capacitores-desde-2024)
10. [Errores frecuentes](#10-errores-frecuentes)
11. [Tabla de fórmulas](#11-tabla-de-fórmulas)

---

## 0. Mapa del parcial

El examen tiene 4 o 5 ejercicios. Casi siempre hay **un campo por superposición** (hilos doblados o espiras), **uno de hilos paralelos**, **uno de inducción** (barra o espira) y **un RLC serie**.

| Tipo de ejercicio | Dónde apareció | Sección |
|---|---|---|
| Hilo doblado / arco: campo en P | [03/12/20 Ej 4](2020-12-03-2do-parcial.md#ejercicio-4), [19/02/21 Ej 1](2021-02-19-2do-recuperatorio-2do-parcial.md#ejercicio-1), [12/12/24 Ej 2](2024-12-12-1er-recuperatorio-2do-parcial.md#ejercicio-2), [27/11/25 Ej 1](2025-11-27-2do-parcial-tema-2.md#ejercicio-1) | [2](#2-campo-de-hilos-arcos-y-espiras-biot-savart) |
| Espira cuadrada/rectangular vs. circular | [2015 Ej 1](2015-11-20-2do-parcial.md#ejercicio-1), [03/12/20 Ej 2](2020-12-03-2do-parcial.md#ejercicio-2), [25/11/21 Ej 2](2021-11-25-2do-parcial.md#ejercicio-2), [18/02/22 Ej 1](2022-02-18-2do-recuperatorio-2do-parcial.md#ejercicio-1), [simulacro Ej 4](simulacro-2do-parcial.md#ejercicio-4) | [2](#2-campo-de-hilos-arcos-y-espiras-biot-savart) |
| Anillo en su eje (con o sin hilo) | [19/02/21 Ej 2](2021-02-19-2do-recuperatorio-2do-parcial.md#ejercicio-2), [09/12/21 Ej 3](2021-12-09-1er-recuperatorio-2do-parcial.md#ejercicio-3), [2015 Ej 2](2015-11-20-2do-parcial.md#ejercicio-2) | [2](#2-campo-de-hilos-arcos-y-espiras-biot-savart) |
| Hilos paralelos: campo nulo, I₂, fuerza | [03/12/20 Ej 1](2020-12-03-2do-parcial.md#ejercicio-1), [25/11/21 Ej 1](2021-11-25-2do-parcial.md#ejercicio-1), [09/12/21 Ej 1](2021-12-09-1er-recuperatorio-2do-parcial.md#ejercicio-1), [28/11/24 Ej 2](2024-11-28-2do-parcial.md#ejercicio-2), [27/11/25 Ej 2](2025-11-27-2do-parcial-tema-2.md#ejercicio-2), [simulacro Ej 1](simulacro-2do-parcial.md#ejercicio-1) | [3](#3-hilos-paralelos-campo-nulo-y-fuerza-entre-hilos) |
| Carga en un campo: hélice, fuerza, B no uniforme | [25/11/21 Ej 3](2021-11-25-2do-parcial.md#ejercicio-3), [18/02/22 Ej 2](2022-02-18-2do-recuperatorio-2do-parcial.md#ejercicio-2) | [4](#4-fuerza-sobre-cargas-y-movimiento-en-un-campo) |
| Solenoide: L, M, energía, longitud | [09/12/21 Ej 2](2021-12-09-1er-recuperatorio-2do-parcial.md#ejercicio-2), [18/02/22 Ej 4](2022-02-18-2do-recuperatorio-2do-parcial.md#ejercicio-4), [28/11/24 Ej 3](2024-11-28-2do-parcial.md#ejercicio-3), [simulacro Ej 3](simulacro-2do-parcial.md#ejercicio-3) | [5](#5-solenoides-campo-autoinducción-inductancia-mutua-y-energía) |
| Espira junto a un hilo: flujo y fem | [19/02/21 Ej 3](2021-02-19-2do-recuperatorio-2do-parcial.md#ejercicio-3), [25/11/21 Ej 1](2021-11-25-2do-parcial.md#ejercicio-1) | [6](#6-flujo-e-inducción-ley-de-faraday-lenz) |
| Bobina con B(t) | [simulacro Ej 2](simulacro-2do-parcial.md#ejercicio-2) | [6](#6-flujo-e-inducción-ley-de-faraday-lenz) |
| Barra sobre rieles (B uniforme o B(x)) | [03/12/20 Ej 3](2020-12-03-2do-parcial.md#ejercicio-3), [27/11/25 Ej 3](2025-11-27-2do-parcial-tema-2.md#ejercicio-3) | [7](#7-fem-de-movimiento-barras) |
| Barra paralela a un hilo / barra que gira | [18/02/22 Ej 3](2022-02-18-2do-recuperatorio-2do-parcial.md#ejercicio-3), [12/12/24 Ej 4](2024-12-12-1er-recuperatorio-2do-parcial.md#ejercicio-4), [2015 Ej 3](2015-11-20-2do-parcial.md#ejercicio-3) | [7](#7-fem-de-movimiento-barras) |
| RLC serie (R, L, C, potencias, resonancia) | todos los parciales | [8](#8-corriente-alterna-circuito-rlc-serie) |
| Dos valores de C / corrección del factor de potencia | [19/02/21 Ej 4](2021-02-19-2do-recuperatorio-2do-parcial.md#ejercicio-4), [28/11/24 Ej 4](2024-11-28-2do-parcial.md#ejercicio-4), [simulacro Ej 5](simulacro-2do-parcial.md#ejercicio-5) | [8](#8-corriente-alterna-circuito-rlc-serie) |
| Afirmaciones conceptuales sobre RLC | [19/02/21 Ej 5](2021-02-19-2do-recuperatorio-2do-parcial.md#ejercicio-5) | [8](#8-corriente-alterna-circuito-rlc-serie) |
| Diagrama de fasores con dos elementos | [27/11/25 Ej 4](2025-11-27-2do-parcial-tema-2.md#ejercicio-4) | [8](#8-corriente-alterna-circuito-rlc-serie) |
| Capacitores con llaves / capacitor cilíndrico | [28/11/24 Ej 1](2024-11-28-2do-parcial.md#ejercicio-1), [12/12/24 Ej 1 y 3](2024-12-12-1er-recuperatorio-2do-parcial.md#ejercicio-1) | [9](#9-capacitores-desde-2024) |

**Formato del examen** (desde 2024): cada ítem se califica B (2 puntos), R (1 punto) o M (0). Hay que **justificar los pasos y las fórmulas**: un error conceptual grave anula el ítem. En los campos siempre se pide **módulo, dirección y sentido**.

**Dato:** $\mu_0 = 4\pi\times10^{-7}$ T m/A, así que $\dfrac{\mu_0}{2\pi} = 2\times10^{-7}$ y $\dfrac{\mu_0}{4\pi} = 10^{-7}$ (en SI).

---

## 1. Sentidos: producto vectorial y regla de la mano derecha

La mitad de los puntos se pierde por sentidos mal puestos. Convención: $\hat x$ a la derecha, $\hat y$ hacia arriba, $\hat k$ **saliente** de la hoja (⊙); entrante es ⊗.

$$\hat x\times\hat y = \hat k \qquad \hat y\times\hat k = \hat x \qquad \hat k\times\hat x = \hat y \qquad (\text{al revés, cambia el signo})$$

- **Campo de una corriente:** pulgar en el sentido de I y los dedos dan el sentido de $\vec B$, que rodea el hilo. Formalmente, $d\vec B \propto I\,d\vec l\times\hat r$, con $\hat r$ **desde el hilo hacia el punto**.
  - Hilo vertical con I hacia arriba: a su **derecha** el campo es entrante; a su **izquierda**, saliente.
- **Espira o arco:** si la corriente gira en **sentido antihorario** visto desde el lector, el campo en el centro es **saliente**; si gira en sentido horario, entrante.
- **Fuerza sobre una carga:** $\vec F = q\vec v\times\vec B$. Si $q < 0$, el sentido se invierte.
- **Tramo cuya prolongación pasa por P:** $d\vec l\parallel\hat r$, así que **no aporta campo**.

Teoría: [fuerza magnética sobre una carga](../5%20-%20Magnetost%C3%A1tica/teoria.md#1-fuerza-magnética-sobre-una-carga), [Biot-Savart](../5%20-%20Magnetost%C3%A1tica/teoria.md#7-ley-de-biot-savart).

---

## 2. Campo de hilos, arcos y espiras (Biot-Savart)

Teoría completa: [Biot-Savart](../5%20-%20Magnetost%C3%A1tica/teoria.md#7-ley-de-biot-savart), [campos de configuraciones típicas](../5%20-%20Magnetost%C3%A1tica/teoria.md#8-campos-de-configuraciones-típicas), [ejemplos de clase](../5%20-%20Magnetost%C3%A1tica/teoria.md#13-ejemplos-resueltos-en-clase).

### Fórmulas base

**Hilo recto finito** ([teoría](../5%20-%20Magnetost%C3%A1tica/teoria.md#hilo-recto-finito)): a distancia $y$ del punto, con $\theta_1, \theta_2$ los ángulos con que se ven los extremos, medidos desde la perpendicular que pasa por P (con signo):

$$B = \frac{\mu_0I}{4\pi y}\left(\operatorname{sen}\theta_2 - \operatorname{sen}\theta_1\right) \qquad \operatorname{sen}\theta = \frac{x_{extremo}}{\sqrt{x_{extremo}^2 + y^2}}$$

| Caso | Resultado |
|---|---|
| [Hilo infinito](../5%20-%20Magnetost%C3%A1tica/teoria.md#hilo-infinito) | $B = \dfrac{\mu_0I}{2\pi r}$ |
| [Semi-infinito](../5%20-%20Magnetost%C3%A1tica/teoria.md#hilo-semiinfinito) con el extremo **al pie** de la perpendicular | $B = \dfrac{\mu_0I}{4\pi r}$ (la mitad) |
| Semi-infinito con el extremo **desplazado** $x_0$ del pie | $B = \dfrac{\mu_0I}{4\pi y}\left(1 \mp \dfrac{x_0}{\sqrt{x_0^2 + y^2}}\right)$ (− si el hilo arranca después del pie, + si lo cruza) |
| Lado de longitud $\ell$, punto en su mediatriz a distancia $y$ | $B = \dfrac{\mu_0I}{4\pi y}\cdot\dfrac{\ell}{\sqrt{(\ell/2)^2 + y^2}}$ |
| [Arco de ángulo Δθ](../5%20-%20Magnetost%C3%A1tica/teoria.md#arco-de-circunferencia-en-el-centro), en su centro | $B = \dfrac{\mu_0I\,\Delta\theta}{4\pi R}$ (semicírculo: $\mu_0I/4R$) |
| [Espira circular](../5%20-%20Magnetost%C3%A1tica/teoria.md#espira-circular-en-su-eje), en el centro | $B = \dfrac{\mu_0I}{2R}$ |
| Espira circular, en el eje a distancia $z$ | $B = \dfrac{\mu_0IR^2}{2(R^2 + z^2)^{3/2}}$ |
| Espira cuadrada de lado $a$, centro | $B = \dfrac{2\sqrt2\,\mu_0I}{\pi a}$ |
| Espira rectangular $a\times b$, centro | $B = \dfrac{2\mu_0I\sqrt{a^2 + b^2}}{\pi ab}$ |

### Método para un hilo doblado (o una figura con tramos)

1. **Ubicar P como origen** y dividir la figura en tramos: rectos (finitos, semi-infinitos) y arcos.
2. Para cada tramo recto: distancia perpendicular $y$ a P, posición del pie de la perpendicular y ángulos de los extremos. **Si la recta del tramo pasa por P, aporta 0.**
3. Para cada arco: ángulo barrido Δθ (puede ser mayor que π, por ejemplo π + α).
4. **Sentido de cada aporte** con la regla de la mano derecha (sección 1). Anotar ⊙ o ⊗.
5. Sumar con signo. Si P y los tramos están en el mismo plano, todos los aportes son perpendiculares a la hoja y la suma es algebraica.

Ejemplos resueltos: [12/12/24 Ej 2](2024-12-12-1er-recuperatorio-2do-parcial.md#ejercicio-2) (arco de π + α y semi-infinito desplazado), [27/11/25 Ej 1](2025-11-27-2do-parcial-tema-2.md#ejercicio-1) (hilo en L), [03/12/20 Ej 4](2020-12-03-2do-parcial.md#ejercicio-4); de clase: [hilo con un arco de 120°](../5%20-%20Magnetost%C3%A1tica/teoria.md#hilo-con-un-arco-de-120-y-dos-tramos-rectos).

### Trucos de examen

- **Comparar espiras** ("¿qué lado/radio para que el campo sea k veces…?"): igualar fórmulas y despejar. Las constantes se cancelan.
- **Anillo en su eje, dado B en D, pedido en 3D:** el cociente $\dfrac{B(D)}{B(0)} = \dfrac{R^3}{(R^2 + D^2)^{3/2}}$ permite despejar D, y después se evalúa en 3D. Ejemplo: [09/12/21 Ej 3](2021-12-09-1er-recuperatorio-2do-parcial.md#ejercicio-3).
- **Anillo + hilo:** el anillo da campo sobre su eje y el hilo, perpendicular a su dirección. Se suman **como vectores** (componentes distintas). Ejemplo: [19/02/21 Ej 2](2021-02-19-2do-recuperatorio-2do-parcial.md#ejercicio-2).

---

## 3. Hilos paralelos: campo nulo y fuerza entre hilos

Teoría completa: [fuerza entre dos hilos paralelos](../5%20-%20Magnetost%C3%A1tica/teoria.md#11-fuerza-entre-dos-hilos-paralelos), [ejemplo de campo nulo exterior](../5%20-%20Magnetost%C3%A1tica/teoria.md#dos-hilos-antiparalelos-campo-nulo-en-un-punto-exterior).

$$B_i = \frac{\mu_0I_i}{2\pi r_i} \qquad \frac{F}{\ell} = \frac{\mu_0I_1I_2}{2\pi D}$$

- **Corrientes paralelas (mismo sentido) se atraen; antiparalelas se repelen.**
- **Dónde se anula el campo:**

| Corrientes | Entre los hilos | Afuera | Cero |
|---|---|---|---|
| Mismo sentido | campos opuestos | campos iguales | **entre** los hilos, más cerca del de **menor** corriente |
| Sentidos opuestos | campos iguales (se suman) | campos opuestos | **afuera**, del lado del de **menor** corriente |

- Condición: $\dfrac{I_1}{r_1} = \dfrac{I_2}{r_2}$. Entre los hilos, $r_2 = D - r_1$; afuera, del lado del hilo 1, $r_2 = r_1 + D$.
- **Problema inverso** (dan dónde se anula y piden I₂): la región (adentro o afuera) dice el sentido, y la condición da el valor. Ejemplos: [25/11/21 Ej 1](2021-11-25-2do-parcial.md#ejercicio-1), [09/12/21 Ej 1](2021-12-09-1er-recuperatorio-2do-parcial.md#ejercicio-1).
- **Dan la fuerza entre hilos:** si se atraen, son paralelas; de $F/\ell$ sale el producto $I_1I_2$. Ejemplos: [27/11/25 Ej 2](2025-11-27-2do-parcial-tema-2.md#ejercicio-2), [simulacro Ej 1](simulacro-2do-parcial.md#ejercicio-1).
- **Carga moviéndose cerca de los hilos:** primero el campo neto en ese punto, después $\vec F = q\vec v\times\vec B$. Si $\vec v\parallel\vec B$, la fuerza es nula; si $\vec v$ es paralela a los hilos, la fuerza es perpendicular a ellos.

---

## 4. Fuerza sobre cargas y movimiento en un campo

Teoría completa: [fuerza sobre una carga](../5%20-%20Magnetost%C3%A1tica/teoria.md#1-fuerza-magnética-sobre-una-carga), [movimiento en campo uniforme](../5%20-%20Magnetost%C3%A1tica/teoria.md#3-movimiento-de-una-carga-en-un-campo-uniforme), [fuerza sobre un conductor](../5%20-%20Magnetost%C3%A1tica/teoria.md#5-fuerza-sobre-un-conductor-con-corriente).

$$\vec F = q\vec v\times\vec B \qquad |\vec F| = |q|vB\operatorname{sen}\theta \qquad \vec F_{conductor} = I\vec\ell\times\vec B$$

- **La fuerza magnética no hace trabajo**, porque es siempre perpendicular a $\vec v$: **el módulo de la velocidad es constante**, aunque B dependa de la posición. Ejemplo: [18/02/22 Ej 2](2022-02-18-2do-recuperatorio-2do-parcial.md#ejercicio-2) (la respuesta es la velocidad inicial).
- **$\vec v\perp\vec B$ uniforme:** movimiento circular uniforme con

$$R = \frac{mv}{|q|B} \qquad T = \frac{2\pi m}{|q|B}$$

- **$\vec v$ oblicua (ángulo θ con B):** hélice con $R = \dfrac{mv\operatorname{sen}\theta}{|q|B}$ y paso $p = v\cos\theta\cdot T$. Si no se conocen $m$, $q$, $v$, se despeja la combinación $mv/|q|$ de un dato y se usa en el otro. Ejemplo: [25/11/21 Ej 3](2021-11-25-2do-parcial.md#ejercicio-3).
- **Carga en el centro de una espira con $\vec v$ en el plano:** $\vec B$ es perpendicular al plano, así que $\vec v\perp\vec B$ y $F = |q|vB$. Ejemplo: [18/02/22 Ej 1](2022-02-18-2do-recuperatorio-2do-parcial.md#ejercicio-1).

---

## 5. Solenoides: campo, autoinducción, inductancia mutua y energía

Teoría completa: [solenoide infinito](../5%20-%20Magnetost%C3%A1tica/teoria.md#solenoide-infinito), [Ampère](../5%20-%20Magnetost%C3%A1tica/teoria.md#9-ley-de-ampère), [autoinductancia](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md#8-autoinductancia), [inductancia mutua](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md#10-inductancia-mutua), [energía magnética](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md#12-energía-magnética).

$$B = \mu_0nI \quad (n = N/\ell) \qquad L = \frac{N\phi}{I} = \frac{\mu_0N^2A}{\ell} = \mu_0n^2A\ell \qquad \mathcal E_L = -L\frac{dI}{dt}$$

$$M = \frac{\mu_0N_1N_2A_{chico}}{\ell} \qquad U = \frac12LI^2 \qquad u = \frac{B^2}{2\mu_0}$$

- **"Justifique la fórmula":** hay que deducirla. Con Ampère, $B = \mu_0nI$; el flujo por espira es $BA$; el flujo concatenado es $N\cdot BA$; y $L = N\phi/I$.
- **Mutua de solenoides coaxiales:** el campo del interior solo existe dentro del solenoide de **menor** radio, así que se usa **el área chica**.
- **Pedir la longitud con L, I y B:** de B sale $n$, y de $L = \mu_0n^2A\ell$ sale $\ell$. También se puede por energía: $\tfrac12LI^2 = \dfrac{B^2}{2\mu_0}A\ell$. Ejemplos: [28/11/24 Ej 3](2024-11-28-2do-parcial.md#ejercicio-3), [simulacro Ej 3](simulacro-2do-parcial.md#ejercicio-3).
- **Fem autoinducida con $I(t) = I_0\operatorname{sen}\omega t$:** $\mathcal E = -LI_0\omega\cos\omega t$. Ejemplo: [18/02/22 Ej 4](2022-02-18-2do-recuperatorio-2do-parcial.md#ejercicio-4).

---

## 6. Flujo e inducción: ley de Faraday-Lenz

Teoría completa: [flujo magnético](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md#1-flujo-magnético), [Faraday-Lenz](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md#2-ley-de-faraday-lenz), [sentido de la corriente inducida](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md#3-cómo-determinar-el-sentido-de-la-corriente-inducida), [espira junto a un hilo](../5%20-%20Magnetost%C3%A1tica/teoria.md#espira-rectangular-junto-a-un-hilo).

$$\phi = \int\vec B\cdot\hat n\,dS \qquad \mathcal E = -N\frac{d\phi}{dt} \qquad I_{ind} = \frac{|\mathcal E|}{R}$$

### Flujo de un hilo infinito a través de una espira rectangular coplanar

Lados $c$ (paralelo al hilo) y desde $a$ hasta $b$ de distancia al hilo. Como B depende de $x$, se integra en franjas $dS = c\,dx$:

$$\phi = \int_a^b\frac{\mu_0I}{2\pi x}\,c\,dx = \frac{\mu_0Ic}{2\pi}\ln\frac{b}{a}$$

Con varios hilos, se suman los flujos con signo (campos opuestos restan).

### Las tres formas de variar el flujo

| Qué varía | Fem | Ejemplo |
|---|---|---|
| La corriente: $I(t)$ | $\mathcal E = -\dfrac{\mu_0c}{2\pi}\ln\dfrac ba\,\dfrac{dI}{dt}$ | [19/02/21 Ej 3a](2021-02-19-2do-recuperatorio-2do-parcial.md#ejercicio-3), [25/11/21 Ej 1c](2021-11-25-2do-parcial.md#ejercicio-1) |
| La posición: la espira se aleja, $a(t) = a_0 + vt$, $b(t) = b_0 + vt$ | $|\mathcal E| = \dfrac{\mu_0Ic}{2\pi}\,v\left(\dfrac1a - \dfrac1b\right)$ | [19/02/21 Ej 3b](2021-02-19-2do-recuperatorio-2do-parcial.md#ejercicio-3) |
| El campo: $B(t)$ uniforme sobre una bobina de N vueltas | $\mathcal E = -NA\dfrac{dB}{dt}$ | [simulacro Ej 2](simulacro-2do-parcial.md#ejercicio-2) |

### Sentido (Lenz)

1. ¿Hacia dónde apunta el flujo (⊙ o ⊗)? ¿Aumenta o disminuye?
2. La corriente inducida crea un campo que **se opone al cambio**. Si el flujo saliente aumenta, el inducido es entrante, y la corriente circula en sentido horario.
3. Si la espira se aleja del hilo, el flujo disminuye y la inducida **refuerza** el campo del hilo.

Si una bobina se arma con un alambre de longitud total $\ell_{alambre}$: $N = \dfrac{\ell_{alambre}}{2\pi r}$, con $r = \sqrt{A/\pi}$.

---

## 7. Fem de movimiento: barras

Teoría completa: [fem de movimiento](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md#4-fem-de-movimiento), [barra sobre rieles](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md#5-barra-sobre-rieles), [barra que gira](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md#barra-que-gira-alrededor-de-un-extremo), [barra paralela a un hilo](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md#barra-que-se-mueve-paralela-a-un-hilo).

$$\mathcal E = \int(\vec v\times\vec B)\cdot d\vec l$$

**Polaridad:** $\vec v\times\vec B$ indica hacia dónde van las cargas positivas. **El extremo hacia el que apunta queda a mayor potencial.**

### Casos

| Situación | Fem |
|---|---|
| Barra de largo $L$ sobre rieles, B uniforme ⊥ | $\mathcal E = BLv$, $I = BLv/R$ |
| Rieles con $B(x) = kx$ | $\mathcal E = B(x)Lv = kxLv$, con $x = vt$ (o por flujo: $\phi = kLx^2/2$) |
| Barra ⊥ a un hilo infinito, moviéndose **paralela** al hilo, de $d$ a $d + l$ | $\mathcal E = \dfrac{\mu_0Iv}{2\pi}\ln\dfrac{d + l}{d}$ |
| Barra que gira con ω alrededor de un extremo, B uniforme | $\mathcal E = \tfrac12B\omega L^2$ |
| Barra que gira alrededor de un punto O **interior** | Cada extremo respecto de O: $\tfrac12B\omega r^2$. Entre extremos: $\tfrac12B\omega(r_Q^2 - r_P^2)$ |

### Barra sobre rieles: fuerzas

- **Fuerza magnética** sobre la barra: $\vec F = I\vec L\times\vec B$, módulo $ILB$. Siempre **frena** el movimiento (Lenz).
- **Velocidad constante** significa fuerza neta nula: el agente externo hace $\vec F_{ext} = -\vec F_{mag}$.
- **Potencia:** $F_{ext}v = I^2R$. Sirve de verificación.
- **Rieles con varias resistencias:** la barra es una fuente de fem $BLv$; el resto se resuelve como un circuito de CC ([teoría del 1er Parcial](../Primer%20Parcial/teoria.md#1-circuitos-de-corriente-continua)). Ejemplo: [03/12/20 Ej 3](2020-12-03-2do-parcial.md#ejercicio-3).

---

## 8. Corriente alterna: circuito RLC serie

Teoría completa: [valores eficaces](../7%20-%20Corriente%20Alterna/teoria.md#3-valores-eficaces), [RLC serie](../7%20-%20Corriente%20Alterna/teoria.md#6-circuito-rlc-serie), [potencias](../7%20-%20Corriente%20Alterna/teoria.md#7-potencias-activa-aparente-y-reactiva), [resonancia](../7%20-%20Corriente%20Alterna/teoria.md#8-resonancia), [formalismo complejo](../7%20-%20Corriente%20Alterna/teoria.md#9-formalismo-complejo), [cómo encarar un RLC](../7%20-%20Corriente%20Alterna/teoria.md#11-cómo-encarar-un-ejercicio-de-rlc-serie).

### Fórmulas

$$\omega = 2\pi f \qquad X_L = \omega L \qquad X_C = \frac{1}{\omega C} \qquad X = X_L - X_C$$

$$Z = \sqrt{R^2 + X^2} \qquad V_{EF} = ZI_{EF} \qquad \cos\varphi = \frac{R}{Z} \qquad \tan\varphi = \frac{X}{R}$$

$$P = V_{EF}I_{EF}\cos\varphi = I_{EF}^2R \qquad S = V_{EF}I_{EF} = I_{EF}^2Z \qquad Q = I_{EF}^2X \qquad S^2 = P^2 + Q^2$$

$$\omega_0 = \frac{1}{\sqrt{LC}} \qquad V_{EF} = \frac{V_{pico}}{\sqrt2} \qquad P = \frac{V_{pico}I_{pico}}{2}\cos\varphi$$

### Inductivo o capacitivo

| | Inductivo | Capacitivo |
|---|---|---|
| Reactancias | $X_L > X_C$ | $X_C > X_L$ |
| Fase | la corriente **atrasa** (la tensión adelanta) | la corriente **adelanta** |
| Frecuencia | $f > f_0$ | $f < f_0$ |

En resonancia $X_L = X_C$, Z = R es mínima, la corriente es máxima y $\cos\varphi = 1$.

### Método general

1. Pasar todo a **eficaces** (el amperímetro mide eficaces; "corriente de pico" o $I_0$ en $I(t)$ es pico).
2. $R = P/I^2$, o $R = Z\cos\varphi$.
3. $Z = V/I = S/I^2$.
4. $|X| = \sqrt{Z^2 - R^2} = Z\operatorname{sen}\varphi$, y el signo sale de la fase o de la frecuencia respecto de la resonancia.
5. **Con $f$ y $f_0$:** $X = \omega L - \dfrac{1}{\omega C}$ y $C = \dfrac{1}{\omega_0^2L}$ dan

$$X = L\,\frac{\omega^2 - \omega_0^2}{\omega} \quad\Rightarrow\quad L = \frac{X\omega}{\omega^2 - \omega_0^2}$$

6. Tensión en cada elemento: $V_R = IR$, $V_L = IX_L$, $V_C = IX_C$. No se suman algebraicamente: $V = \sqrt{V_R^2 + (V_L - V_C)^2}$.

Ejemplos: [25/11/21 Ej 4](2021-11-25-2do-parcial.md#ejercicio-4), [18/02/22 Ej 5](2022-02-18-2do-recuperatorio-2do-parcial.md#ejercicio-5), [03/12/20 Ej 5](2020-12-03-2do-parcial.md#ejercicio-5).

### Situaciones especiales

- **Dos valores de C para el mismo |X|** (misma Z o mismo factor de potencia): $X_C = X_L \mp|X|$. Uno deja el circuito **inductivo** (por encima de la resonancia) y el otro **capacitivo**. Existen los dos si $X_L - |X| > 0$. Ejemplos: [28/11/24 Ej 4](2024-11-28-2do-parcial.md#ejercicio-4), [19/02/21 Ej 4](2021-02-19-2do-recuperatorio-2do-parcial.md#ejercicio-4).
- **Corregir el factor de potencia de una bobina real** (R interna + L) agregando C en serie: el nuevo $|X'| = R\tan(\arccos fp')$, y $X_C = X_L \mp|X'|$. Hay **dos** soluciones. Ejemplo: [simulacro Ej 5](simulacro-2do-parcial.md#ejercicio-5).
- **Reemplazar C sin cambiar el factor de potencia:** hace falta el mismo $|X|$ con el signo opuesto, $X_{C'} = 2X_L - X_C$. Existe si da positivo. Ejemplo: [09/12/21 Ej 4c](2021-12-09-1er-recuperatorio-2do-parcial.md#ejercicio-4).
- **Tensión sobre una bobina real:** $V_{bobina} = I\sqrt{R_{int}^2 + X_L^2}$, no $IX_L$.
- **Circuito de dos elementos con diagrama de fasores:** si la tensión adelanta, son R y L; si atrasa, R y C. Si disipa potencia, uno es R. Del dato de P sale $\cos\varphi$, y si da mayor que 1 no hay solución. Ejemplo: [27/11/25 Ej 4](2025-11-27-2do-parcial-tema-2.md#ejercicio-4).

### Afirmaciones conceptuales típicas

- "Por encima de la resonancia el circuito es capacitivo": **falsa** (es inductivo).
- "Si es inductivo, aumentando C se puede volver capacitivo": **falsa**. Aumentar C **baja** $X_C$, así que el circuito se vuelve más inductivo. Para volverlo capacitivo hay que **disminuir** C.
- "Una bobina con fp < 0,9 admite exactamente dos C en serie que llevan el fp a 0,9": **verdadera**.

Ejemplo: [19/02/21 Ej 5](2021-02-19-2do-recuperatorio-2do-parcial.md#ejercicio-5).

---

## 9. Capacitores (desde 2024)

Los parciales de 2024 incluyeron ejercicios de capacitores: llaves con energía disipada y un capacitor cilíndrico como parte de un RLC. La teoría está en la [teoría del 1er Parcial, sección 2](../Primer%20Parcial/teoria.md#2-capacitores-llaves-redistribución-de-carga-y-energía). Lo esencial:

- Al **cargar** un capacitor desde una fuente se disipa $\tfrac12CV^2$, la mitad de lo que entrega la fuente.
- Al **repartir** carga entre capacitores, se conserva la carga, todos los capacitores en paralelo terminan a la misma tensión, y se disipa $U_{antes} - U_{después}$.
- Capacitor cilíndrico: $C = \dfrac{2\pi\varepsilon_0\ell}{\ln(b/a)}$. Combinado con la resonancia: $L = \dfrac{1}{\omega_0^2C}$.

Ejemplos: [28/11/24 Ej 1](2024-11-28-2do-parcial.md#ejercicio-1), [12/12/24 Ej 1](2024-12-12-1er-recuperatorio-2do-parcial.md#ejercicio-1), [12/12/24 Ej 3](2024-12-12-1er-recuperatorio-2do-parcial.md#ejercicio-3).

---

## 10. Errores frecuentes

- **Sentidos:** sumar módulos de campos que en realidad se restan. Anotar ⊙ o ⊗ junto a cada aporte antes de sumar.
- Olvidar que un tramo alineado con P **no aporta** campo.
- Usar $\mu_0I/(2\pi r)$ (hilo infinito) para un tramo finito o semi-infinito.
- Mezclar valores **pico** y **eficaces** en alterna.
- Signo de X: decidirlo con la fase (adelanta → capacitivo) o con la frecuencia respecto de la resonancia. No suponerlo.
- Inductancia mutua con el área del solenoide grande (va la del **chico**).
- Ángulos de 0,01 s en $\operatorname{sen}(100\pi t)$: la calculadora tiene que estar en **radianes**.
- Olvidar N (el número de vueltas) en Faraday.
- Polaridad de una barra: el extremo **hacia donde empuja** $\vec v\times\vec B$ a las cargas positivas es el de **mayor** potencial.

---

## 11. Tabla de fórmulas

| Tema | Fórmula |
|---|---|
| Fuerza sobre una carga | $\vec F = q\vec v\times\vec B$ |
| Fuerza sobre un conductor | $\vec F = I\vec\ell\times\vec B$ |
| MCU | $R = mv/(\lvert q\rvert B)$, $T = 2\pi m/(\lvert q\rvert B)$ |
| Hélice | paso $p = v\cos\theta\,T$ |
| Hilo finito | $B = \frac{\mu_0I}{4\pi y}(\operatorname{sen}\theta_2 - \operatorname{sen}\theta_1)$ |
| Hilo infinito | $B = \mu_0I/(2\pi r)$ |
| Arco (centro) | $B = \mu_0I\Delta\theta/(4\pi R)$ |
| Espira circular (centro / eje) | $\mu_0I/(2R)$ / $\mu_0IR^2/[2(R^2 + z^2)^{3/2}]$ |
| Espira cuadrada / rectangular (centro) | $2\sqrt2\mu_0I/(\pi a)$ / $2\mu_0I\sqrt{a^2 + b^2}/(\pi ab)$ |
| Hilos paralelos | $F/\ell = \mu_0I_1I_2/(2\pi D)$ |
| Solenoide | $B = \mu_0nI$, $L = \mu_0N^2A/\ell$, $M = \mu_0N_1N_2A_{chico}/\ell$ |
| Energía magnética | $U = \tfrac12LI^2$, $u = B^2/(2\mu_0)$ |
| Faraday | $\mathcal E = -N\,d\phi/dt$ |
| Flujo hilo → espira | $\phi = \frac{\mu_0Ic}{2\pi}\ln(b/a)$ |
| Fem de movimiento | $\mathcal E = BLv$; barra que gira $\tfrac12B\omega L^2$; junto a hilo $\frac{\mu_0Iv}{2\pi}\ln\frac{d + l}{d}$ |
| Reactancias | $X_L = \omega L$, $X_C = 1/(\omega C)$ |
| Impedancia | $Z = \sqrt{R^2 + (X_L - X_C)^2}$ |
| Potencias | $P = VI\cos\varphi = I^2R$, $S = VI$, $Q = I^2X$ |
| Resonancia | $\omega_0 = 1/\sqrt{LC}$ |
| Capacitores | $U = \tfrac12CV^2$; cilíndrico $2\pi\varepsilon_0\ell/\ln(b/a)$ |

Tablas completas por tema: [Magnetostática](../5%20-%20Magnetost%C3%A1tica/teoria.md#14-tabla-de-fórmulas), [Inducción](../6%20-%20Inducci%C3%B3n%20Magn%C3%A9tica/teoria.md#14-tabla-de-fórmulas), [Corriente alterna](../7%20-%20Corriente%20Alterna/teoria.md#12-tabla-de-fórmulas).
