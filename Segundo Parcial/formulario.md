# Formulario del 2º Parcial

Lo único que hay que memorizar para los parciales: constantes, leyes, 10 atajos y reglas de sentido. Todo lo demás (despejes, casos particulares, potencias, resonancia, radio de la órbita, $L$ y $M$, etc.) sale de acá en una línea; cómo, está en la [guía de resolución](guia-de-resolucion.md#011-atajos-para-el-día-del-parcial).

Volver al [índice de parciales](README.md).

---

## Constantes

| Qué | Valor |
|---|---|
| Permeabilidad del vacío | $\mu_0 = 4\pi\times10^{-7}$ T m/A $\quad\left(\dfrac{\mu_0}{2\pi} = 2\times10^{-7},\ \dfrac{\mu_0}{4\pi} = 10^{-7}\right)$ |
| Permitividad del vacío | $\varepsilon_0 = 8{,}85\times10^{-12}$ F/m |
| Pulsación | $\omega = 2\pi f$ |

Todo en metros antes de reemplazar. Calculadora en **radianes**.

---

## Leyes

| Ley | Fórmula |
|---|---|
| Fuerza magnética | $\vec F = q\,\vec v\times\vec B$ $\qquad \vec F = I\,\vec\ell\times\vec B$ |
| Faraday | $\mathcal E = -N\dfrac{d\phi}{dt}$, $\quad\phi = BA$ (uniforme y perpendicular), $\quad I = \dfrac{\mathcal E}{R}$ |
| Inductancia | $N\phi = LI$ $\qquad N_2\phi_2 = MI_1$ |
| Capacitor | $Q = CV$ |
| Alterna | $Z = R + j(X_L - X_C)$, $\quad X_L = \omega L$, $\quad X_C = \dfrac{1}{\omega C}$, $\quad V = ZI$ |

---

## Los 10 atajos

| # | Atajo |
|---|---|
| 1 | **Tramo recto:** $B = \dfrac{\mu_0 I}{4\pi d}(\mathrm{sen}\,\beta_2 - \mathrm{sen}\,\beta_1)$. Hilo infinito $\dfrac{\mu_0 I}{2\pi d}$; semi-infinito con P frente a su extremo $\dfrac{\mu_0 I}{4\pi d}$; P sobre la prolongación $0$ |
| 2 | **Arco centrado en P:** $B = \dfrac{\mu_0 I\theta}{4\pi R}$. Espira circular $\dfrac{\mu_0 I}{2R}$ |
| 3 | **Anillo en su eje:** $B = \dfrac{\mu_0 IR^2}{2(R^2 + z^2)^{3/2}}$ |
| 4 | **Solenoide:** $B = \mu_0 nI$, $\ n = N/\ell$ |
| 5 | **Hilo y logaritmo:** flujo en una espira $\phi = \dfrac{\mu_0 Ic}{2\pi}\ln\dfrac{x_2}{x_1}$; barra junto al hilo $\mathcal E = \dfrac{\mu_0 Iv}{2\pi}\ln\dfrac{d + \ell}{d}$ |
| 6 | **Barra que gira:** $\mathcal E = \tfrac12B\omega r_0^2$ |
| 7 | **Energía magnética:** $U = \tfrac12LI^2 = \dfrac{B^2}{2\mu_0}\cdot\text{volumen}$ |
| 8 | **Energía de un capacitor:** $U = \tfrac12CV^2$; la fuente entrega $QV$ (se disipa la mitad) |
| 9 | **Eficaces y potencia:** $V_{EF} = \dfrac{V_0}{\sqrt2}$, $\ P = V_{EF}I_{EF}\cos\varphi = I_{EF}^2R$ |
| 10 | **Capacitor cilíndrico:** $C = \dfrac{2\pi\varepsilon_0\ell}{\ln(b/a)}$ |

Imprescindibles: **1**, **2** y **4**.

---

## Reglas de sentido

| Situación | Regla |
|---|---|
| Campo de un hilo | pulgar = corriente, dedos = $\vec B$ (corriente hacia arriba: a la derecha ⊗, a la izquierda ⊙) |
| Campo de espira, arco o solenoide | dedos = corriente, pulgar = $\vec B$ (antihoraria → ⊙, horaria → ⊗) |
| Versores | $\hat x\times\hat y = \hat z$, $\ \hat y\times\hat z = \hat x$, $\ \hat z\times\hat x = \hat y$ |
| Lenz | la corriente inducida se opone al cambio de flujo |
| Polaridad de una barra | mayor potencial en el extremo hacia el que apunta $\vec v\times\vec B$ |
| Alterna | $X_L > X_C$: inductivo, la tensión adelanta. $X_C > X_L$: capacitivo, la corriente adelanta |
