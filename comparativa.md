//  Comparativa de Sistemas ERP y CRM - UD2

//  1. Datos Generales
// Propietario: mangeltorves-debug
/Empresa asignada: 16 Maderas Noble
 Palabra del día:compañero

// 2. Licencias y Modelosss
// Diferenciación de Modelos
Software Libre: Garantiza las cuatro libertades esenciales: ejecutar, estudiar, modificar y redistribuir el software. Pone el foco en la ética y el control del usuario sobre sus herramientas tecnológicas.
Código Abierto: Se centra en los beneficios prácticos y metodológicos del modelo de desarrollo colaborativo. Todo software libre suele ser de código abierto, pero no a la inversa bajo criterios estrictamente filosóficos.
Software Propietario:El código fuente está restringido, pertenece a una entidad concreta y su uso, modificación o redistribución están limitados por contratos restrictivos de licencia.

// ¿Por qué "Libre" no significa "Gratuito"?
// El término "libre" hace referencia a la libertad, no al precio .En el ámbito empresarial, implantar un ERP o CRM libre conlleva costes económicos directos e indirectos:
// Auditoría, consultoría de implantación y adaptación a los procesos de negocio.
// Despliegue en servidores propios o en la nube, costes de infraestructura y mantenimiento.
// Soporte técnico especializado y actualizaciones evolutivas.

// Edición Community frente a Enterprise
Community: Versión gratuita y de código abierto orientada a pymes o comunidades de desarrollo. Suele carecer de soporte técnico oficial directo por parte del fabricante, herramientas avanzadas de seguridad corporativa, y determinados módulos especializados.
Enterprise: Versión comercial de pago por suscripción anual por usuario. Incluye soporte oficial con SLA , actualizaciones estables y garantizadas, parches de seguridad críticos, y herramientas propietarias de gestión o rendimiento.

// 3. Fichas Técnicas

// 3.1 ERP Libre: Odoo Community
Licencia LGPLv3 / OPL-1
Versión vigente: Odoo 18 Community
Lenguaje del servidor: Python
SGBD compatibles:PostgreSQL
Modalidad: Local (On-Premises) / Nube (Odoo.sh / PaaS)
Módulos principales: Inventario, Fabricación (MRP), Compras, Ventas, Facturación.
Requisitos: Python 3.10+, PostgreSQL 15+, mínimo 2 CPU y 4 GB de RAM.
Fuente y fecha: (https://www.odoo.com/) (Consultado: septiembre de 2026).

3.2 ERP Propietario: Microsoft Dynamics 365 (Business Central)
Licencia: Propietario (SaaS comercial)
Versión vigente: Dynamics 365 Business Central (Wave 2)
Lenguaje del servidor: AL (Plataforma Azure)
SGBD compatibles: Azure SQL Database (Gestionado)
Modalidad: Nube (SaaS nativo) / Híbrido
Módulos principales: Gestión Financiera, Cadena de Suministro, Fabricación, Ventas.
Requisitos: Navegador web moderno actualizado; integración nativa con Microsoft 365.
Fuente y fecha: ](https://dynamics.microsoft.com/) ( septiembre de 2026).

 3.3 CRM Libre: SuiteCRM
Licencia: GNU AGPL v3
Versión vigente: SuiteCRM 8.x
Lenguaje del servidor: PHP (8.1 / 8.2)
SGBD compatibles: MySQL, MariaDB, PostgreSQL
Modalidad: Local (On-Premises) / Nube privada
Módulos principales: Gestión de Cuentas, Contactos, Oportunidades de Venta, Campañas.
Requisitos: Servidor web (Apache/Nginx), PHP 8.1+, MariaDB 10.5+ / MySQL 8.0+.
Fuente y fecha: (https://suitecrm.com/) (septiembre de 2026).

3.4 CRM Propietario: Salesforce (Sales Cloud)
Licencia: Propietario (SaaS de suscripción)
Versión vigente: Salesforce Lightning Enterprise
Lenguaje del servidor: Apex (Java-like) / Lightning Web Components (JS)SGBD compatibles: Base de datos multi-tenant propietaria en la nube de Salesforce
Modalidad: Nube (SaaS puro)
Módulos principales: Gestión de Leads y Oportunidades, Automatización de Ventas, Einstein AI.
Requisitos: Conexión a Internet de banda ancha y navegadores compatibles.
Fuente y fecha: (https://www.salesforce.com/) ( septiembre de 2026).

// 4. Fe de Erratas del Tema 2

-- 1. Dato sobre versiones de Odoo en el material:**
   Qué dice el tema: Afirma que Odoo Community carece por completo de soporte para trazabilidad de lotes y fabricación avanzada.
   Qué es correcto hoy: Odoo Community incluye de serie módulos funcionales de gestión de inventario, rutas de almacén y órdenes de fabricación básicas, limitando solo algunas automatizaciones corporativas complejas y contabilidad analítica avanzada de la versión Enterprise.
   Fuente: Documentación oficial de Odoo Apps & Features.

-- 2. Requisitos de despliegue de sistemas ERP en la nube:**
    Qué dice el tema: Sugiere que los ERP propietarios actuales operan exclusivamente mediante instalación local pesada con clientes de escritorio instalados en cada equipo.
    Qué es correcto hoy:** La gran mayoría de plataformas corporativas actuales funcionan nativamente en la nube en formato SaaS mediante acceso web puro.
    Fuente: Informes de arquitectura cloud de Gartner y documentación de Microsoft Cloud.


// 5. Matriz de Decisión y Recomendación

 Justificación de Criterios 
Se han evaluado tres soluciones candidatas adaptadas a Maderas Noble :
// 1. Opción A: Odoo Community .
// 2. Opción B: Microsoft Dynamics 365 Business Central .
// 3. Opción C:   Odoo Enterprise .

 Coste Total de Propiedad : Odoo Community destaca por la ausencia de licencias por usuario.
Módulos de Fabricación y Almacén: Odoo ofrece una gestión excelente de trazabilidad de lotes y materias primas.
Facilidad de Integración: Dynamics 365 destaca si ya se utiliza el ecosistema de herramientas Microsoft 365.

 Recomendación Final y Análisis de Riesgos
Para Maderas Noble, la opción recomendada es Odoo Community por el equilibrio entre costes de inversión inicial, adaptabilidad del código fuente a procesos específicos de carpintería y control absoluto de los datos de inventario.

Riesgos asociados:
Coste total : Dependencia de horas de consultoría externa para actualizaciones o incidencias complejas.
Dependencia del proveedor: Si se delegan los desarrollos a medida en un único partner externo, cambiar de proveedor puede resultar complejo.
Soporte técnico: Al ser Community, no se dispone de SLA directo del fabricante, dependiendo de la capacidad del partner o equipo propio.
Migración futura: La transición de esquemas personalizados de Community a Enterprise requiere una planificación rigurosa para evitar pérdidas de histórico.