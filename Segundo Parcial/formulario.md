# Formulario del 2º Parcial

Todas las fórmulas y constantes que se usan en los parciales, sin deducciones. Las deducciones están en la [guía de resolución](guia-de-resolucion.md).

Volver al [índice de parciales](README.md).

---

## Constantes y unidades

| Qué | Valor |
|---|---|
| Permeabilidad del vacío | $\mu_0 = 4\pi\times10^{-7}$ T m/A |
| | $\dfrac{\mu_0}{2\pi} = 2\times10^{-7}$ T m/A $\qquad \dfrac{\mu_0}{4\pi} = 10^{-7}$ T m/A |
| Permitividad del vacío | $\varepsilon_0 = 8{,}85\times10^{-12}$ F/m |
| Pulsación | $\omega = 2\pi f$ $\quad$ (50 Hz → $\omega = 100\pi$ rad/s) |
| Unidad imaginaria | $j = \sqrt{-1}$ |
| Prefijos | m = $10^{-3}$, μ = $10^{-6}$, n = $10^{-9}$ |

Unidades: B en T, flujo en Wb = T m², fem en V, L y M en H, C en F, R, X y Z en Ω, P en W, Q en VAR, S en VA.

Pasar todo a metros antes de reemplazar. Calculadora en **radianes** para $\mathrm{sen}\,(\omega t)$.

---

## Sentidos

| Situación | Regla |
|---|---|
| Campo de un hilo | pulgar = corriente, dedos = $\vec B$. Hilo vertical con corriente hacia arriba: a la derecha ⊗, a la izquierda ⊙ |
| Campo de espira, arco o solenoide | dedos = corriente, pulgar = $\vec B$. Antihoraria → ⊙, horaria → ⊗ |
| Campo de un elemento | sentido de $d\vec l\times\hat r$ ($\hat r$ va del cable al punto) |
| Versores | $\hat x\times\hat y = \hat z$, $\ \hat y\times\hat z = \hat x$, $\ \hat z\times\hat x = \hat y$ (al invertir el orden cambia el signo) |
| Corriente inducida (Lenz) | se opone al cambio de flujo: flujo ⊗ que crece → antihoraria; flujo ⊗ que decrece → horaria |
| Polaridad de una barra | el extremo hacia el que apunta $\vec v\times\vec B$ está a **mayor** potencial |
| Fuerza sobre la barra | siempre frena; agente externo $= -\vec F_M$ si $v$ es constante |

---

## Campo magnético

| Caso | Fórmula |
|---|---|
| Tramo recto (P a distancia $d$ de la recta) | $B = \dfrac{\mu_0 I}{4\pi d}(\mathrm{sen}\,\beta_2 - \mathrm{sen}\,\beta_1)$, con $\mathrm{sen}\,\beta = \dfrac{x}{\sqrt{x^2 + d^2}}$ medido desde el pie de la perpendicular, con signo |
| Hilo infinito | $B = \dfrac{\mu_0 I}{2\pi d}$ |
| Semi-infinito, P frente a su extremo | $B = \dfrac{\mu_0 I}{4\pi d}$ |
| P sobre la prolongación de un tramo | $B = 0$ |
| Arco de ángulo $\theta$ (radianes), en su centro | $B = \dfrac{\mu_0 I\theta}{4\pi R}$ |
| Semicircunferencia, en su centro | $B = \dfrac{\mu_0 I}{4R}$ |
| Espira circular, en su centro | $B = \dfrac{\mu_0 I}{2R}$ |
| Espira circular, en su eje a distancia $z$ | $B = \dfrac{\mu_0 IR^2}{2(R^2 + z^2)^{3/2}}$ |
| Espira rectangular $a\times b$, en su centro | $B = \dfrac{2\mu_0 I\sqrt{a^2 + b^2}}{\pi ab}$ |
| Espira cuadrada de lado $D$, en su centro | $B = \dfrac{2\sqrt2\,\mu_0 I}{\pi D}$ |
| Lado de largo $\ell$ visto desde su mediatriz | $B = \dfrac{\mu_0 I}{4\pi d}\cdot\dfrac{\ell}{\sqrt{(\ell/2)^2 + d^2}}$ |
| Solenoide largo ($n = N/\ell$) | $B = \mu_0 nI = \mu_0\dfrac N\ell I$ adentro, uniforme; $\approx 0$ afuera |

**Hilos paralelos, campo nulo:**

| Corrientes | Entre los hilos | Afuera |
|---|---|---|
| Paralelas | puede haber cero | nunca cero |
| Antiparalelas | nunca cero | cero del lado del hilo con **menos** corriente |

Condición de cero: $\dfrac{I_1}{d_1} = \dfrac{I_2}{d_2}$.

---

## Fuerzas y movimiento

| Caso | Fórmula |
|---|---|
| Carga puntual | $\vec F = q\,\vec v\times\vec B$ (con el signo de $q$); $\ \lvert F\rvert = \lvert q\rvert vB\,\mathrm{sen}\,\theta$ |
| Tramo recto en campo uniforme | $\vec F = I\,\vec\ell\times\vec B$ |
| Entre dos hilos paralelos | $\dfrac F\ell = \dfrac{\mu_0 I_1I_2}{2\pi D}$; paralelas se atraen, antiparalelas se repelen |
| Radio de la órbita | $r = \dfrac{mv_\perp}{\lvert q\rvert B}$ |
| Período | $T = \dfrac{2\pi m}{\lvert q\rvert B}$ (no depende de $v$) |
| Componentes | $v_\perp = v\,\mathrm{sen}\,\theta$, $\ v_\parallel = v\cos\theta$ ($\theta$ entre $\vec v$ y $\vec B$) |
| Paso de la hélice | $p = v_\parallel T = \dfrac{2\pi m\,v\cos\theta}{\lvert q\rvert B}$ |
| Trabajo de la fuerza magnética | $W = 0$: el módulo de $\vec v$ no cambia nunca |

---

## Inducción

| Caso | Fórmula |
|---|---|
| Faraday | $\mathcal E = -N\dfrac{d\phi}{dt}$, $\ I = \dfrac{\mathcal E}{R}$ |
| Flujo uniforme | $\phi = BA\cos\theta$ |
| Bobina quieta con $B(t)$ | $\lvert\mathcal E\rvert = NA\left\lvert\dfrac{dB}{dt}\right\rvert$ |
| Vueltas a partir del alambre | $N = \dfrac{\text{largo del alambre}}{2\pi r}$, $\ r = \sqrt{A/\pi}$ |
| Flujo de un hilo en una espira coplanar (lado paralelo $c$, de $x_1$ a $x_2$) | $\phi = \dfrac{\mu_0 Ic}{2\pi}\ln\dfrac{x_2}{x_1}$ |
| Ídem con $I(t)$ | $\lvert\mathcal E\rvert = \dfrac{\mu_0 c}{2\pi}\ln\dfrac{x_2}{x_1}\left\lvert\dfrac{dI}{dt}\right\rvert$ |
| Ídem, espira que se aleja a $v$ (ancho $b$, a distancia $x$) | $\lvert\mathcal E\rvert = \dfrac{\mu_0 Ic}{2\pi}\cdot\dfrac{bv}{x(x + b)}$ |
| Barra sobre rieles, $B$ uniforme | $\mathcal E = B\ell v$ |
| Barra sobre rieles, $B(x)$ | $\mathcal E = B(x)\,\ell v$ |
| Barra junto a un hilo, moviéndose paralela a él | $\mathcal E = \dfrac{\mu_0 Iv}{2\pi}\ln\dfrac{d + \ell}{d}$ |
| Barra que gira alrededor de un extremo | $\mathcal E = \tfrac12B\omega r_0^2$ |
| Barra que gira alrededor de un punto interior O | $V_P - V_Q = \tfrac12B\omega(OQ^2 - OP^2)$ en módulo; las dos mitades se restan |

---

## Inductancia y energía magnética

| Caso | Fórmula |
|---|---|
| Definición | $N\phi = LI$, $\ N_2\phi_2 = MI_1$ |
| Fem autoinducida | $\mathcal E = -L\dfrac{dI}{dt}$ |
| L de un solenoide | $L = \mu_0\dfrac{N^2}{\ell}A = \mu_0 n^2A\ell$, $\ A = \pi R^2$ |
| M de dos solenoides coaxiales de igual largo | $M = \mu_0\dfrac{N_1N_2}{\ell}A_{\text{menor}}$ |
| Energía | $U = \tfrac12LI^2$ |
| Energía en un solenoide | $U = \dfrac{B^2}{2\mu_0}\cdot A\ell$ (densidad $u = \dfrac{B^2}{2\mu_0}$) |
| Longitud de un solenoide con L, I, B, R | $\ell = \dfrac{\mu_0 LI^2}{B^2\pi R^2}$ |

---

## Capacitores

| Caso | Fórmula |
|---|---|
| Definición | $Q = CV$ |
| Energía | $U = \tfrac12CV^2 = \dfrac{Q^2}{2C} = \tfrac12QV$ |
| Energía que entrega una fuente al cargar | $W = QV = CV^2$ |
| Energía disipada al cargar desde una fuente | $\tfrac12CV^2$ (la mitad) |
| Paralelo | $C_{eq} = \sum C_i$ (misma tensión) |
| Serie | $\dfrac{1}{C_{eq}} = \sum\dfrac{1}{C_i}$ (misma carga) |
| Reparto (capacitor cargado conectado a descargados) | $V_f = \dfrac{Q_0}{\sum C}$, $\ Q_i = C_iV_f$ |
| Energía disipada en el reparto | $U_{antes} - U_{después}$ |
| Capacitor cilíndrico (radios $a < b$) | $C = \dfrac{2\pi\varepsilon_0\ell}{\ln(b/a)}$ |

---

## Corriente alterna (RLC serie)

| Caso | Fórmula |
|---|---|
| Reactancias | $X_L = \omega L$, $\ X_C = \dfrac{1}{\omega C}$ |
| Impedancia compleja | $Z = R + j(X_L - X_C)$ |
| Módulo | $Z = \sqrt{R^2 + (X_L - X_C)^2} = \dfrac{V_0}{I_0} = \dfrac{V_{EF}}{I_{EF}}$ |
| Fase | $\tan\varphi = \dfrac{X_L - X_C}{R}$, $\ \cos\varphi = \dfrac RZ$, $\ \mathrm{sen}\,\varphi = \dfrac{X_L - X_C}{Z}$ |
| Despejes del triángulo | $R = Z\cos\varphi$, $\ \lvert X_L - X_C\rvert = Z\,\mathrm{sen}\,\varphi = \sqrt{Z^2 - R^2} = R\tan\varphi$ |
| Inductivo | $X_L > X_C$, $\varphi > 0$, la tensión adelanta, $\omega > \omega_0$ |
| Capacitivo | $X_C > X_L$, $\varphi < 0$, la corriente adelanta, $\omega < \omega_0$ |
| Resonancia | $\omega_0 = \dfrac{1}{\sqrt{LC}}$, $\ f_0 = \dfrac{1}{2\pi\sqrt{LC}}$; ahí $Z = R$ y $\varphi = 0$ |
| Despejes de la resonancia | $C = \dfrac{1}{\omega_0^2L}$, $\ L = \dfrac{1}{\omega_0^2C}$ |
| Reactancia con $\omega_0$ como dato | $X_L - X_C = L\,\dfrac{\omega^2 - \omega_0^2}{\omega}$ |
| Tensión en cada elemento | $V_R = RI$, $\ V_L = X_LI$, $\ V_C = X_CI$; $\ V = \sqrt{V_R^2 + (V_L - V_C)^2}$ |
| Eficaces | $V_{EF} = \dfrac{V_0}{\sqrt2}$, $\ I_{EF} = \dfrac{I_0}{\sqrt2}$ (amperímetro y voltímetro miden eficaces) |
| Potencia activa | $P = V_{EF}I_{EF}\cos\varphi = I_{EF}^2R = \tfrac12V_0I_0\cos\varphi = \tfrac12I_0^2R$ [W] |
| Potencia reactiva | $Q = V_{EF}I_{EF}\,\mathrm{sen}\,\varphi = I_{EF}^2(X_L - X_C)$ [VAR] |
| Potencia aparente | $S = V_{EF}I_{EF} = I_{EF}^2Z = \sqrt{P^2 + Q^2}$ [VA] |
| Factor de potencia | $\cos\varphi = \dfrac PS = \dfrac RZ$ |
| Z a partir de S | $Z = \dfrac{S}{I_{EF}^2}$ |
| R a partir de P | $R = \dfrac{P}{I_{EF}^2} = \dfrac{2P}{I_0^2}$ |
| Dos capacitores para una reactancia neta $X$ | $X_C = X_L - X$ (queda inductivo, si da $> 0$) o $X_C = X_L + X$ (queda capacitivo) |
| Cambiar C sin cambiar el factor de potencia | $X'_C = 2X_L - X_C$ |
| Cociente de capacitores a igual $\omega$ | $\dfrac{C'}{C} = \dfrac{X_C}{X'_C}$ |
| Aumentar C | baja $X_C$ → más inductivo. Aumentar L → más inductivo |
| Dos elementos con disipación | tensión adelantada → R y L; atrasada → R y C |
