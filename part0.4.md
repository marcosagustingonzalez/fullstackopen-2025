flowchart TD
    A[Usuario escribe una nota en el campo de texto] --> B[Usuario hace clic en el botón "Save"]
    B --> C[Browser previene el comportamiento por defecto del formulario]
    C --> D[JavaScript captura el contenido del input]
    D --> E[Se crea un objeto con la nota y la fecha actual]
    E --> F[JavaScript envía una solicitud POST al servidor con la nueva nota]
    F --> G[Servidor recibe la solicitud y guarda la nota]
    G --> H[Servidor responde con un redireccionamiento a /notes]
    H --> I[Browser carga nuevamente la página /notes]
    I --> J[Browser repite las solicitudes: HTML, CSS, JS, JSON]
    J --> K[La nueva nota aparece listada en la página]

    click F href "https://studies.cs.helsinki.fi/exampleapp/notes" "Ir a la app"
