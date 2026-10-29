<!-- Plantilla README para librerías/paquetes. Reemplaza todo lo que está entre {{ }} y borra las secciones que no apliquen. -->
# {{nombre-paquete}}

[![npm](https://img.shields.io/npm/v/{{nombre-paquete}})](https://www.npmjs.com/package/{{nombre-paquete}})
[![CI](https://github.com/{{usuario}}/{{repo}}/actions/workflows/ci.yml/badge.svg)](https://github.com/{{usuario}}/{{repo}}/actions/workflows/ci.yml)
[![Licencia](https://img.shields.io/badge/licencia-{{MIT}}-blue)](LICENSE)

> {{Una frase: qué hace y para quién. Ej.: "Valida RFC, CURP y NIF en una línea, sin dependencias."}}

## Características
- {{Ventaja concreta 1 (ej.: "Sin dependencias, 3 kB minificado")}}
- {{Ventaja concreta 2}}
- {{Ventaja concreta 3}}

## Instalación
```bash
{{npm install nombre-paquete}}
# o: {{pip install nombre-paquete}} · {{cargo add nombre-paquete}}
```
Requiere {{Node.js ≥ 20 / Python ≥ 3.10}}.

## Uso rápido
```js
{{import { validar } from 'nombre-paquete';

validar('ABC123');   // => true}}
```

## API
### `{{funcion(parametro, opciones?)}}`
{{Descripción breve.}}

| Parámetro | Tipo | Por defecto | Descripción |
|---|---|---|---|
| `{{parametro}}` | `{{string}}` | — | {{Qué es}} |
| `{{opciones.estricto}}` | `{{boolean}}` | `{{false}}` | {{Qué cambia}} |

**Devuelve:** `{{tipo}}` — {{qué significa}}.
**Lanza:** `{{TipoDeError}}` si {{condición}}.

## Ejemplos
- {{Caso de uso real 1, con código}}
- Más ejemplos en [`ejemplos/`](ejemplos/).

## Compatibilidad
| {{Entorno}} | Soportado |
|---|---|
| {{Node.js 20+}} | ✅ |
| {{Navegadores modernos}} | ✅ |

## Preguntas frecuentes
**{{¿Pregunta frecuente?}}** {{Respuesta corta.}}

## Contribuir
¡Las contribuciones son bienvenidas! Lee [CONTRIBUTING.md](CONTRIBUTING.md) y el [Código de Conducta](CODE_OF_CONDUCT.md).
Los cambios de cada versión están en [CHANGELOG.md](CHANGELOG.md).

## Licencia
[{{MIT}}](LICENSE) © {{año}} {{tu nombre}}
