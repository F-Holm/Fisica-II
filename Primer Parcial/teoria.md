# 1er Parcial — teoría para resolver los parciales

Guía de estudio orientada al examen: qué tipos de ejercicio se toman en el 1er Parcial (temas 1 a 4), qué teoría hace falta para cada uno y cómo se resuelve paso a paso. Para el desarrollo completo de cada tema hay links a los resúmenes de [Termodinámica](../1%20-%20Termodin%C3%A1mica/teoria.md), [Electrostática](../2%20-%20Electrost%C3%A1tica/teoria.md), [Electrodinámica](../3%20-%20Electrodin%C3%A1mica/teoria.md) y [Capacitores](../4%20-%20Capacitores%20y%20Diel%C3%A9ctricos/teoria.md).

Volver al [índice de parciales](README.md) · Ver la [teoría del 2º Parcial](../Segundo%20Parcial/teoria.md).

---

## Índice

0. [Mapa del parcial](#0-mapa-del-parcial)
1. [Circuitos de corriente continua](#1-circuitos-de-corriente-continua)
2. [Capacitores: llaves, redistribución de carga y energía](#2-capacitores-llaves-redistribución-de-carga-y-energía)
3. [Campo y potencial de distribuciones de carga](#3-campo-y-potencial-de-distribuciones-de-carga)
4. [Ley de Gauss](#4-ley-de-gauss)
5. [Conducción del calor: barras en serie y en paralelo](#5-conducción-del-calor-barras-en-serie-y-en-paralelo)
6. [Termodinámica: primer principio, máquinas y Carnot](#6-termodinámica-primer-principio-máquinas-y-carnot)
7. [Calorimetría y dilatación](#7-calorimetría-y-dilatación)
8. [Errores frecuentes](#8-errores-frecuentes)
9. [Tabla de fórmulas](#9-tabla-de-fórmulas)

---

## 0. Mapa del parcial

El examen tiene 4 o 5 ejercicios. Casi siempre hay **un circuito**, **un ejercicio de campo o potencial por integración**, **uno de Gauss** y **uno de térmica** (conducción o Carnot). Los capacitores con llaves aparecen en el 1er Parcial y, desde 2024, también en el 2º.

| Tipo de ejercicio | Dónde apareció | Sección |
|---|---|---|
| Circuito con amperímetro/voltímetro, potencia de la fuente | [12/02/21 Ej 1](2021-02-12-2do-recuperatorio-1er-parcial.md#ejercicio-1), [19/08/21 Ej 1](2021-08-19-1er-parcial.md#ejercicio-1) | [1](#1-circuitos-de-corriente-continua) |
| Circuito con capacitor en estado estacionario + Joule + calorimetría | [16/12/21 Ej 1](2021-12-16-1er-recuperatorio-1er-parcial.md#ejercicio-1) | [1](#1-circuitos-de-corriente-continua), [7](#7-calorimetría-y-dilatación) |
| Capacitores con llaves (cargas finales, energía disipada) | [19/08/21 Ej 2](2021-08-19-1er-parcial.md#ejercicio-2), [28/11/24 Ej 1](../Segundo%20Parcial/2024-11-28-2do-parcial.md#ejercicio-1), [12/12/24 Ej 1](../Segundo%20Parcial/2024-12-12-1er-recuperatorio-2do-parcial.md#ejercicio-1) | [2](#2-capacitores-llaves-redistribución-de-carga-y-energía) |
| Hilo finito cargado sobre el eje: campo, fuerza, trabajo | [12/02/21 Ej 3](2021-02-12-2do-recuperatorio-1er-parcial.md#ejercicio-3), [16/12/21 Ej 5](2021-12-16-1er-recuperatorio-1er-parcial.md#ejercicio-5) | [3](#3-campo-y-potencial-de-distribuciones-de-carga) |
| Anillo cargado: fuerza en el eje, trabajo, mitades con distinta λ | [19/08/21 Ej 3](2021-08-19-1er-parcial.md#ejercicio-3), [16/12/21 Ej 3](2021-12-16-1er-recuperatorio-1er-parcial.md#ejercicio-3) | [3](#3-campo-y-potencial-de-distribuciones-de-carga) |
| Gauss: esfera uniforme, cilindro con ρ(r), cilindro con σ | [12/02/21 Ej 2](2021-02-12-2do-recuperatorio-1er-parcial.md#ejercicio-2), [19/08/21 Ej 4](2021-08-19-1er-parcial.md#ejercicio-4), [16/12/21 Ej 4](2021-12-16-1er-recuperatorio-1er-parcial.md#ejercicio-4) | [4](#4-ley-de-gauss) |
| Barras en serie entre dos focos | [12/02/21 Ej 4](2021-02-12-2do-recuperatorio-1er-parcial.md#ejercicio-4), [19/08/21 Ej 5](2021-08-19-1er-parcial.md#ejercicio-5) | [5](#5-conducción-del-calor-barras-en-serie-y-en-paralelo) |
| Carnot vs. máquina real | [16/12/21 Ej 2](2021-12-16-1er-recuperatorio-1er-parcial.md#ejercicio-2) | [6](#6-termodinámica-primer-principio-máquinas-y-carnot) |
| Capacitor cilíndrico (en un RLC) | [12/12/24 Ej 3](../Segundo%20Parcial/2024-12-12-1er-recuperatorio-2do-parcial.md#ejercicio-3) | [2](#2-capacitores-llaves-redistribución-de-carga-y-energía) |

**Formato del examen** (desde 2024): cada ítem se califica B (2 puntos), R (1 punto) o M (0). Hay que **justificar los pasos y las fórmulas**: un error conceptual grave anula el ítem. Conviene escribir siempre la fórmula simbólica antes de reemplazar.

---

## 1. Circuitos de corriente continua

Teoría completa: [Electrodinámica](../3%20-%20Electrodin%C3%A1mica/teoria.md) — [Ley de Ohm](../3%20-%20Electrodin%C3%A1mica/teoria.md#4-ley-de-ohm-y-resistencia), [potencia](../3%20-%20Electrodin%C3%A1mica/teoria.md#5-potencia-y-efecto-joule), [serie y paralelo](../3%20-%20Electrodin%C3%A1mica/teoria.md#6-conexión-de-resistencias), [Kirchhoff](../3%20-%20Electrodin%C3%A1mica/teoria.md#10-leyes-de-kirchhoff), [instrumentos](../3%20-%20Electrodin%C3%A1mica/teoria.md#11-instrumentos-de-medición), [capacitores en CC](../3%20-%20Electrodin%C3%A1mica/teoria.md#12-capacitores-en-circuitos-de-corriente-continua).

### Lo que hay que saber

$$V = IR \qquad P = VI = I^2R = \frac{V^2}{R} \qquad E = P\,t$$

$$R_{serie} = R_1 + R_2 + \dots \qquad \frac{1}{R_{paralelo}} = \frac{1}{R_1} + \frac{1}{R_2} + \dots \qquad \left(R_1\parallel R_2 = \frac{R_1R_2}{R_1 + R_2}\right)$$

- **Serie:** misma corriente; las tensiones se suman. **Paralelo:** misma tensión; las corrientes se suman.
- **Amperímetro ideal:** resistencia nula, va **en serie** y mide la corriente de su rama. **Voltímetro ideal:** resistencia infinita, va **en paralelo** y no deriva corriente.
- **Potencia que entrega la fuente:** $P = V_{fuente}\,I_{fuente}$. Siempre coincide con la suma de $I^2R$ de todas las resistencias, y sirve de verificación.

### Método

1. Identificar qué resistencias están realmente en serie (misma corriente, sin nodos intermedios) o en paralelo (mismos dos nodos). Si no se puede reducir, usar Kirchhoff.
2. **Kirchhoff:** asignar una corriente a cada rama con un sentido arbitrario, y plantear:
   - **nodos:** $\sum I_{entran} = \sum I_{salen}$ (nodos − 1 ecuaciones);
   - **mallas:** $\sum\mathcal E = \sum IR$ recorriendo cada malla independiente.

   Si una corriente da negativa, circula al revés.
3. Usar el dato del instrumento: el amperímetro fija una corriente y el voltímetro una diferencia de potencial ($V = IR$ entre sus bornes).
4. **"¿Existen valores de R tales que…?"**: plantear la corriente pedida en función de R. Queda una ecuación, a veces cuadrática. Hay solución si da **R > 0** real; si no, justificar que no existe. Ejemplo: [19/08/21 Ej 1b](2021-08-19-1er-parcial.md#ejercicio-1).

### Capacitores en estado estacionario

Con un tiempo largo, **por la rama de un capacitor no circula corriente**: la rama se trata como abierta. Se resuelve el circuito sin esa rama, y la tensión del capacitor es la diferencia de potencial entre sus dos nodos. Después $Q = CV$. Si el capacitor está en serie con una resistencia, esa resistencia no tiene caída de tensión (I = 0). Ejemplo: [16/12/21 Ej 1](2021-12-16-1er-recuperatorio-1er-parcial.md#ejercicio-1).

### Joule + calorimetría

La energía que disipa una resistencia en un tiempo $t$ se transforma en calor: $Q = I^2R\,t$ (en J; 1 cal = 4,18 J). Si calienta agua en un recipiente adiabático: $I^2Rt = mc\,\Delta T$. Ver [sección 7](#7-calorimetría-y-dilatación).

---

## 2. Capacitores: llaves, redistribución de carga y energía

Teoría completa: [Capacitores](../4%20-%20Capacitores%20y%20Diel%C3%A9ctricos/teoria.md) — [capacitancia](../4%20-%20Capacitores%20y%20Diel%C3%A9ctricos/teoria.md#1-capacitor-y-capacitancia), [serie y paralelo](../4%20-%20Capacitores%20y%20Diel%C3%A9ctricos/teoria.md#6-conexión-en-serie-y-en-paralelo), [redistribución de carga](../4%20-%20Capacitores%20y%20Diel%C3%A9ctricos/teoria.md#7-redistribución-de-carga-entre-capacitores), [energía](../4%20-%20Capacitores%20y%20Diel%C3%A9ctricos/teoria.md#8-energía-almacenada), [transitorios RC](../4%20-%20Capacitores%20y%20Diel%C3%A9ctricos/teoria.md#9-transitorios-rc-carga-y-descarga).

### Lo que hay que saber

$$Q = CV \qquad U = \frac12CV^2 = \frac{Q^2}{2C} = \frac12QV$$

- **Serie:** misma carga, $\dfrac{1}{C_{eq}} = \sum\dfrac{1}{C_i}$. **Paralelo:** misma tensión, $C_{eq} = \sum C_i$.
- Capacitores típicos ([plano](../4%20-%20Capacitores%20y%20Diel%C3%A9ctricos/teoria.md#2-capacitor-plano), [cilíndrico](../4%20-%20Capacitores%20y%20Diel%C3%A9ctricos/teoria.md#3-capacitor-cilíndrico), [esférico](../4%20-%20Capacitores%20y%20Diel%C3%A9ctricos/teoria.md#4-capacitor-esférico)):

$$C_{plano} = \frac{\varepsilon_0A}{d} \qquad C_{cilíndrico} = \frac{2\pi\varepsilon_0\ell}{\ln(b/a)} \qquad C_{esférico} = 4\pi\varepsilon_0\frac{ab}{b - a}$$

### Ejercicio típico: "se cierra la llave 1, pasado mucho tiempo se abre y se cierra la llave 2"

1. **Leer el circuito con cada combinación de llaves.** Con L1 cerrada, ver qué capacitores quedan conectados a la fuente. Los que quedan en una rama abierta no se cargan.
2. **Etapa 1 (con fuente):** después de mucho tiempo, cada capacitor conectado tiene la tensión que le impone el circuito. Si está directamente sobre la fuente, $Q_0 = CV$.
3. **Etapa 2 (sin fuente):** al abrir L1 la fuente queda afuera. Al cerrar L2 la carga se reparte. Se plantean:
   - **conservación de la carga en cada "isla"** (conjunto de placas conectadas entre sí y aisladas del resto);
   - **mallas sin fuente:** $\sum Q_i/C_i = 0$, con el signo de cada placa;
   - **capacitores en serie** tienen la misma carga.

   En el caso más común, un capacitor cargado con $Q_0$ se conecta en paralelo con otros descargados:

$$V_f = \frac{Q_0}{\sum C_i} \qquad Q_i = C_iV_f$$

### Energía disipada en las resistencias

Las resistencias pueden ser solo las de los cables: **la energía disipada no depende de su valor**.

- **Al cargar un capacitor desde una fuente ideal** se disipa siempre **la mitad** de lo que entrega la fuente: la fuente entrega $QV = CV^2$, el capacitor guarda $\tfrac12CV^2$ y se disipa $\tfrac12CV^2$.
- **Al repartir la carga** se disipa la diferencia de energías: $E = U_{antes} - U_{después}$. Para $C_1$ cargado a $V$ conectado a $C_2$ descargado:

$$E_{reparto} = \frac12\frac{C_1C_2}{C_1 + C_2}V^2$$

- **"En la evolución completa"** = carga + reparto. Ejemplos: [28/11/24 Ej 1](../Segundo%20Parcial/2024-11-28-2do-parcial.md#ejercicio-1) (64,8 mJ) y [12/12/24 Ej 1](../Segundo%20Parcial/2024-12-12-1er-recuperatorio-2do-parcial.md#ejercicio-1) (57,6 mJ).

**Verificación:** la suma de las cargas de la isla tiene que dar la carga inicial, y todos los capacitores en paralelo tienen que quedar a la misma tensión.

---

## 3. Campo y potencial de distribuciones de carga

Teoría completa: [Electrostática](../2%20-%20Electrost%C3%A1tica/teoria.md) — [Coulomb](../2%20-%20Electrost%C3%A1tica/teoria.md#3-ley-de-coulomb), [distribuciones continuas](../2%20-%20Electrost%C3%A1tica/teoria.md#5-distribuciones-continuas-de-carga), [campos típicos](../2%20-%20Electrost%C3%A1tica/teoria.md#6-campos-de-distribuciones-típicas), [potencial](../2%20-%20Electrost%C3%A1tica/teoria.md#11-potencial-eléctrico), [potenciales típicos](../2%20-%20Electrost%C3%A1tica/teoria.md#13-potenciales-de-distribuciones-típicas).

### Lo que hay que saber

$$k = \frac{1}{4\pi\varepsilon_0} = 9\times10^9\ \frac{\text{N m}^2}{\text{C}^2} \qquad d\vec E = k\frac{dq}{r^2}\hat r \qquad dV = k\frac{dq}{r} \qquad dq = \lambda\,dl$$

$$\vec F = q\vec E \qquad W_{campo}^{A\to B} = q\,(V_A - V_B) = -\Delta U$$

**Método general:** elegir un $dq$, escribir su distancia $r$ al punto, descomponer $d\vec E$ y **usar la simetría** para anular componentes antes de integrar. El potencial es escalar: se integra sin descomponer, y suele ser el camino más corto para calcular trabajos.

### Resultados que se usan directamente

| Distribución | Campo | Potencial (cero en ∞) |
|---|---|---|
| [Hilo finito, punto en su eje](../2%20-%20Electrost%C3%A1tica/teoria.md#hilo-finito-en-un-punto-de-su-eje), a distancias $a$ y $b$ de los extremos ($a < b$) | $E = k\lambda\left(\dfrac1a - \dfrac1b\right)$, sobre el eje | $V = k\lambda\ln\dfrac{b}{a}$ |
| [Hilo infinito](../2%20-%20Electrost%C3%A1tica/teoria.md#hilo-infinito) | $E = \dfrac{2k\lambda}{r} = \dfrac{\lambda}{2\pi\varepsilon_0r}$ | (solo diferencias) $V_A - V_B = 2k\lambda\ln\dfrac{r_B}{r_A}$ |
| [Anillo, punto en su eje](../2%20-%20Electrost%C3%A1tica/teoria.md#anillo-en-su-eje) a distancia $z$ | $E = \dfrac{kQz}{(R^2 + z^2)^{3/2}}$ | $V = \dfrac{kQ}{\sqrt{R^2 + z^2}}$ |
| [Arco de ángulo θ, en el centro](../2%20-%20Electrost%C3%A1tica/teoria.md#arco-de-circunferencia-en-el-centro) | $E = \dfrac{2k\lambda}{R}\operatorname{sen}\dfrac\theta2$ (semianillo: $2k\lambda/R$) | $V = k\lambda\theta$ |
| Carga puntual | $E = kq/r^2$ | $V = kq/r$ |

### Casos de examen

- **Fuerza de un hilo finito sobre una carga en su eje:** $F = qE$ con la fórmula del hilo en su eje. El **trabajo** al mover la carga de $x_3$ a $x_4$ por el eje es $W = q(V_3 - V_4)$, con $V = k\lambda\ln(b/a)$ en cada punto. Ejemplo: [16/12/21 Ej 5](2021-12-16-1er-recuperatorio-1er-parcial.md#ejercicio-5).
- **Dos hilos sobre el mismo eje:** superposición, y para cada uno se miden las distancias a sus propios extremos. Atención al signo de λ y al sentido (un hilo positivo "empuja" hacia afuera). Ejemplo: [12/02/21 Ej 3](2021-02-12-2do-recuperatorio-1er-parcial.md#ejercicio-3).
- **Anillo con dos mitades de distinta densidad:** cada semianillo da $2k\lambda/R$ en el centro, en sentidos opuestos (cada uno empuja desde su lado). El neto es $E = 2k|\lambda_1 - \lambda_2|/R$. Al igualar a un dato con módulo aparecen **dos soluciones**. Ejemplo: [16/12/21 Ej 3](2021-12-16-1er-recuperatorio-1er-parcial.md#ejercicio-3).
- **Carga sobre el eje de un anillo:** fuerza con el campo axial; trabajo con $V = kQ/\sqrt{R^2 + z^2}$ en las dos posiciones. Ejemplo: [19/08/21 Ej 3](2021-08-19-1er-parcial.md#ejercicio-3).

---

## 4. Ley de Gauss

Teoría completa: [Flujo](../2%20-%20Electrost%C3%A1tica/teoria.md#8-flujo-de-campo-eléctrico), [Ley de Gauss](../2%20-%20Electrost%C3%A1tica/teoria.md#9-ley-de-gauss), [conductores en equilibrio](../2%20-%20Electrost%C3%A1tica/teoria.md#10-conductores-en-equilibrio-electrostático).

$$\oint\vec E\cdot d\vec S = \frac{Q_{enc}}{\varepsilon_0}$$

### Método (hay que justificarlo en el examen)

1. **Simetría:** decir hacia dónde apunta $\vec E$ (radial) y de qué depende su módulo (solo de $r$).
2. **Superficie gaussiana** con esa simetría: una esfera de radio $r$, o un cilindro coaxial de radio $r$ y largo $\ell$. En el cilindro, las tapas no aportan flujo porque $\vec E$ es paralelo a ellas.
3. **Flujo:** $E\cdot4\pi r^2$ (esfera) o $E\cdot2\pi r\ell$ (cilindro).
4. **Carga encerrada:** si ρ es uniforme, $\rho\cdot$volumen. Si $\rho(r)$, **integrar en cascarones**: $Q_{enc} = \int_0^r\rho(r')\,dV'$ con $dV' = 4\pi r'^2dr'$ (esfera) o $2\pi r'\ell\,dr'$ (cilindro). Para $r$ fuera de la distribución, la integral llega solo hasta $R$.
5. Despejar E, una vez **adentro** ($r < R$) y otra **afuera** ($r > R$).

### Resultados

| Distribución | $r < R$ | $r > R$ |
|---|---|---|
| Esfera con ρ uniforme | $E = \dfrac{\rho r}{3\varepsilon_0}$ | $E = \dfrac{kQ}{r^2} = \dfrac{\rho R^3}{3\varepsilon_0r^2}$ |
| Cilindro con ρ uniforme | $E = \dfrac{\rho r}{2\varepsilon_0}$ | $E = \dfrac{\rho R^2}{2\varepsilon_0r}$ |
| Cilindro con $\rho = \alpha r$ | $E = \dfrac{\alpha r^2}{3\varepsilon_0}$ | $E = \dfrac{\alpha R^3}{3\varepsilon_0r}$ |
| Cilindro con σ en la superficie | $E = 0$ | $E = \dfrac{\sigma R}{\varepsilon_0r}$ |
| Conductor en equilibrio | $E = 0$ | según la carga total |

### Casos de examen

- **Relaciones entre puntos:** si se da E en un punto y se pide en otro, se hace el cociente de fórmulas y las constantes se cancelan. Para la esfera, $E(R/2) = \rho R/(6\varepsilon_0)$ y $E(2R) = \rho R/(12\varepsilon_0)$, así que $E(2R) = E(R/2)/2$. Ejemplo: [12/02/21 Ej 2](2021-02-12-2do-recuperatorio-1er-parcial.md#ejercicio-2).
- **Diferencia de potencial:** $V_A - V_B = \int_A^B\vec E\cdot d\vec r$. Afuera de una esfera, $V_A - V_B = kQ\left(\dfrac{1}{r_A} - \dfrac{1}{r_B}\right)$. Para un cilindro, $V_A - V_B = \dfrac{\lambda}{2\pi\varepsilon_0}\ln\dfrac{r_B}{r_A}$.
- **Trabajo dentro de un cascarón con σ:** el campo es nulo, así que el potencial es constante y **W = 0**. Ejemplo: [16/12/21 Ej 4](2021-12-16-1er-recuperatorio-1er-parcial.md#ejercicio-4).

---

## 5. Conducción del calor: barras en serie y en paralelo

Teoría completa: [Conducción](../1%20-%20Termodin%C3%A1mica/teoria.md#conducción), [resistencia térmica](../1%20-%20Termodin%C3%A1mica/teoria.md#resistencia-térmica), [conexión de resistencias térmicas](../1%20-%20Termodin%C3%A1mica/teoria.md#conexión-de-resistencias-térmicas).

$$H = \frac{dQ}{dt} = kA\frac{\Delta T}{L} = \frac{\Delta T}{R_T} \qquad R_T = \frac{L}{kA}$$

Es la "ley de Ohm térmica": $H \leftrightarrow I$, $\Delta T \leftrightarrow \Delta V$, $R_T \leftrightarrow R$.

### Método para barras en serie

1. En **régimen estacionario** y con las barras aisladas lateralmente, **el flujo de calor H es el mismo en todas**.
2. $T_{caliente} - T_{frío} = H\,(R_1 + R_2 + \dots)$, de donde sale H.
3. Temperatura de cada unión: desde el foco frío, $T_{unión} = T_{frío} + H R_1$ (o desde el caliente restando).
4. Si falta una conductividad: con la temperatura de una unión se obtiene H usando las barras conocidas, y después se despeja la $k$ que falta.

Con radios iguales, el área se cancela al comparar barras, y alcanza con $L/k$. **En paralelo:** misma $\Delta T$, y los $H$ se suman.

Ejemplos: [12/02/21 Ej 4](2021-02-12-2do-recuperatorio-1er-parcial.md#ejercicio-4) y [19/08/21 Ej 5](2021-08-19-1er-parcial.md#ejercicio-5).

---

## 6. Termodinámica: primer principio, máquinas y Carnot

Teoría completa: [primer principio](../1%20-%20Termodin%C3%A1mica/teoria.md#7-primer-principio), [trabajo en un gas](../1%20-%20Termodin%C3%A1mica/teoria.md#6-trabajo-en-un-gas), [energía interna](../1%20-%20Termodin%C3%A1mica/teoria.md#8-calores-específicos-molares-y-energía-interna), [adiabáticas](../1%20-%20Termodin%C3%A1mica/teoria.md#9-transformaciones-adiabáticas), [máquinas](../1%20-%20Termodin%C3%A1mica/teoria.md#10-máquinas-térmicas-y-frigoríficas), [Carnot](../1%20-%20Termodin%C3%A1mica/teoria.md#11-ciclo-de-carnot), [segundo principio](../1%20-%20Termodin%C3%A1mica/teoria.md#12-segundo-principio).

### Máquinas

$$\eta = \frac{W}{Q_{abs}} = 1 - \frac{|Q_{ced}|}{Q_{abs}} \qquad W = Q_{abs} - |Q_{ced}| \qquad \eta_{Carnot} = 1 - \frac{T_F}{T_C}\ \ (\text{en kelvin})$$

$$\text{Frigorífica:}\quad \varepsilon = \frac{Q_F}{W} \qquad \varepsilon_{Carnot} = \frac{T_F}{T_C - T_F}$$

- **Las temperaturas siempre en kelvin** (0 °C = 273 K). Es el error más común.
- Ninguna máquina real supera a la de Carnot entre los mismos focos.
- **Máquina real con "rendimiento la mitad que Carnot":** $\eta_r = \eta_C/2$, después $Q_{abs} = W/\eta_r$ y $|Q_{ced}| = Q_{abs} - W$. Ejemplo: [16/12/21 Ej 2](2021-12-16-1er-recuperatorio-1er-parcial.md#ejercicio-2).

### Primer principio y gas ideal (por si aparece)

$$\Delta U = Q - W \qquad pV = nRT \qquad \Delta U = nc_V\Delta T \qquad c_P - c_V = R$$

| Proceso | W | Q |
|---|---|---|
| Isocórico | 0 | $nc_V\Delta T$ |
| Isobárico | $p\Delta V$ | $nc_P\Delta T$ |
| Isotérmico | $nRT\ln(V_f/V_i)$ | $= W$ |
| Adiabático ($pV^\gamma$ = cte) | $-\Delta U$ | 0 |

En un ciclo $\Delta U = 0$, así que $W_{neto} = Q_{neto}$.

---

## 7. Calorimetría y dilatación

Teoría completa: [calorimetría](../1%20-%20Termodin%C3%A1mica/teoria.md#2-calorimetría), [dilatación](../1%20-%20Termodin%C3%A1mica/teoria.md#3-dilatación-térmica).

$$Q = mc\,\Delta T \qquad Q = mL\ (\text{cambio de fase}) \qquad \sum Q_i = 0\ (\text{recipiente adiabático})$$

$$\Delta L = \alpha L_0\Delta T \qquad \Delta V = \beta V_0\Delta T \qquad \beta = 3\alpha$$

Con Joule, la energía eléctrica entra como calor: $I^2Rt = mc\,\Delta T$, con $c_{agua} = 1$ cal/(g °C) = 4,18 J/(g °C).

---

## 8. Errores frecuentes

- Mezclar cm con m o μC con C. **Pasar todo al SI antes de reemplazar.**
- Temperaturas en °C en Carnot o en gases (van en K). En conducción y calorimetría da lo mismo, porque solo importan diferencias.
- Olvidar que **un capacitor en régimen estacionario corta la corriente** de su rama.
- En Gauss, olvidar integrar cuando ρ depende de r, o usar el radio de la gaussiana en lugar de R para la carga encerrada desde afuera.
- Signos de λ y sentidos de los campos en la superposición. Dibujar el vector de cada aporte antes de sumar.
- Trabajo del campo vs. trabajo externo: $W_{campo} = q(V_A - V_B) = -W_{externo}$, si no cambia la energía cinética.
- En energía disipada con capacitores, olvidarse de la etapa de **carga** (la mitad de lo que entrega la fuente).

---

## 9. Tabla de fórmulas

| Tema | Fórmula |
|---|---|
| Ohm y potencia | $V = IR$, $P = VI = I^2R = V^2/R$ |
| Kirchhoff | $\sum I = 0$ en nodos, $\sum\mathcal E = \sum IR$ en mallas |
| Capacitor | $Q = CV$, $U = \tfrac12CV^2$ |
| Serie / paralelo (C) | $1/C_{eq} = \sum1/C_i$ / $C_{eq} = \sum C_i$ |
| Energía disipada al cargar | $\tfrac12CV^2$ |
| Energía disipada al repartir | $\tfrac12\frac{C_1C_2}{C_1 + C_2}V^2$ |
| C cilíndrico | $2\pi\varepsilon_0\ell/\ln(b/a)$ |
| Coulomb | $F = kq_1q_2/r^2$, $k = 9\times10^9$ |
| Hilo finito en su eje | $E = k\lambda(1/a - 1/b)$, $V = k\lambda\ln(b/a)$ |
| Anillo en su eje | $E = kQz/(R^2 + z^2)^{3/2}$, $V = kQ/\sqrt{R^2 + z^2}$ |
| Semianillo (centro) | $E = 2k\lambda/R$ |
| Hilo infinito | $E = 2k\lambda/r$ |
| Gauss | $\oint\vec E\cdot d\vec S = Q_{enc}/\varepsilon_0$ |
| Trabajo del campo | $W = q(V_A - V_B)$ |
| Conducción | $H = kA\Delta T/L$, $R_T = L/(kA)$ |
| Rendimiento | $\eta = W/Q_{abs}$, $\eta_C = 1 - T_F/T_C$ |
| Primer principio | $\Delta U = Q - W$ |
| Calorimetría | $Q = mc\Delta T$, $Q = mL$ |

Tablas completas por tema: [Termodinámica](../1%20-%20Termodin%C3%A1mica/teoria.md#13-tabla-de-fórmulas), [Electrostática](../2%20-%20Electrost%C3%A1tica/teoria.md#15-tabla-de-fórmulas), [Electrodinámica](../3%20-%20Electrodin%C3%A1mica/teoria.md#14-tabla-de-fórmulas), [Capacitores](../4%20-%20Capacitores%20y%20Diel%C3%A9ctricos/teoria.md#17-tabla-de-fórmulas).
