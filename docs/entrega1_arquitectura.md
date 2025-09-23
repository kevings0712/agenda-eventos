# Arquitectura y Principios (borrador)

## Arquitectura
- Backend en 3 capas: controladores (Express), servicios (reglas), repositorios (Prisma).
- Frontend SPA (React) consume API REST.
- Servicio de Email planificado para invitaciones/RSVP.
- Índices en BD por ownerId+startAt.

## SOLID (aplicado)
- SRP: separar EventService, InvitationService y EmailService.
- OCP: EmailService con interfaz; cambiar proveedor sin tocar casos de uso.
- DIP: controladores dependen de interfaces (inyectadas) no implementaciones concretas.

## Patrones
- Observer: notificar al organizador ante cambios de RSVP.
- Factory: crear EmailService según entorno (dev/prod).
- Singleton: PrismaClient como cliente único de BD.

## Seguridad y Escalabilidad
- Hash de contraseñas (bcrypt), JWT con expiración, CORS restringido.
- Validación de entrada (Zod), sanitización y rate limiting (a agregar).
- API stateless, paginación, logs y métricas.
