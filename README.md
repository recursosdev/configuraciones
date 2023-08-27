# Configuraciones

Algunas configuraciones útiles.

* [Github](#github)

<a id="github"></a>

## Configuraciones Github

### Tokens

Para conectarnos con github, ahora es necesario generar un token de validación

Logueados en github, vamos a ir a [https://github.com/settings/tokens/new](https://github.com/settings/tokens/new)

>Esto se encuentra en el apartado de `settings` que encontraremos en el perfil (imagen arriba derecha), y luego entramos en `Developer settings`, luego en `Personal access tokens` y utilizaremos el `Token (classic)`

* Seleccionamos `repo` en `Select scopes` para tener los accesos.
* Creamos token `Generate token`

En local activar escribiremos en consola:

```bash
git config credential.helper cache
```

>El comando de arriba cachea las credenciales usuario y pasword token para no tener que indicarlo cada vez que hagamos un push.

Cuando nos pida el usuario, indicaremos el usuario de nuestro repositorio, y cuando nos pida el password, indicaremos el **token**.

### Vincular VSCode

Si queremos vincular VSCode para que administre git, directamente nos logueamos desde este IDE y seguimos los pasos que nos va pidiendo.
