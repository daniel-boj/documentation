# Autenticación del usuario

Para poder acceder a la aplicación, el usuario debe autenticarse con un nombre de usuario y una contraseña válidos para acceder a las aplicaciones de la tarjeta de Ciudadano. La autenticación se realiza mediante el servicio de autenticación de la tarjeta de Ciudadano y podrá configurarse para realizarse automáticamente mediante la autenticación biométrica del dispositivo.

![Autenticación biométrica](./img/sshots/biometrica.png)

![Pantalla de autenticación](./img/sshots/auth.png)

1. Al acceder a la aplicación por primera vez, si no se ha activado en el dispositivo la autenticación biométrica, se mostrará de forma automática el diálogo estandar del dispositivo para activarla. Si el usuario no desea activarla, podrá hacerlo en cualquier momento desde la configuración del dispositivo.
2. En el primer acceso, el usuario deberá introducir su nombre de usuario y contraseña de la Tarjeta Ciudadano de forma manual. Si la autenticación es correcta, se almacenará en el dispositivo de forma encriptada para automatizar los futuros accesos mediante la autenticación biométrica. Si el usuario intentara identificarse con la autenticación biométrica en el primer uso de la aplicación, esta le informará del error y le solicitará que se identifique de forma manual.
3. En los accesos posteriores, el usuario podrá identificarse tanto manualmente como mediante la autenticación biométrica.
4. Si el usuaria no realiza un *cierre de sesión* explícito, la aplicación mantendrá la sesión activa en el dispositivo hasta que el usuario cierre la aplicación o reinicie el dispositivo. De este modo, el usuario no tendrá que identificarse en cada uso de la aplicación y esta volverá a mostrar el estado en el que se encontraba en el último uso.

## Interfaz de uso
1. Formulario de autenticación: Dispone de 2 campos de texto, el primero para introducir el nombre de usuario y el segundo para introducir la contraseña. En el campo de contraseña, a la derecha, hay un icono seleccionable: En forma de *candado*, indica que el contenido de la contraseña se oculta. Al pulsar sobre él, se mostrará el contenido de la contraseña y se mostrará el icono de un *ojo*. Al pulsar de nuevo, se ocultará.
2. Botón de *Enviar*: Pulsando este botón se inicia el proceso de autenticación manual, si las credenciales del usuario son correctas, se procedera a la siguiente pantalla. Si son incorrectas, se mostrará un aviso al usuario.
3. Icono de *huella digital*: Pulsando este icono, se abre el diálogo de identificación biométrida. Si el usuario a cancelado la identificación biométrica, si el dispositivo no dispone de esta funcionalidad o si el usuario no ha activado la autenticación biométrica, este icono mostrará la imagen de una *huella digital con un símbolo de prohibición*.
