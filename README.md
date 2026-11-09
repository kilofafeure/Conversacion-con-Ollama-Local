Chat con Ollama
Un proyecto simple para probar Ollama en local, construido con HTML, CSS y JavaScript vanilla.

## Estructura del proyecto

```
├── index.html      # Estructura principal
├── main.css        # Estilos
└── script.js       # Lógica de interacción con Ollama
```

## Requisitos previos

Ollama instalado y corriendo en tu máquina
El modelo gemma4:e2b descargado

Abre index.html en tu navegador. Puedes hacerlo directamente haciendo doble clic en el archivo o usando un servidor local como Live Server en VS Code.

Escribe tu mensaje en el textarea y pulsa Enviar.

## Cómo funciona

El usuario escribe un prompt en el campo de texto.
Al pulsar Enviar, se realiza una petición POST al endpoint /api/generate de Ollama:
Modelo: gemma4:e2b
Streaming: desactivado (stream: false)
El botón se deshabilita y se muestra un estado de "Pensando..."
La respuesta se muestra en el área de resultados.
Si hay un error de conexión, se muestra un mensaje de error.

## 🔌 API invocada

| Propiedad | Valor |
| --- | --- |
| Endpoint | `http://localhost:11434/api/generate` |
| Método | `POST` |
| Modelo | `gemma4:e2b` |
| Streaming | `false` |
| Content-Type | `application/json` |

## Notas

El proyecto es una prueba básica de interacción con Ollama. No incluye historial de conversación ni modo streaming.
Para cambiar el modelo, edita la línea model en script.js.

## Licencia
Proyecto personal sin licencia.
