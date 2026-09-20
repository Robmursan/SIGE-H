
## 🌿 Estrategia de Ramas y Control de Versiones

Este repositorio implementa **GitHub Flow** como modelo de integración continua hacia la rama protegida `main`.

### Nomenclatura de Ramas
Toda rama debe originarse desde `main` actualizado, utilizando minúsculas y formato *kebab-case*:
- `feature/nombre-tarea`: Desarrollo de nuevos módulos o componentes.
- `bugfix/nombre-error`: Corrección de fallos en desarrollo o pruebas.
- `hotfix/nombre-fallo`: Parches urgentes para fallos en producción.
- `refactor/nombre-mejora`: Optimización o reestructuración de código sin alterar comportamiento.

### Políticas de Pull Request (PR) y Code Review
1. **Bloqueo de Push Directo:** Ningún desarrollador puede enviar commits directamente a `main`.
2. **Revisión Obligatoria:** Todo PR requiere la aprobación formal (*Approve*) de al menos 1 revisor antes de fusionar.
3. **Cumplimiento de Lista de Cotejo:** El autor debe verificar ausencia de credenciales `.env` y pruebas locales satisfactorias.
4. **Estrategia de Combinación:** Se utiliza exclusivamente **Squash and Merge** para mantener un historial lineal y atómico, eliminando la rama al completar la fusión.
