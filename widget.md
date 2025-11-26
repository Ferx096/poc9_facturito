# Codigo para colocar en html para el widget

**Importante** : Cambiar el webhookUrl por el personal de n8n

```
    <!-- Chat de n8n - JavaScript -->
    <script type="module">
        import { createChat } from 'https://cdn.jsdelivr.net/npm/@n8n/chat/dist/chat.bundle.es.js';
        
        createChat({
            webhookUrl: 'https://inadvance.app.n8n.cloud/webhook/faa21603-f8af-4b1e-9058-417a8f6c8151/chat',
            webhookConfig: {
                method: 'POST',
                headers: {}
            },
            target: '#n8n-chat',
            mode: 'fullscreen',
            chatInputKey: 'chatInput',
            chatSessionKey: 'sessionId',
            loadPreviousSession: true,
            metadata: {},
            showWelcomeScreen: false,
            defaultLanguage: 'es',
            initialMessages: [
                
                '¡Hola!👋, Soy FACTURITO, tu asistente virtual para consultas sobre guías operativas de proveedores e información de facturas de Prima.',
                '¿En qué puedo ayudarte hoy?'
            ],
            i18n: {
                es: {
                    title: 'FACTURITO 🤖',
                    subtitle: "Disponible 24/7 para ayudarte",
                    footer: '',
                    getStarted: 'Nueva Conversación',
                    inputPlaceholder: 'Escribe tu consulta aquí...',
                },
            },
            enableStreaming: false,
        });
    </script>
```

### Docuemntacion donde detalla el procedimiento por n8n
[docuemntacion n8n](https://www.npmjs.com/package/@n8n/chat)
