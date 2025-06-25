# clase03-2bim

### 25 junio 2025

* Para agregar un numero de telefono a un usuario existen primero desdes el archivo forms.py se crea una clase NumeroTelefonicoEstudianteForm para asociar a un numero de telefono a un estudiante especifico de forma  oculta, se hace pasandole el estudiante como parametro y ocultando el mismo en el formulario para evitar que un usuario cambie este parametro.
* En el archivo view.py se tiene una funcion que permite registrar un nuevo numero de telegono para un usuario especifico. Primero lo busca al estudiante a traves de 'id' como parametro, luego se crea una instancia con el formulario 'NumeroTelefonicoEstudianteForm'.
* Si la solicitud es de tipo 'Post' y los campos dentro del formulario son validos entonces guarda el numero de telefono en el estudiante que tiene asociado y lo redirecciona al index, en cambio si el tipo de solicitud es 'Get' se muestra el formulario vacio.