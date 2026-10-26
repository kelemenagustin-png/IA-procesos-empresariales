# Prompt 02 — Desarrollo de una aplicación de stock con Vibe Coding

## 1. Objetivo

Explorar el uso de Inteligencia Artificial para desarrollar una aplicación web de gestión de stock y ventas sin escribir manualmente todo el código.

El proyecto busca transformar una necesidad administrativa de un pequeño emprendimiento en un prototipo funcional mediante la herramienta v0 de Vercel.

## 2. Problema identificado

Un emprendimiento de lentes realiza ventas mediante redes sociales y stands en eventos, pero no cuenta con un sistema organizado para registrar sus productos, controlar inventario y analizar sus ventas.

Se plantea desarrollar una aplicación que permita:

- Registrar productos y cantidades disponibles.
- Controlar entradas y salidas de mercadería.
- Registrar ventas por canal.
- Descontar automáticamente productos vendidos.
- Consultar información comercial básica.

## 3. Herramienta utilizada

**Plataforma:** v0 de Vercel.

**Metodología:** Vibe Coding, mediante instrucciones en lenguaje natural.

**Resultado publicado:**

https://gestion-lens-stock.vercel.app/

## 4. Primera versión del prompt

La primera solicitud consistió en desarrollar una aplicación web llamada **Lens Stock**, asignando a la IA el rol de desarrollador full-stack, arquitecto de software y diseñador UI/UX.

Se solicitaron las siguientes características:

- Aplicación privada para un único propietario.
- Desarrollo con Next.js, TypeScript y Tailwind CSS.
- Base de datos PostgreSQL mediante Supabase.
- Inicio de sesión y autenticación.
- Protección de información mediante políticas de seguridad.
- Gestión de productos, inventario y ventas.
- Descuento automático del stock.
- Reportes comerciales y estadísticas.
- Diseño responsive para celulares y computadoras.

También se definieron reglas para evitar ventas sin stock, registrar movimientos de inventario y conservar el historial de operaciones.

**Problema detectado durante el desarrollo:**

La herramienta solicitó autorización para ejecutar una migración de Supabase que incluía modificaciones de la base de datos y del sistema de autenticación.

Como se trataba de una primera experiencia de Vibe Coding, decidí revisar el alcance técnico y simplificar el proyecto antes de autorizar modificaciones que todavía no comprendía completamente.

## 5. Segunda versión del prompt — Simplificación del MVP

Quiero simplificar la aplicación que estamos desarrollando para el emprendimiento de lentes.

Es una aplicación privada, pensada para que una sola persona administre su negocio.

**Funcionalidades necesarias:**

1. Registrar productos con modelo, color, costo de compra, precio de venta y cantidad disponible.
2. Registrar ventas, indicando producto, cantidad, precio y canal de venta.
3. Descontar automáticamente las unidades vendidas del inventario.
4. Registrar entradas de mercadería, reposiciones y ajustes de stock.
5. Consultar un historial de ventas y movimientos.
6. Mostrar un resumen de ingresos, costos de mercadería vendida y ganancia bruta estimada.

**Prioridad actual:**

Estoy aprendiendo Vibe Coding y quiero probar primero una versión funcional sencilla.

Por ahora, utilizá almacenamiento local del navegador para guardar los datos, sin Supabase, sin registro de usuarios y sin servicios externos.

Agregá una función para exportar e importar copias de seguridad de los datos en formato JSON, validando el archivo antes de importarlo.

Aclará en la interfaz que esta versión guarda los datos únicamente en el navegador actual y que no es adecuada para almacenar información crítica sin respaldos.

Conservá el diseño visual existente.

No elimines código ni datos existentes sin mostrarme primero qué modificarías.

Más adelante quiero evaluar una migración a Supabase, con acceso privado mediante una única cuenta administradora y medidas de seguridad adecuadas.

Priorizá una versión mínima, clara y funcional.

## 6. Resultado obtenido

Se publicó un prototipo web orientado a gestionar productos, ventas e inventario de un emprendimiento de lentes.

**Enlace:** https://gestion-lens-stock.vercel.app/

La aplicación constituye un primer resultado del proceso de desarrollo asistido por IA.

La publicación de la página no demuestra por sí sola que todas las funcionalidades hayan sido verificadas.

## 7. Validación del proyecto

**Estado:** Pendiente de pruebas funcionales documentadas.

Pruebas previstas:

1. Registrar un producto con 10 unidades.
2. Registrar una venta de 2 unidades.
3. Verificar que el stock disminuya a 8.
4. Registrar una reposición de 5 unidades y comprobar que el stock aumente a 13.
5. Cerrar y volver a abrir la página para comprobar la persistencia local.
6. Exportar los datos y verificar que puedan importarse correctamente.
7. Comprobar que la aplicación rechace ventas superiores al stock disponible.

Los resultados se documentarán después de ejecutar las pruebas.

## 8. Conclusiones y aprendizajes

Este ejercicio permitió experimentar cómo una necesidad empresarial puede convertirse en un prototipo mediante instrucciones en lenguaje natural.

El principal aprendizaje fue comprender la importancia de definir correctamente el alcance de un proyecto.

La primera versión incorporaba demasiados componentes técnicos para una práctica inicial. La segunda priorizó las funciones esenciales y redujo la complejidad.

También permitió identificar la diferencia entre una aplicación publicada, una aplicación funcional y una aplicación preparada para almacenar información empresarial real.

**Aprendizaje principal:** un prompt técnicamente detallado no necesariamente produce un mejor resultado cuando la complejidad supera las necesidades de la primera versión.

**Estado:** prototipo publicado, pendiente de validación funcional completa.
