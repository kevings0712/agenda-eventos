# Agenda de Eventos con Invitaciones

Aplicación para crear eventos, enviar invitaciones y gestionar RSVP.

## Entrega 1 (diseño y base del repo)
- Historias de usuario, casos de uso, arquitectura, SOLID y patrones.
- Estructura real del proyecto (front/back), archivos base y este README.

## Stack propuesto
- Frontend: React + Vite + TypeScript.
- Backend: Node.js + Express + TypeScript + PostgreSQL.


## Cómo ejecutar (se irá ampliando)
- Backend: `src/backend/` (API).
- Frontend: `src/frontend/` (SPA).

## ️ Requisitos
Antes de iniciar, asegúrate de tener instalado:
- **Node.js** LTS (18 o superior)
- **npm** (10 o superior)
- **PostgreSQL** (versión 16 o 17)

## Estructura
proyecto-agenda/
├─ docs/
│ ├─ entrega1_historias.md
│ ├─ entrega1_casos_uso.puml / .png
│ ├─ entrega1_arquitectura.md
│ ├─ entrega1_arquitectura_capas.puml / .png
│ ├─ entrega1_componentes.puml / .png
│ ├─ entrega1_clases.puml / .png
│ ├─ entrega1_secuencia_crear_evento.puml / .png
│ └─ entrega1_resumen.md # consolidado para exportar a PDF
├─ src/
│ ├─ backend/
│ │ ├─ package.json
│ │ ├─ tsconfig.json
│ │ └─ src/
│ │ ├─ app.ts
│ │ ├─ server.ts
│ │ └─ routes/
│ │ ├─ health.ts
│ │ └─ db.ts
│ └─ frontend/ # (se implementará después)
├─ .gitignore
└─ README.md


---

##️ Instalación y ejecución del backend

1. Clonar el repositorio:

```bash
git clone https://github.com/kevingS0712/agenda-eventos.git
cd agenda-eventos/src/backend

2. Instalar dependencias
npm install

3. crear un archivo .env dentro de src/backend con el siguiente contenido cambiando usuario y pssword por tus credenciales de postgres
PORT=3001
DATABASE_URL=postgresql://usuario:password@localhost:5432/agenda_db

4.
npm run dev

5. Probar endpoints en el navegador o Postman:

http://localhost:3001/health

http://localhost:3001/db/health

Autores

Kevin Adrian Gil Soto (@kevingS0712)


