# Taller Final - Fundamentos Algorítmicos

---

## SECCIÓN A: Fundamentos Lógicos

### 1. Evaluación de Motor Aritmética

**Expresión:**
resultado <- 5 + 3 * 2 ^ 2 - (10 MOD 3)

**Paso a paso:**
1. Potencia: 2 ^ 2 = 4
2. Multiplicación: 3 * 4 = 12
3. Módulo: 10 MOD 3 = 1
4. Operaciones finales:
   5 + 12 - 1 = 16

**Resultado final:**
16


---

### 2. Álgebra Booleana Operacional

Datos:
var_A = Verdadero
var_B = Falso
var_C = Verdadero


Expresión:
No(var_A O var_B) Y (var_C Y No(var_B))


Paso a paso:
1. var_A O var_B = Verdadero
2. No(Verdadero) = Falso
3. No(var_B) = Verdadero
4. var_C Y Verdadero = Verdadero
5. Falso Y Verdadero = Falso

**Resultado final:**
Falso
