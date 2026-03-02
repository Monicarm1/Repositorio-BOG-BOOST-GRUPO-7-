# Guía de Contribución a BOG-BOOST

¡Gracias por tu interés en contribuir! Este documento describe el proceso y las convenciones que seguimos para mantener un flujo de trabajo ordenado y colaborativo.

---

## Índice

- [Guía de Contribución a BOG-BOOST](#guía-de-contribución-a-sena-attendance)
  - [Índice](#índice)
  - [Convenciones de Commits](#convenciones-de-commits)
    - [Ejemplo](#ejemplo)
  - [Versionamiento Semántico](#versionamiento-semántico)
  - [Cierre de Issues y Co-Autores](#cierre-de-issues-y-co-autores)
  - [Recursos adicionales](#recursos-adicionales)

---

## Convenciones de Commits

Utilizamos una convención basada en [Conventional Commits](https://www.conventionalcommits.org/es/v1.0.0/), adaptada para BOG-BOOST.  
La estructura del mensaje es:

```text
<type>(<scope>): <resumen breve>

<cuerpo del mensaje>

<footer>
```

- **`type`** : Tipo de cambio. Usa minúsculas.
    - **feat**: Nueva funcionalidad para el usuario.
    - **fix**: Corrección de errores para el usuario.
    - **docs**: Cambios en la documentación.
    - **style**: Formateo, sin cambios en la lógica.
    - **refactor**: Refactorización, sin añadir funcionalidad.
    - **test**: Añadir o actualizar pruebas.
    - **chore**: Tareas de mantenimiento.
    - **merge**: Fusión de ramas.
    - **release**: Creación de una nueva versión.

- **`scope`** : Módulo o área afectada (opcional si el cambio es global).

- **`resumen breve`** : Primera línea del mensaje, clara y concisa (máximo 70 caracteres), que explica de forma rápida y entendible qué se hizo. Es obligatorio y debe ser en tiempo presente, en minúsculas y sin punto final.

- **`cuerpo del mensaje`** : Descripción más detallada del cambio, explicando el motivo y contexto si es relevante. Debe ayudar a entender el "por qué" del cambio, pero evita detalles innecesarios o técnicos muy profundos. Deja una línea en blanco entre el resumen y el cuerpo. Cada línea debe tener máximo 80 caracteres.

- **`footer`** : Información adicional, como cierre de issues (Closes #número), co-autores (co-authored-by: Nombre <correo>), Notas de breaking change (BREAKING CHANGE: Ahora se requiere Node 20+), referencias a tareas relacionadas o cualquier tipo de metadato relevante sobre el commit.

### Ejemplo

```text
feat(auth): agregar autenticación OAuth2

Se agrega soporte para autenticación usando el protocolo OAuth2,
permitiendo la integración con proveedores externos.

Closes #3030
co-authored-by: Jose Andres <correo@hola.co>
```

---

## Versionamiento Semántico

El proyecto sigue [SemVer 2.0.0](https://semver.org/lang/es/):

- **X**: `major` - Cambios incompatibles a nivel de API o funcionalidades principales.
- **Y**: `minor` - Nuevas funcionalidades compatibles con versiones anteriores.
- **Z**: `patch` - Correcciones de errores y mejoras menores.

**Recomendación:**  
Etiqueta las versiones siguiendo el formato estándar:  
`vX.Y.Z`  
Por ejemplo:  
`v1.2.3`

---

## Cierre de Issues y Co-Autores

- Para cerrar issues, usa `Closes #número` en el footer.
- Para co-autores, agrega `co-authored-by: Nombre <correo>` en el footer.

---

## Recursos adicionales

- [Conventional Commits](https://www.conventionalcommits.org/es/v1.0.0/)
- [Semantic Versioning](https://semver.org/lang/es/)
- [Guía de Git Commit Messages](https://chris.beams.io/posts/git-commit/)