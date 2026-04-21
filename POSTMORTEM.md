import os

# Contenido del informe final del ejercicio
content = """==========================================================
INFORME FINAL: LABORATORIO DE COLABORACIÓN (GIT/GITHUB)
Proyecto: Calculadora de Equipo (math_operations.py)
==========================================================

1. RESUMEN DEL FLUJO DE TRABAJO
----------------------------------------------------------
El equipo trabajó bajo un modelo de ramificación (branching)
paralelo, utilizando Pull Requests (PRs) para garantizar la
calidad del código antes de su integración en la rama 'main'.

2. PARTICIPANTES Y ROLES
----------------------------------------------------------
- Coder A (Juan): Gestión del repositorio, gobernanza y
  desarrollo de la función 'suma'.
- Coder B (Joel): Desarrollo de la función 'resta' y
  creación intencionada de conflicto.
- Coder C (Luis): Documentación técnica (README.md) y
  revisión de código.

3. TRAZABILIDAD DE LAS PULL REQUESTS
----------------------------------------------------------
* PR #1 (Suma): Implementada por Juan. Aprobada por Joel.
* PR #2 (README): Implementada por Luis. Juan solicitó 
  cambios (corrección de nombres). Aprobada tras corrección.
* PR #3 (Resta): Implementada por Joel. Aprobada por Luis.

4. GESTIÓN DEL CONFLICTO
----------------------------------------------------------
Se detectó un conflicto en el archivo 'math_operations.py'
debido a ediciones concurrentes en la cabecera del script.

Resolución:
- Se eliminaron las marcas de conflicto (<<<<, ====, >>>>).
- Se unificó el código manteniendo ambas funciones.
- Resultado final verificado localmente con éxito.

5. CÓDIGO FINAL INTEGRADO (math_operations.py)
----------------------------------------------------------
# Calculadora de Equipo

def suma(a, b):
    return a + b

def subtract(a, b):
    return a - b

if __name__ == "__main__":
    print(f"Resultado suma: {suma(5, 7)}")
    print(f"Resultado resta: {subtract(10, 4)}")

6. ESTADO FINAL DEL REPOSITORIO
----------------------------------------------------------
- Ramas locales: Eliminadas (Limpio).
- Ramas remotas: Eliminadas (Limpio).
- Rama 'main': Protegida y actualizada.

==========================================================
Informe generado automáticamente - Fin del Ejercicio
==========================================================
"""

file_path = '/mnt/data/ejercicio-colaboracion-calculadora.txt'

with open(file_path, 'w', encoding='utf-8') as f:
    f.write(content)

print(f"Archivo guardado en: {file_path}")