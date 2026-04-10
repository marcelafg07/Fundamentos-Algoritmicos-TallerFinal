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



---

### 3. Depuracion de software ( Debugging código corregido)

Algoritmo SelectorCandidatos
    Definir estatura_ingresada Como Real
    Definir peso_ingresado Como Real

    Leer estatura_ingresada
    Leer peso_ingresado

    Si estatura_ingresada > 1.70 Y peso_ingresado < 80 Entonces
        Escribir "Validación del perfil: Correcta."
    Sino
        Escribir "Validación del perfil: Fallida."
    FinSi
FinAlgoritmo


## SECCIÓN B: Logica de Rendimiento


Algoritmo Nomina

    Definir nombre_operador Como Cadena
    
    Definir horas Como Entero
    
    Definir tarifa, subtotal, extra, deducciones, neto Como Real

    tarifa <- 35000

    Escribir "Ingrese nombre:"
    Leer nombre_operador

    Escribir "Ingrese horas trabajadas:"
    Leer horas

    Si horas <= 160 Entonces
        subtotal <- horas * tarifa
    Sino
        extra <- (horas - 160) * (tarifa * 1.35)
        subtotal <- (160 * tarifa) + extra
    FinSi

    Si subtotal < 1500000 Entonces
        deducciones <- subtotal * 0.04
    Sino
        Si subtotal < 3000000 Entonces
            deducciones <- subtotal * 0.08
        Sino
            deducciones <- subtotal * 0.13
        FinSi
    FinSi

    neto <- subtotal - deducciones

    Escribir "Empleado: ", nombre_operador
    Escribir "Salario Bruto: ", subtotal
    Escribir "Deducciones: ", deducciones
    Escribir "Salario Neto: ", neto
    
FinAlgoritmo



