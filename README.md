# Teoría — Espacios Métricos y Topológicos

Apunte compilado de **Espacios Métricos y Topológicos** (Licenciatura en Matemática,
**Universidad CAECE**, cursada 2026), con las definiciones, proposiciones y teoremas
de la materia y las resoluciones de los ejercicios de las guías.

El material cruza tres fuentes: las clases, la **guía teórica de la cátedra**
(*Topología: Espacios Métricos y Topológicos*, curso 2011/2012) y los apuntes de
**Marta Macho Stadler, _Topología_ (2014)**. Está pensado para **estudiar y practicar
memoria espaciada**: cada enunciado aparece dos veces, **en lenguaje natural y como
predicado en lenguaje lógico**, y al final hay una lista por parcial con todo lo que
hay que saber enunciar y demostrar.

## Contenido

El apunte (`03-apunte/Topologia-apunte-compilado.pdf`, 104 páginas) tiene 11 secciones y
cubre **toda la guía teórica** (caps. 1–4), con lo dictado en clase hasta la clase 13 (5/10/2026). Cada enunciado indica la **ubicación exacta en la fuente** (numeración y página), y se
distingue qué es definición (se admite), qué es proposición o teorema (hay que saber
demostrarlo) y qué es ejemplo o contraejemplo.

**Primer parcial**
1. Espacios métricos y normados: normas, producto interno, Cauchy–Schwarz, distancias entre funciones, fabricación de métricas, distancia a un conjunto, bolas
2. La topología de un espacio métrico: interior, adherencia, frontera y cerrados leídos con bolas
3. Espacios topológicos: interior, clausura, acumulación, frontera, densidad, operadores de Kuratowski
4. Bases, subbases y comparación de topologías; entornos y bases locales
5. Axiomas de separación T₀, T₁, T₂
6. Sucesiones y convergencia; unicidad del límite; clausura por sucesiones
7. Continuidad: en un punto, global, álgebra de continuas, continuidad uniforme, la distancia es continua, homeomorfismos, inmersiones
8. Topología de subespacio y su propiedad universal

**Segundo parcial**

9. Topología producto: base de rectángulos, proyecciones (continuas, abiertas, no cerradas), continuidad hacia un producto, clausura e interior de un producto
10. Conexidad: abiertos-cerrados, imagen continua, funciones a un discreto, dos puntos en un conexo, uniones y clausura de conexos, frontera, totalmente disconexos, peine del topólogo, producto de conexos; intervalos de ℝ y Bolzano; conexión por caminos, la relación "estar conectados" y uniones de arcoconexos, componentes conexas y por caminos, conexión local, invarianza por homeomorfismos (contar componentes y puntos de corte), conexo + localmente arcoconexo ⇒ arcoconexo
11. Compacidad: recubrimientos y subrecubrimientos, no compacto, finitos y discretos, [a,b] compacto, compacto ⇒ acotado, cerrados y Hausdorff, imagen continua y Weierstrass, lema del tubo y Tychonoff finito, compacidad en métricos (Heine–Borel, Bolzano–Weierstrass, número de Lebesgue, Heine), completitud, compacidad local

**Apéndices**
- A. Mapa de los ejercicios de las guías y la herramienta que usa cada uno
- B. Lista para el primer parcial
- C. Lista para el segundo parcial: producto, conexidad, intervalos y Bolzano, caminos, componentes y puntos de corte, y compacidad
- D. Glosario de notación
- E. Catálogo de topologías de referencia, con una tabla de separación, metrizabilidad y conexidad

Las cajas naranjas de **Intuición** y las figuras (TikZ) fijan la imagen mental antes
del enunciado formal; no son contenido evaluable.

## Ejercicios resueltos

`03-apunte/Topologia-ejercicios-resueltos.pdf` resuelve los ejercicios de las guías
cuya técnica es reutilizable o cuyo contraejemplo conviene tener a mano: espacios
métricos (A, C y producto interno), espacios topológicos (A, D, bases, separación),
continuidad (A y B), productos (1–3) y conexidad (1–14, más el peine del topólogo).

## Estructura del repositorio

```
.
└── 03-apunte/
    ├── Topologia-apunte-compilado.tex        # Apunte: teoría + apéndices
    ├── Topologia-apunte-compilado.pdf        # PDF compilado
    ├── Topologia-ejercicios-resueltos.tex    # Resoluciones de las guías
    └── Topologia-ejercicios-resueltos.pdf    # PDF compilado
```

## Cómo compilar

Requiere una distribución de LaTeX (TeX Live / MacTeX) con `pdflatex`.

```bash
cd 03-apunte
pdflatex Topologia-apunte-compilado.tex   # primera pasada
pdflatex Topologia-apunte-compilado.tex   # segunda pasada (índice y referencias)
```

Lo mismo para `Topologia-ejercicios-resueltos.tex`. No se usa `babel`; en una
instalación completa conviene agregar `\usepackage[spanish]{babel}` al preámbulo para
la partición de palabras.

## Notas

- Las fuentes (guía teórica, libro de Macho Stadler, guías de ejercicios y apuntes de
  la cátedra, notas de clase) **no** se incluyen en el repositorio por tratarse de
  material de terceros; el apunte sólo cita numeraciones y páginas.
- Las figuras están hechas con **TikZ**.
- Material de estudio sin fines de lucro.
