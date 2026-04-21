cat <<EOF > POSTMORTEM.md
# 📊 Informe Final: Laboratorio de Colaboración
**Proyecto:** Calculadora de Equipo (\`math_operations.py\`)

---

## 1. Resumen del Flujo de Trabajo
El equipo trabajó bajo un modelo de ramificación (**branching**) paralelo, utilizando **Pull Requests (PRs)** para garantizar la calidad del código antes de su integración en la rama \`main\`.

## 2. Participantes y Roles
* **Coder A (Juan):** Gestión del repositorio, gobernanza y desarrollo de la función \`suma\`.
* **Coder B (Joel):** Desarrollo de la función \`resta\` y creación intencionada de conflicto.
* **Coder C (Luis):** Documentación técnica (\`README.md\`) y revisión de código.

## 3. Trazabilidad de las Pull Requests
| PR # | Descripción | Estado |
| :--- | :--- | :--- |
| **1** | Implementación de función Suma | ✅ Aprobada por Joel |
| **2** | Documentación README | ✅ Aprobada tras corrección |
| **3** | Implementación de función Resta | ✅ Aprobada por Luis |

## 4. Gestión del Conflicto
Se detectó un conflicto en el archivo \`math_operations.py\` debido a ediciones concurrentes en la cabecera del script.

**Resolución:**
1. Se eliminaron las marcas de conflicto (\`<<<<\`, \`====\`, \`>>>>\`).
2. Se unificó el código manteniendo ambas funciones.
3. Resultado final verificado localmente con éxito.

## 5. Código Final Integrado
\`\`\`python
# Calculadora de Equipo

def suma(a, b):
    return a + b

def subtract(a, b):
    return a - b

if __name__ == "__main__":
    print(f"Resultado suma: {suma(5, 7)}")
    print(f"Resultado resta: {subtract(10, 4)}")
\`\`\`

## 6. Estado Final del Repositorio
* 🧹 **Ramas locales:** Eliminadas.
* ☁️ **Ramas remotas:** Eliminadas.
* 🔒 **Rama 'main':** Protegida y actualizada.

---
*Informe generado para el registro de competencias técnicas - v1.1*
EOF