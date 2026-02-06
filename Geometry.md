# জ্যামিতি (Geometry) - BDMO প্রস্তুতি গাইড

## সূচিপত্র
1. [মৌলিক ধারণা - Points, Lines, Polygons](#মৌলিক-ধারণা)
2. [Trigonometry](#trigonometry)
3. [Triangle Centers](#triangle-centers)
4. [Ceva এবং Menelaus Theorems](#ceva-এবং-menelaus-theorems)
5. [Quadrilaterals](#quadrilaterals)
6. [Circle Geometry](#circle-geometry)
7. [বিশেষ Theorems](#বিশেষ-theorems)
8. [Coordinate Geometry](#coordinate-geometry)
9. [Complex Number Geometry](#complex-number-geometry)
10. [Barycentric Coordinates](#barycentric-coordinates)
11. [Inversion Geometry](#inversion-geometry)
12. [Projective Geometry](#projective-geometry)

---

## মৌলিক ধারণা

### Points এবং Lines

#### Point:
একটি exact location যার কোনো dimension নেই।

#### Line:
দুটি point দিয়ে একটি unique line তৈরি হয়।

**Distance formula:** দুটি point A(x₁, y₁) এবং B(x₂, y₂) এর মধ্যে দূরত্ব:

**d = √[(x₂ - x₁)² + (y₂ - y₁)²]**

#### Collinearity:

তিনটি point A, B, C collinear হয় যদি:
- Area of triangle ABC = 0
- Slope AB = Slope BC

---

### Polygons

#### Triangle:

তিন বাহু বিশিষ্ট polygon।

**Properties:**
- Sum of angles = 180°
- Sum of two sides > third side (Triangle Inequality)
- Exterior angle = sum of opposite interior angles

**Area formulas:**

1. **Base-Height:** A = (1/2) × base × height

2. **Heron's Formula:** 
   - s = (a + b + c)/2 (semi-perimeter)
   - **A = √[s(s-a)(s-b)(s-c)]**

3. **Using two sides and included angle:**
   - **A = (1/2)ab sin(C)**

4. **Circumradius formula:**
   - **A = abc/(4R)**

5. **Inradius formula:**
   - **A = rs** যেখানে r = inradius

---

#### Types of Triangles:

**By sides:**
- Equilateral: সব বাহু সমান
- Isosceles: দুটি বাহু সমান
- Scalene: সব বাহু ভিন্ন

**By angles:**
- Acute: সব angle < 90°
- Right: একটি angle = 90°
- Obtuse: একটি angle > 90°

---

#### Quadrilaterals:

চার বাহু বিশিষ্ট polygon।

**Properties:**
- Sum of angles = 360°

**Types:**
- Square: সব বাহু সমান, সব angle = 90°
- Rectangle: opposite বাহু সমান, সব angle = 90°
- Rhombus: সব বাহু সমান
- Parallelogram: opposite বাহু parallel ও সমান
- Trapezoid: একজোড়া বাহু parallel
- Kite: দুই জোড়া adjacent বাহু সমান

---

#### Regular Polygons:

n বাহু বিশিষ্ট regular polygon এর:

**Sum of interior angles:** (n - 2) × 180°

**Each interior angle:** (n - 2) × 180° / n

**Each exterior angle:** 360° / n

**Area (side = a):** 
- **A = (na²)/(4 tan(180°/n))**

**Area (circumradius = R):**
- **A = (nR²/2) sin(360°/n)**

---

## Trigonometry

### মৌলিক Ratios:

একটি right triangle এ angle θ এর জন্য:

```
        |\
        | \  hypotenuse
opposite|  \
        |   \
        |____\
       adjacent
```

- **sin(θ) = opposite/hypotenuse**
- **cos(θ) = adjacent/hypotenuse**
- **tan(θ) = opposite/adjacent**
- **csc(θ) = 1/sin(θ)**
- **sec(θ) = 1/cos(θ)**
- **cot(θ) = 1/tan(θ)**

---

### Pythagorean Identity:

**sin²(θ) + cos²(θ) = 1**

**Other forms:**
- 1 + tan²(θ) = sec²(θ)
- 1 + cot²(θ) = csc²(θ)

---

### বিশেষ Angles:

| Angle | sin | cos | tan |
|-------|-----|-----|-----|
| 0° | 0 | 1 | 0 |
| 30° | 1/2 | √3/2 | 1/√3 |
| 45° | 1/√2 | 1/√2 | 1 |
| 60° | √3/2 | 1/2 | √3 |
| 90° | 1 | 0 | ∞ |

---

### Sum এবং Difference Formulas:

**sin(A ± B) = sin(A)cos(B) ± cos(A)sin(B)**

**cos(A ± B) = cos(A)cos(B) ∓ sin(A)sin(B)**

**tan(A ± B) = [tan(A) ± tan(B)]/[1 ∓ tan(A)tan(B)]**

---

### Double Angle Formulas:

**sin(2A) = 2sin(A)cos(A)**

**cos(2A) = cos²(A) - sin²(A) = 2cos²(A) - 1 = 1 - 2sin²(A)**

**tan(2A) = 2tan(A)/[1 - tan²(A)]**

---

### Half Angle Formulas:

**sin(A/2) = ±√[(1 - cos(A))/2]**

**cos(A/2) = ±√[(1 + cos(A))/2]**

**tan(A/2) = sin(A)/[1 + cos(A)] = [1 - cos(A)]/sin(A)**

---

### Product-to-Sum Formulas:

**sin(A)sin(B) = [cos(A-B) - cos(A+B)]/2**

**cos(A)cos(B) = [cos(A-B) + cos(A+B)]/2**

**sin(A)cos(B) = [sin(A+B) + sin(A-B)]/2**

---

### Sine Rule:

একটি triangle ABC তে:

**a/sin(A) = b/sin(B) = c/sin(C) = 2R**

যেখানে R = circumradius

---

### Cosine Rule:

**a² = b² + c² - 2bc cos(A)**

**b² = a² + c² - 2ac cos(B)**

**c² = a² + b² - 2ab cos(C)**

**Alternative form:**

**cos(A) = (b² + c² - a²)/(2bc)**

---

### Tangent Rule (Napier's Analogy):

**tan[(A-B)/2] = [(a-b)/(a+b)] cot(C/2)**

---

### Projection Formula:

**a = b cos(C) + c cos(B)**

**b = a cos(C) + c cos(A)**

**c = a cos(B) + b cos(A)**

---

### Triangle এ Trigonometric Relations:

**Area = (1/2)ab sin(C) = (1/2)bc sin(A) = (1/2)ca sin(B)**

**Area = 2R² sin(A) sin(B) sin(C)**

**tan(A) + tan(B) + tan(C) = tan(A)tan(B)tan(C)** (triangle এ)

**sin(A) + sin(B) + sin(C) = 4cos(A/2)cos(B/2)cos(C/2)**

---

## Triangle Centers

### 1. Circumcenter (O)

**সংজ্ঞা:** Triangle এর তিন বাহুর perpendicular bisectors এর intersection point।

**বৈশিষ্ট্য:**
- Triangle এর সব vertices থেকে সমান দূরত্বে
- OA = OB = OC = R (circumradius)
- Triangle এর circumcircle এর center

**অবস্থান:**
- Acute triangle: ভিতরে
- Right triangle: hypotenuse এর midpoint এ
- Obtuse triangle: বাইরে

**Circumradius formula:**

**R = a/(2sin(A)) = b/(2sin(B)) = c/(2sin(C))**

**R = abc/(4×Area)**

---

### 2. Incenter (I)

**সংজ্ঞা:** Triangle এর তিন angle bisectors এর intersection point।

**বৈশিষ্ট্য:**
- Triangle এর তিন বাহু থেকে সমান দূরত্বে
- সবসময় triangle এর ভিতরে থাকে
- Incircle এর center

**Inradius formula:**

**r = Area/s** যেখানে s = semi-perimeter

**r = (s - a)tan(A/2) = (s - b)tan(B/2) = (s - c)tan(C/2)**

**r = 4R sin(A/2)sin(B/2)sin(C/2)**

**Distance from vertices:**

**IA = r/sin(A/2) = 4R sin(B/2)sin(C/2)**

---

### 3. Orthocenter (H)

**সংজ্ঞা:** Triangle এর তিন altitudes এর intersection point।

**বৈশিষ্ট্য:**
- Altitudes হলো vertex থেকে opposite বাহুতে perpendicular

**অবস্থান:**
- Acute triangle: ভিতরে
- Right triangle: right angle vertex এ
- Obtuse triangle: বাইরে

**Distance formula:**

**OH² = R² - 8R² cos(A)cos(B)cos(C)**

---

### 4. Centroid (G)

**সংজ্ঞা:** Triangle এর তিন medians এর intersection point।

**বৈশিষ্ট্য:**
- Median হলো vertex থেকে opposite বাহুর midpoint পর্যন্ত line segment
- সবসময় triangle এর ভিতরে থাকে
- Median কে 2:1 ratio তে ভাগ করে

**Distance from vertex:**
- **GA:AA' = 2:1** (যেখানে A' হলো BC এর midpoint)

**Coordinates:**
যদি vertices হয় A(x₁, y₁), B(x₂, y₂), C(x₃, y₃):

**G = ((x₁ + x₂ + x₃)/3, (y₁ + y₂ + y₃)/3)**

**Median length:**

**mₐ = (1/2)√(2b² + 2c² - a²)**

---

### Euler Line

**Important theorem:** একটি non-equilateral triangle এ Centroid (G), Circumcenter (O), এবং Orthocenter (H) একই সরলরেখায় থাকে।

এই line টিকে **Euler Line** বলে।

**Relation:** G দিয়ে Euler line কে ভাগ করলে:

**OG:GH = 1:2**

অর্থাৎ: **OG = GH/2**

অথবা: **\vec{OG} = (1/3)\vec{OH}**

**Note:** Equilateral triangle এ O, G, H এক point এ মিলিত হয়।

---

### Nine-Point Center (N)

Nine-point circle টি এই 9টি point দিয়ে যায়:
1. তিন বাহুর midpoints (3)
2. তিন altitudes এর feet (3)
3. Orthocenter থেকে তিন vertices এর midpoints (3)

**বৈশিষ্ট্য:**
- Nine-point center (N) Euler line এ থাকে
- Nine-point circle এর radius = R/2
- **ON:NH = 1:2**

---

## Ceva এবং Menelaus Theorems

### Ceva's Theorem

**Statement:** Triangle ABC তে তিনটি cevians AD, BE, CF concurrent হয় যদি এবং কেবলমাত্র যদি:

**(AF/FB) × (BD/DC) × (CE/EA) = 1**

```
        A
       /|\
      / | \
     /  |  \
    /   P   \
   /   /|\   \
  /  /  |  \  \
 / /    |    \ \
//______|_____\\
B   D   |   E   C
        F
```

যেখানে P হলো concurrent point (cevians এর intersection)।

**প্রমাণ:** Area ratios ব্যবহার করে prove করা যায়।

---

### Menelaus's Theorem

**Statement:** Triangle ABC এবং একটি transversal line যা বাহুগুলোকে D, E, F তে কাটে। তাহলে:

**(AF/FB) × (BD/DC) × (CE/EA) = -1**

Negative sign নির্দেশ করে যে directed ratios consider করতে হবে।

```
        A
       /  \
      /    \
     /      \
    E________F____
   /          \
  /            \
 /              \
B_______D________C
```

**Note:** Points D, E, F collinear হলেই এই theorem apply হয়।

---

### Applications:

**Ceva's Theorem দিয়ে prove করা যায়:**
- Medians concurrent
- Angle bisectors concurrent
- Altitudes concurrent

**উদাহরণ - Medians concurrent:**

যদি D, E, F হয় midpoints, তাহলে:
- AF/FB = 1
- BD/DC = 1
- CE/EA = 1

Product = 1 × 1 × 1 = 1 ✓

---

## Quadrilaterals

### Parallelogram

**Properties:**
- Opposite sides parallel এবং সমান
- Opposite angles সমান
- Diagonals একে অপরকে bisect করে
- Consecutive angles supplementary (sum = 180°)

**Area = base × height = ab sin(θ)** যেখানে θ = angle between sides

---

### Rectangle

**Properties:**
- সব angles = 90°
- Diagonals সমান এবং একে অপরকে bisect করে

**Area = length × width**

**Diagonal = √(l² + w²)**

---

### Rhombus

**Properties:**
- সব sides সমান
- Diagonals perpendicular এবং একে অপরকে bisect করে
- Diagonals angle bisectors

**Area = (1/2) × d₁ × d₂** যেখানে d₁, d₂ = diagonals

**Area = a² sin(θ)** যেখানে a = side, θ = angle

---

### Square

**Properties:**
- সব sides সমান
- সব angles = 90°
- Diagonals সমান, perpendicular, এবং bisect করে

**Area = a²**

**Diagonal = a√2**

---

### Trapezoid

**Properties:**
- একজোড়া opposite sides parallel

**Midsegment = (b₁ + b₂)/2** যেখানে b₁, b₂ = parallel sides

**Area = (1/2)(b₁ + b₂) × h** যেখানে h = height

---

### Cyclic Quadrilateral

একটি quadrilateral যার সব vertices একটি circle এর উপর থাকে।

**Ptolemy's Theorem:** (পরে আলোচনা করা হবে)

**Brahmagupta's Formula (Area):**

যদি sides হয় a, b, c, d এবং s = (a+b+c+d)/2:

**Area = √[(s-a)(s-b)(s-c)(s-d)]**

**বৈশিষ্ট্য:**
- Opposite angles এর sum = 180°
- ∠A + ∠C = 180°, ∠B + ∠D = 180°

---

## Circle Geometry

### মৌলিক সংজ্ঞা:

**Circle:** একটি fixed point (center) থেকে সমান দূরত্বে থাকা সব points এর locus।

**Radius (r):** Center থেকে circle এর যেকোনো point এর দূরত্ব

**Diameter (d):** d = 2r

**Chord:** Circle এর দুটি point যুক্ত করা line segment

**Secant:** Circle কে দুই জায়গায় কাটে এমন line

**Tangent:** Circle কে ঠিক এক জায়গায় স্পর্শ করে এমন line

**Arc:** Circle এর একটি অংশ

**Sector:** দুটি radii এবং একটি arc দ্বারা আবদ্ধ অংশ

**Segment:** একটি chord এবং একটি arc দ্বারা আবদ্ধ অংশ

---

### Circle Theorems:

#### 1. Tangent-Radius Theorem:

**Tangent সবসময় radius এর সাথে perpendicular থাকে contact point এ।**

যদি PT tangent হয় point T তে, তাহলে OT ⊥ PT

---

#### 2. Two Tangents from External Point:

একটি external point থেকে circle এ দুটি tangent টানা হলে:
- দুটি tangent segments সমান
- Center থেকে point এর দূরত্ব tangent segments এর angle bisect করে

**PA = PB** যেখানে A, B হলো tangent points

---

#### 3. Inscribed Angle Theorem:

**একটি arc এর উপর inscribed angle = central angle এর অর্ধেক**

যদি ∠AOB = θ (central angle), তাহলে ∠ACB = θ/2 (inscribed angle)

```
      A
     /|\
    / | \
   /  O  \
  /   |   \
 /    |    \
C_____|_____B
```

---

#### 4. Angles in Same Segment:

একই arc এর উপর সব inscribed angles সমান।

---

#### 5. Angle in Semicircle:

**Diameter এর উপর inscribed angle = 90°**

যদি AB diameter হয়, তাহলে ∠ACB = 90° (C circle এর উপর যেকোনো point)

---

#### 6. Cyclic Quadrilateral Theorem:

**Opposite angles এর sum = 180°**

∠A + ∠C = 180°
∠B + ∠D = 180°

**Converse:** যদি একটি quadrilateral এ opposite angles এর sum = 180°, তাহলে এটি cyclic।

---

#### 7. Tangent-Chord Angle:

**Tangent এবং chord এর মধ্যে angle = inscribed angle (একই arc এর জন্য)**

---

#### 8. Power of a Point:

একটি point P থেকে circle এ secant বা tangent টানা হলে:

**যদি secant PAB হয়:** PA × PB = constant (power of point)

**যদি tangent PT হয়:** PT² = PA × PB

```
    P
   /|\
  / | \
 /  |  \
A___O___B
    |
    T
```

PT² = PA × PB = power of P

---

#### 9. Intersecting Chords:

দুটি chord AB এবং CD যদি point P তে intersect করে:

**PA × PB = PC × PD**

```
A___P___B
    X
C___P___D
```

---

### Circle Formulas:

**Circumference = 2πr**

**Area = πr²**

**Arc length = (θ/360°) × 2πr = rθ** (θ in radians)

**Sector area = (θ/360°) × πr² = (1/2)r²θ**

**Segment area = (1/2)r²(θ - sin θ)**

**Chord length = 2r sin(θ/2)** যেখানে θ = central angle

---

## বিশেষ Theorems

### 1. Stewart's Theorem

Triangle ABC তে যদি cevian AD থাকে (D on BC), তাহলে:

**b² · BD + c² · DC - AD² · BC = BC · BD · DC**

অথবা: **man + dad = bmb + cnc**

যেখানে:
- m = AD (cevian)
- a = BC
- n = BD
- d = DC
- b = AC
- c = AB

**Simplified form যখন D হলো midpoint:**

**AD² = (2b² + 2c² - a²)/4**

এটি median length formula।

---

### 2. Ptolemy's Theorem

**Cyclic quadrilateral ABCD তে:**

**AC × BD = AB × CD + AD × BC**

অর্থাৎ: **diagonals এর product = opposite sides এর products এর sum**

```
A_______B
|\     /|
| \   / |
|  \ /  |
|   X   |
|  / \  |
| /   \ |
|/_____\|
D       C
```

**Corollary:** যদি ABCD একটি rectangle হয়, তাহলে diagonals সমান এবং Pythagorean theorem পাওয়া যায়।

---

### 3. Nine-Point Circle Theorem

একটি triangle এর nine-point circle এই 9টি point দিয়ে যায়:

1. **তিন বাহুর midpoints:** Mₐ, M_b, M_c
2. **তিন altitudes এর feet:** Hₐ, H_b, H_c
3. **Euler points:** Orthocenter H থেকে vertices A, B, C এর midpoints

**বৈশিষ্ট্য:**
- Radius = R/2 (যেখানে R = circumradius)
- Center N হলো Euler line এ
- Nine-point circle incircle কে স্পর্শ করে (Feuerbach's theorem)

---

### 4. Simson Line (Wallace Line)

যদি P একটি point হয় triangle ABC এর circumcircle এর উপর, এবং D, E, F হয় P থেকে বাহু BC, CA, AB তে perpendiculars এর feet, তাহলে **D, E, F collinear**।

এই line কে **Simson line** বলে।

**বৈশিষ্ট্য:**
- দুটি point P এবং Q এর Simson lines perpendicular হয় যদি ∠POQ = 90° (O = circumcenter)
- Simson line orthocenter এর সাথে বিশেষ relation রাখে

---

### 5. Euler Line

**Theorem:** একটি triangle (equilateral বাদে) এর Circumcenter (O), Centroid (G), Orthocenter (H), এবং Nine-point center (N) একই line এ থাকে।

**Relations:**
- **OG:GH = 1:2**
- **ON:NH = 1:2**
- **ON = R/2** যেখানে R = circumradius

**Equation:** \vec{OH} = \vec{OA} + \vec{OB} + \vec{OC}

---

### 6. Angle Bisector Theorem

Triangle ABC তে যদি angle A এর bisector বাহু BC কে point D তে কাটে, তাহলে:

**BD/DC = AB/AC = c/b**

```
    A
   /|\
  / | \
 /  |  \
/   |   \
B___D___C
```

**External angle bisector theorem:**

External angle bisector বাহু BC extended কে E তে কাটলে:

**BE/EC = AB/AC** (কিন্তু E external point)

---

### 7. Apollonius's Theorem

Triangle ABC তে যদি median AM থাকে (M হলো BC এর midpoint), তাহলে:

**AB² + AC² = 2(AM² + BM²)**

অথবা: **b² + c² = 2(m² + a²/4)**

যেখানে m = median length

---

### 8. British Flag Theorem

একটি rectangle ABCD তে যদি P কোনো point হয় rectangle এর ভিতরে বা উপরে, তাহলে:

**PA² + PC² = PB² + PD²**

```
A_______B
|       |
|   P   |
|       |
D_______C
```

---

## Coordinate Geometry

### Distance Formula:

দুটি point A(x₁, y₁) এবং B(x₂, y₂) এর মধ্যে:

**d = √[(x₂ - x₁)² + (y₂ - y₁)²]**

---

### Section Formula:

যদি point P, line segment AB কে m:n ratio তে divide করে:

**Internal division:**
**P = ((mx₂ + nx₁)/(m+n), (my₂ + ny₁)/(m+n))**

**External division:**
**P = ((mx₂ - nx₁)/(m-n), (my₂ - ny₁)/(m-n))**

**Midpoint (m = n = 1):**
**M = ((x₁ + x₂)/2, (y₁ + y₂)/2)**

---

### Slope:

Line যা points (x₁, y₁) এবং (x₂, y₂) দিয়ে যায়:

**m = (y₂ - y₁)/(x₂ - x₁)**

**Parallel lines:** m₁ = m₂

**Perpendicular lines:** m₁ × m₂ = -1

---

### Straight Line Equations:

**1. Slope-intercept form:**
**y = mx + c**

**2. Point-slope form:**
**y - y₁ = m(x - x₁)**

**3. Two-point form:**
**(y - y₁)/(y₂ - y₁) = (x - x₁)/(x₂ - x₁)**

**4. Intercept form:**
**x/a + y/b = 1**

**5. General form:**
**Ax + By + C = 0**

---

### Distance from Point to Line:

Point (x₀, y₀) থেকে line Ax + By + C = 0 এর দূরত্ব:

**d = |Ax₀ + By₀ + C|/√(A² + B²)**

---

### Triangle Area (Coordinate):

Vertices A(x₁, y₁), B(x₂, y₂), C(x₃, y₃) হলে:

**Area = (1/2)|x₁(y₂ - y₃) + x₂(y₃ - y₁) + x₃(y₁ - y₂)|**

---

### Circle Equations:

**Standard form (center at origin):**
**x² + y² = r²**

**Center-radius form:**
**(x - h)² + (y - k)² = r²**

Center = (h, k), Radius = r

**General form:**
**x² + y² + 2gx + 2fy + c = 0**

Center = (-g, -f)
Radius = √(g² + f² - c)

---

### Conic Sections:

**Circle:** x² + y² = r²

**Parabola:** y² = 4ax (standard)

**Ellipse:** x²/a² + y²/b² = 1

**Hyperbola:** x²/a² - y²/b² = 1

---

## Complex Number Geometry

### Complex Number as Point:

একটি complex number z = x + iy কে plane এ point (x, y) হিসেবে represent করা যায়।

**Modulus:** |z| = √(x² + y²) = distance from origin

**Argument:** arg(z) = θ = tan⁻¹(y/x)

**Polar form:** z = r(cos θ + i sin θ) = re^(iθ)

---

### Geometric Operations:

**Addition:** z₁ + z₂ = parallelogram law

**Subtraction:** z₁ - z₂ = vector from z₂ to z₁

**Multiplication by i:** 90° rotation counterclockwise

**Conjugate:** z̄ = x - iy = reflection about real axis

---

### Distance:

Distance between z₁ and z₂:

**d = |z₁ - z₂|**

---

### Rotation:

Point z কে origin সম্পর্কে θ angle rotate করলে:

**z' = ze^(iθ) = z(cos θ + i sin θ)**

---

### Triangle Centers (Complex):

যদি triangle এর vertices হয় z₁, z₂, z₃:

**Centroid:** G = (z₁ + z₂ + z₃)/3

**Circumcenter:** O সমাধান করে |O - z₁| = |O - z₂| = |O - z₃|

**Orthocenter:** H = z₁ + z₂ + z₃ (যদি circumcenter origin এ হয়)

---

### Useful Identities:

**z₁z̄₁ = |z₁|²**

**|z₁z₂| = |z₁||z₂|**

**arg(z₁z₂) = arg(z₁) + arg(z₂)**

**Triangle inequality:** |z₁ + z₂| ≤ |z₁| + |z₂|

---

### Geometric Theorems using Complex:

**Collinearity:** z₁, z₂, z₃ collinear যদি:

**(z₃ - z₁)/(z₂ - z₁)** real হয়

**Concyclic:** z₁, z₂, z₃, z₄ concyclic যদি:

**[(z₁ - z₃)/(z₁ - z₄)]/[(z₂ - z₃)/(z₂ - z₄)]** real হয়

---

## Barycentric Coordinates

### সংজ্ঞা:

Triangle ABC তে একটি point P কে represent করা হয় তিনটি coordinate (α, β, γ) দিয়ে যেখানে:

**P = (αA + βB + γC)/(α + β + γ)**

সাধারণত normalize করা হয়: α + β + γ = 1

---

### Special Points:

**Centroid:** G = (1, 1, 1) বা (1/3, 1/3, 1/3)

**Incenter:** I = (a, b, c) যেখানে a, b, c = বাহুর দৈর্ঘ্য

**Circumcenter:** O = (sin 2A, sin 2B, sin 2C)

**Orthocenter:** H = (tan A, tan B, tan C)

---

### Distance Formula:

**PA² = -βγa² - γαb² - αβc²** (normalized coordinates এ)

---

### Line Equation:

একটি line এর equation: **αu + βv + γw = 0**

যেখানে (u, v, w) line এ থাকা point।

---

### Applications:

Barycentric coordinates অনেক geometry problems সহজ করে দেয়, বিশেষ করে:
- Cevian সংক্রান্ত problems
- Triangle centers খুঁজে বের করা
- Ratio problems

---

## Inversion Geometry

### সংজ্ঞা:

একটি circle (center O, radius r) সম্পর্কে point P এর inversion হলো point P' যেন:

**OP × OP' = r²**

এবং O, P, P' collinear।

---

### বৈশিষ্ট্য:

**1. Circle এর ভিতরের points বাইরে যায়, বাইরের ভিতরে আসে**

**2. Circle এর উপরের points unchanged থাকে**

**3. Lines through center → lines through center**

**4. Lines not through center → circles through center**

**5. Circles through center → lines not through center**

**6. Circles not through center → circles not through center**

**7. Angles preserved হয় (orientation reverse হতে পারে)**

---

### Inversion Formula (Coordinate):

Center at origin, radius r:

যদি P = (x, y), তাহলে P' = (x', y') যেখানে:

**x' = r²x/(x² + y²)**

**y' = r²y/(x² + y²)**

---

### Applications:

**Inversion ব্যবহার করে সমাধান করা যায়:**
- Circle tangency problems
- Apollonius problems
- Ptolemy's theorem proof
- Various olympiad geometry problems

**Technique:** একটি complicated configuration কে invert করে সহজ করা।

---

## Projective Geometry

### মৌলিক ধারণা:

Projective geometry তে parallel lines একটি "point at infinity" তে মিলিত হয়।

**Projective plane = Euclidean plane + points at infinity**

---

### Homogeneous Coordinates:

একটি point (x, y) কে represent করা হয় (X, Y, Z) দিয়ে যেখানে:

**x = X/Z, y = Y/Z**

Point at infinity: Z = 0

---

### Duality:

Projective geometry তে **points** এবং **lines** dual concepts:
- দুটি points একটি line নির্ধারণ করে
- দুটি lines একটি point নির্ধারণ করে

---

### Cross-Ratio:

চারটি collinear points A, B, C, D এর cross-ratio:

**(A, B; C, D) = (AC/BC)/(AD/BD)**

**Important property:** Cross-ratio preserved হয় projection এর পরেও।

---

### Desargues's Theorem:

দুটি triangles ABC এবং A'B'C' perspective from point O হলে (অর্থাৎ AA', BB', CC' concurrent), তাহলে corresponding sides এর intersections collinear।

---

### Pascal's Theorem:

একটি conic (circle সহ) এর উপর ছয়টি points A, B, C, D, E, F থাকলে:

**AB ∩ DE, BC ∩ EF, CD ∩ FA collinear**

```
Circle এর উপর hexagon ABCDEF এর opposite sides এর intersections collinear।
```

---

### Brianchon's Theorem:

Pascal's theorem এর dual:

একটি conic এ ছয়টি tangent lines থাকলে, opposite vertices এর সংযোগ concurrent।

---

## অনুশীলন সমস্যা

### Trigonometry:

1. প্রমাণ করো: sin²(A) + sin²(B) + sin²(C) = 2[1 + cos(A)cos(B)cos(C)] একটি triangle ABC তে

2. যদি A + B + C = 180°, প্রমাণ করো: tan(A) + tan(B) + tan(C) = tan(A)tan(B)tan(C)

### Triangle Centers:

3. প্রমাণ করো যে medians concurrent (Ceva's theorem ব্যবহার করে)

4. একটি triangle এর circumradius R = 5 এবং inradius r = 2। Area বের করো।

### Circle Geometry:

5. দুটি circles externally tangent। তাদের common external tangent এর length 12 এবং radii 5 ও 3। Centers এর মধ্যে দূরত্ব বের করো।

6. একটি cyclic quadrilateral এর sides 3, 4, 5, 6। Area বের করো।

### Theorems:

7. Stewart's theorem ব্যবহার করে প্রমাণ করো যে একটি triangle এর median এর length:
   mₐ = (1/2)√(2b² + 2c² - a²)

8. Ptolemy's theorem ব্যবহার করে একটি regular hexagon এর diagonal এর length বের করো।

### Coordinate Geometry:

9. Points A(1, 2), B(3, 5), C(7, 4) একটি triangle তৈরি করে। Centroid এবং circumcenter বের করো।

10. Line 3x + 4y = 12 এবং point (2, 3) এর মধ্যে দূরত্ব বের করো।

---

## সমস্যা সমাধানের কৌশল

### 1. Diagram আঁকো:

সবসময় একটি accurate diagram আঁকো। এটি problem বুঝতে এবং pattern খুঁজে পেতে সাহায্য করে।

### 2. Special Cases দেখো:

Equilateral triangle, right triangle, বা অন্য special cases এ কী হয় তা দেখো।

### 3. Auxiliary Lines যোগ করো:

প্রয়োজনে extra lines, circles বা points add করো যা problem সহজ করে দেয়।

### 4. Angle Chasing:

Unknown angles খুঁজে বের করো geometry theorems ব্যবহার করে।

### 5. সঠিক Theorem প্রয়োগ করো:

- Circle problems → Circle theorems
- Triangle centers → Ceva, Menelaus
- Distance/area → Coordinate geometry বা trigonometry

### 6. সমতুল্য Conditions খোঁজো:

যেমন: Cyclic quadrilateral ⟺ opposite angles sum = 180°

### 7. Inversion বা Projection ব্যবহার করো:

Complex problems কে transform করে সহজ করো।

### 8. Symmetry কাজে লাগাও:

Symmetric configurations অনেক সময় সহজ সমাধান দেয়।

---

## গুরুত্বপূর্ণ সূত্র সারসংক্ষেপ

### Triangle:

- **Area = (1/2)bh = √[s(s-a)(s-b)(s-c)] = (1/2)ab sin C = abc/(4R) = rs**
- **Sine rule:** a/sin A = b/sin B = c/sin C = 2R
- **Cosine rule:** a² = b² + c² - 2bc cos A

### Circle:

- **Power of point:** PA × PB = PC × PD (chords)
- **Tangent:** PT² = PA × PB
- **Inscribed angle = (1/2) × Central angle**

### Centers:

- **Circumradius:** R = abc/(4×Area)
- **Inradius:** r = Area/s
- **Euler line:** OG:GH = 1:2

### Theorems:

- **Ceva:** (AF/FB)(BD/DC)(CE/EA) = 1
- **Menelaus:** (AF/FB)(BD/DC)(CE/EA) = -1
- **Ptolemy:** AC × BD = AB × CD + AD × BC
- **Stewart:** b²m + c²n = a(d² + mn)

---

## শেষ কথা

Geometry BDMO এর সবচেয়ে challenging এবং beautiful অংশ। সফল হতে:

1. **Theorems এর proofs বুঝো** - শুধু মুখস্থ নয়
2. **প্রচুর diagrams আঁকো** - visualization develop করো
3. **বিভিন্ন approaches চেষ্টা করো** - synthetic, coordinate, complex, barycentric
4. **Classic problems solve করো** - IMO, USAMO, BDMO previous years
5. **Pattern recognition develop করো** - কোন configuration এ কোন theorem কাজ করে
6. **Auxiliary constructions practice করো** - এটি geometry এর key skill

**Remember:** Geometry তে instant solution নাও থাকতে পারে। Patience এবং persistence খুবই জরুরি!

**তোমার BDMO geometry journey এ শুভকামনা! 📐✨**

---

**তৈরি করেছে:** Claude AI  
**উদ্দেশ্য:** Bangladesh Mathematical Olympiad (BDMO) প্রস্তুতি  
**বিষয়:** Geometry (Complete Comprehensive Guide)  
**তারিখ:** ফেব্রুয়ারি ২০২৬
