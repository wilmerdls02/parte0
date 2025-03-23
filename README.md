parte0

0.4: Nuevo diagrama de nota

sequenceDiagram

partcipant Usuario

partcipant Navegador

partcipant Servidor

Usuario->> Navegador: Hece clic en el boton del formulario

Navegador->>Servidor: Post /nwe_nota (con el contenido de la notas)

Servidor-->>Navegador: Respuesta 201 Created

Navegador-->>Servidor: Get /notes (para actualizar la lista de notas)

Servidor-->>Navegador: Json con todas las notas

Navegador-->>Usuario: Muestra la nueva nota en la pagina
