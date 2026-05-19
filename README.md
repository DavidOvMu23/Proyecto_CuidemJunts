# CuidemJunts

Plataforma de seguimiento telefónico para personas mayores en riesgo de soledad.  
Permite a equipos de teleoperadores gestionar llamadas, registrar incidencias y mantener un contacto regular y humano con cada persona atendida.

---

## Descripción del proyecto

CuidemJunts conecta a supervisores y teleoperadores con las personas que cuidan. El supervisor organiza los grupos de trabajo y supervisa las llamadas desde un panel web de escritorio; los teleoperadores realizan las llamadas y registran el resultado de cada una. Los familiares y contactos de emergencia de cada persona están centralizados en el sistema para actuar rápido cuando sea necesario.

El proyecto está formado por dos aplicaciones independientes que trabajan juntas:

| Parte | Tecnología | Descripción |
|---|---|---|
| **Frontend** | Flutter (Web / Desktop) | Panel de administración y seguimiento |
| **Backend** | NestJS + PostgreSQL | API REST + base de datos |

---

## Estructura del repositorio

```
Proyecto_CuidemJunts/
├── Frontend_CuidemJunts/   # Aplicación Flutter
└── Backend_CuidemJunts/    # API NestJS + Docker Compose
```

---

## Puesta en marcha rápida

### 1. Backend (Docker)

```bash
cd Backend_CuidemJunts
cp .env.example .env          # Edita las variables de entorno
docker compose up -d
```

El servidor arranca en `http://localhost:3000` por defecto.

### 2. Frontend (Flutter)

```bash
cd Frontend_CuidemJunts
flutter pub get
flutter run -d chrome         # Web
# o:
flutter run -d macos          # macOS
```

Consulta el README de cada subcarpeta para instrucciones detalladas.

---

## Funcionalidades principales

- Registro y gestión de **usuarios/pacientes** (datos personales, nivel de dependencia, medicación)
- Gestión de **trabajadores** (supervisores y teleoperadores) con roles diferenciados
- Organización por **grupos de trabajo** (turnos, equipos)
- **Llamadas** — registro de cada llamada con estado, duración, resumen y observaciones
- **Contactos de emergencia** — vinculados a cada paciente, diferenciando contactos personales y servicios oficiales
- **Notificaciones** internas para alertar a teleoperadores de eventos relevantes
- Panel de estadísticas diarias: llamadas programadas, completadas y pendientes
- Calendario mensual con vista de todas las llamadas
- Soporte multiidioma: **español, catalán e inglés**
- Tema claro y oscuro

---

## Estado del proyecto

En desarrollo activo. No disponible para instalación pública.

---

## Contacto

Si formas parte del equipo o quieres colaborar, contacta con los responsables del proyecto para recibir acceso.
