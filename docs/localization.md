# Localization

We use the navigator preferred language to serve the JS Widget. It's built-in so
you don't have to worry about it.

## Force a default language

You can force the display language to be static:

```
<script>

    window._PrudioSettings = {
        language: 'fr'
    };

</script>
```

## Add a language

You can add your own translation with:

```
<script>

    window._PrudioSettings = {
        //...
        language: 'es_MX',
        localization: {
            'es_MX': {
                CHAT_WITH_US: 'Habla con nosotros',
                NAME: 'Nombre',
                EMAIL: 'E-mail',
                START_CONVERSATION: 'Iniciar una conversación',
                NEW_MESSAGE: 'Nuevo mensaje',
                NO_USERS_ONLINE: 'Perdon! Actualmente no hay miembros en línea para ayudarle. Deja un mensaje y trataremos de ponernos en contacto lo antes posible!',
                CONVERSATION_HISTORY: 'Historial de la conversación',
                JUST_WRITE: 'Escriba aqui...',
                PROBLEM_CONNECTING_TO_SERVER: 'Hubo un problema al conectar con el servidor!',
                ERROR_FILL_ALL_FIELDS: 'Por favor, rellene los campos con un nombre y una dirección de correo electrónico válida.',
                CONNECTING_TO_SERVER: 'Conectando con el servidor...',
                SERVER_OFFLINE: 'Servidor está apagado!',
                USER_IS_TYPING: 'El usuario está escribiendo...',
                UPLOADING_FILE: 'Enviando fichero',
                ERROR_UPLOADING_FILE: 'Error al adjuntar fichero!',
                ATTACH_FILE: 'Adjuntar un fichero',
                USER_OFFLINE: 'La internet se ha ido',
                USER_ONLINE: 'Estamos de vuelta!',
                MUTE: 'Silenciar conversación',
                CLOSE: 'Cerrar conversación',
                MINIMIZE: 'Minimizar conversación',
                TITLE: 'Soporte'
            }
        }
    };

</script>
```

## Extend an existing language

You can extend an existing translation:

```
<script>

    window._PrudioSettings = {
        //...
        localization: {
            'es': {
                NAME: 'Su nombre',
                EMAIL: 'Su correo',
            }
        }
    };

</script>
```

## Languages available

Currently we have:

* English (*default*)
* Portuguese
* Spanish
* Turkish
* French
* German
* Romanian
* Portuguese (Brazil)
* more coming soon...
