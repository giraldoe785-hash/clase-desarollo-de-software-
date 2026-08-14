# MyCode v3 — QA, i18n, dark mode y membresías

Esta versión continúa el proyecto MyCode existente. No reemplaza el modelo de membresías/tokens; lo refuerza con auditoría de entradas, planes con precios, botón Volver, modo oscuro, i18n ES/EN, búsqueda multidioma, accesibilidad básica y responsive.

## Importante sobre seguridad

Esta es una demo frontend. Los datos de usuarios y tokens se guardan en `localStorage` y la sesión en `sessionStorage` para poder probar flujos. Esto **no es una arquitectura de producción**. El control real de planes, tokens, autenticación, pagos y autorización debe vivir en un backend.

No se almacenan datos de tarjetas en esta versión.

## Datos de demostración

Registro:
- Usuario: 3–30 caracteres.
- Correo: válido.
- Contraseña: mínimo 8 caracteres, letras y números.
- Tipo: estudiante o usuario general.

Planes:
- Bronce: $22.00 USD/mes · 50 tokens.
- Plata: $55.00 USD/mes · 120 tokens.
- Oro: $200.00 USD/mes · 350 tokens.

Costes de tokens: 1, 2, 3, 5 y 8.

## Flujos verificados

1. Registro → Login → Dashboard → Cursos.
2. Dashboard → Planes → Cambio de plan.
3. Curso → Consumo de tokens → actualización de saldo.
4. Tokens bajos → advertencia → planes.
5. ES → EN → recarga → persistencia del idioma.
6. Búsqueda `variables` y `loops` usando metadatos ES/EN.
7. Claro → Oscuro → recarga → persistencia.
8. Página secundaria → botón Volver.
9. Entradas de prueba con HTML/script y cadenas tipo SQL se tratan como texto/validación; no se ejecutan.
