# Un día de un gato

Escribamos las vicisitudes de un gato durante el día.

## How To

### 1. Creamos rama nueva

> Completemos el nombre de feature/{lo que sea}

```bash
git checkout -b feature/
```

### 2. Escribimos nuestros cambios

(Abrimos el .txt del día correspondiente)

### 3. Añadimos los cambios a nuestro staging.

```bash
git add .
```

### 4. Commiteamos los cambios a nuestro repo local.

> Usemos nombres descriptivos para nuestros mensajes. Ejemplo: "Se agrega desayuno."

Para más info: https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/

```bash
git commit -m "Mensaje del commit"
```

### 5. Subimos los cambios al repo remoto.

> feature/ es la rama que creamos previamente. El origin se añade porque no existe de forma remota aún.

```bash
git push origin feature/
```

Para "atar" la rama remota a la local basta con poner una vez:

```bash
git push --set-upstream origin feature/
```

En los próximos push, alcanzará con poner solo con git push.

### 6 Queremos incorporar a nuestra rama los cambios de main:

Esto va a traerse los cambios que hay en la rama main a la rama local.


```bash
git pull origin main
```

Si hay un conflicto, se tendrá que resolver y commitear.
