# Conventional_commit

# ¿Qué es conventional commit?

**Conventional Commit** (o Commits Convencionales) es una convención de estilo para los mensajes de commit en ```Git``` que sigue un **formato específico**. Esta convención hace que los mensajes de commit sean más claros, estructurados y útiles tanto para los desarrolladores como para las herramientas automáticas. El propósito es establecer una manera consistente de escribir los mensajes de commit, lo que facilita la interpretación del historial de cambios, la generación de versiones y el análisis automatizado.

<br>

## Estructura de un mensaje de commit convencional:

```
<tipo>(<área opcional>): <descripción corta>

[Opcional] Cuerpo del mensaje

[Opcional] Pie del mensaje
```

## Ejemplo:

```
feat(api): agregar endpoint para crear usuarios
fix(auth): corregir error en la validación del token
docs(readme): actualizar instrucciones de instalación
refactor(core): optimizar función de cálculo de totales
chore(deps): actualizar versión de eslint
```
<br>

# ¿Por qué es importante usar Conventional Commits?

1. ###### **Estandariza el historial del proyecto**
    Todos los commits siguen un mismo formato, lo que hace que sea fácil entender qué se cambió y por qué.

2. ###### **Facilita la automatización**
    Herramientas como semantic-release pueden generar versiones automáticamente (v1.2.3 → v1.3.0, etc.) basándose en los tipos de commit (feat, fix, etc.).

3. ###### **Mejor comunicación en equipo**
    Cualquiera puede ver rápidamente qué tipo de cambio se hizo sin leer el código.

4. ###### **Generación automática de changelogs**
    Los commits bien estructurados permiten crear ```CHANGELOG.md``` automáticamente, con secciones de “Features”, “Fixes”, etc.

5. ###### **Integración con CI/CD y control de versiones semántico (SemVer)**
    Puedes **automatizar** el versionado (major, minor, patch) dependiendo del tipo de commit:

 * ```feat```: → incrementa minor

 * ```fix``` : → incrementa patch

 * ```BREAKING CHANGE```: → incrementa major


<br>
<br>

# Tipos más comunes de commits

| Tipo | Descripción |
| ---- | ----------- |
| ```feat``` | Nueva funcionalidad |
| ```fix``` | Corrección de error |
| ```docs```| Cambios en documentación |
| ```style```| Formato, sin cambios en lógica|
| ```refactor``` | Reestructuración sin cambiar comportamiento |
| ```test```| Cambios o agregados de tests |
| ```chore``` | Tareas de mantenimiento o configuración |

<br>



## En resumen

Usar Conventional Commits mejora:

* La claridad del historial git

* La automatización del versionado

* La colaboración en equipo
