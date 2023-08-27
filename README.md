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

Hora cuando hagamos un push, nos va a solicitar usuario (user) y contraseña (password).

Cuando nos pida el usuario, indicaremos el usuario de nuestro repositorio, y cuando nos pida el password, indicaremos el **token** generado.

Para no volver a escribir el usuario y el token cada vez que hacemos un push a github, podemos indicar a git que cachee `cache` por un tiempo corto (un día por ejemplo), o bien guarde `store` en el disco definitivamente.

Para el caché utilizaremos esta línea siempre ubicados dentro de nuestro proyecto:

```bash
git config credential.helper cache
```

Y para almacenarlo en el dico definitivamente:

```bash
git config credential.helper store
```

### Vincular VSCode

Si queremos vincular VSCode para que administre git, directamente nos logueamos desde este IDE y seguimos los pasos que nos va pidiendo.
