# SICAT-Prototipo-TRL5
Prototipo web funcional (TRL5) para la gestión y programación administrativa de citas en consultorios odontológicos pequeños (SICAT), desarrollado en el curso Proyecto de grado (202016907) de la UNAD con datos simulados.
# SICAT – Sistema Web para la Gestión de Citas en Consultorios Odontológicos Pequeños (TRL5)

Proyecto académico de Ingeniería de Sistemas – **UNAD** (Curso: *Proyecto de grado – 202016907*, Fase 4 – Componente práctico – Práctica simulada)[cite: 1, 2, 7].

## Objetivo y alcance del prototipo (TRL5)
Desarrollar y validar en un entorno simulado relevante un prototipo web funcional (nivel de maduración tecnológica **TRL5**) que centralice la programación y administración de citas en consultorios odontológicos pequeños, permitiendo a usuarios autorizados administrar profesionales, horarios, disponibilidad y citas mediante controles de integridad y seguridad[cite: 3, 8, 9, 11].

- **Enfoque y metodología:** Proyecto aplicado con alcance descriptivo para caracterizar el proceso y marco ágil basado en **Scrum** adaptado a ejecución individual en ciclos incrementales[cite: 8, 9, 19].
- **Arquitectura y tecnología:** Diseño en capas con **ASP.NET Core**, **Entity Framework Core**, base de datos relacional (**SQL Server**) y componentes web (**HTML5, CSS3, JavaScript y Bootstrap**)[cite: 15, 22].
- **Control y privacidad:** Autenticación, control de acceso basado en roles (`Administrador`, `Recepción`, `Odontólogo`), validación de entradas, prevención de cruces de horario y uso de datos 100 % ficticios en entorno simulado[cite: 8, 9, 14, 15, 20, 23, 24].
- **Exclusiones expresas:** No contempla historias clínicas electrónicas, diagnósticos, prescripciones, facturación, integración con EPS, pagos en línea ni mensajería automática externa[cite: 8, 9, 12].

## Estructura del repositorio
- `README.md`: Documentación general del repositorio y del prototipo SICAT[cite: 34].
- `database/SICAT_Schema_Seed.sql`: Script de base de datos en SQL Server con tablas, restricciones, datos ficticios y validación contra conflictos de horario[cite: 23, 24, 36].
- `src/Controllers/CitasController.cs`: Controlador para consulta de agenda, validación de campos obligatorios y registro de citas sin traslapes[cite: 22, 24, 38].
- `src/Services/DisponibilidadService.cs`: Servicio de verificación de solapamiento y disponibilidad horaria[cite: 21, 24, 37].
- `src/Views/Citas/Index.cshtml`: Vista web para visualización de agenda y registro de citas en entorno simulado[cite: 22].
- `docs/Arquitectura_y_Pruebas_TRL5.md`: Síntesis de arquitectura y estado de los casos de prueba (`P01–P10`)[cite: 24, 25, 35].

## Autora y curso
- **Estudiante:** Paula Andrea Torres Salazar[cite: 7]
- **Tutor:** Daniel Andrés Guzmán[cite: 7]
- **Programa:** Ingeniería de Sistemas – UNAD[cite: 7]
- **Centro:** San Vicente del Caguán – Caquetá[cite: 7]
