# Automatización de Entrega de Códigos

## Descripción

Sistema de automatización desarrollado en Make para gestionar solicitudes de códigos de autorización mediante Telegram.

## Tecnologías utilizadas

- Make
- Telegram Bot API
- Airtable
- Outlook
- Groq

## Arquitectura

Usuario → Telegram → Make → Airtable → Outlook → Telegram

## Human In The Loop (HITL)

1. El usuario solicita un código.
2. Se crea un registro en Airtable.
3. El estado queda como "Esperando autorización".
4. Un administrador revisa la solicitud.
5. El administrador cambia el estado a:
   - Autorizado
   - Denegado
6. Un segundo escenario monitorea Airtable.
7. El proceso continúa únicamente después de la aprobación humana.

## Estructura del repositorio

### /blueprints

Contiene los escenarios exportados desde Make.

### /docs

Contiene la documentación técnica y diagramas del proyecto.

## Mejoras futuras

- Gestión de múltiples administradores.
- Integración con WhatsApp.
- Auditoría avanzada.
- Roles y permisos.

ACLARACIONES:se agregan las nuevas capturas a docs.
