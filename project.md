**Warehouse & Logistics Management System (Industria de Logística y Cadena de Suministro):** Desarrollar un sistema integral de gestión de almacenes e inventario basado en una aplicación CLI utilizando Python y PostgreSQL. El sistema deberá permitir la administración de productos, proveedores, órdenes de compra, movimientos de inventario y múltiples almacenes, simulando las operaciones principales de una plataforma logística empresarial.

El proyecto deberá implementar una arquitectura limpia y escalable con separación por capas, aplicando buenas prácticas de desarrollo como tipado estático estricto mediante mypy, validación de datos, migraciones de base de datos con Alembic y pruebas unitarias utilizando pytest. Además, deberá integrar herramientas de calidad y mantenimiento de código como ruff y black.

A nivel de base de datos, se deberán desarrollar consultas SQL complejas orientadas al análisis y optimización del rendimiento mediante el uso de EXPLAIN ANALYZE, índices compuestos, optimización de consultas y vistas materializadas. También se incluirán scripts de automatización mediante Bash, gestión del proyecto con Poetry y un entorno completamente dockerizado utilizando Docker Compose para facilitar su ejecución y despliegue.

**SCHEMA:**

products
id
name
price
categories
sku


suppliers
id
company_name
email
phone
contact_name


warehouses_products
name
location


warehouses_suppliers
name
location


Del almacen de suplidores se puedan pasar productos hacia el almacen de productos. Depende lo que quieras puedes buscar por almacen o por el nombre del producto.

