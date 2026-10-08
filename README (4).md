# Checklist Solferino · Anáhuac Cancún

Página para pasar lista (entrada y salida), controlar documentos y guardar el registro en GitHub.

## Contenido

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La página completa (lista de alumnos, registro, PDF, CSV, respaldo y guardado en GitHub) |
| `libs/` | Librerías para generar el PDF (incluidas, no hay que instalar nada) |
| `registro/` | Aquí se guarda `registro.json`, el registro de entradas y salidas |
| `.nojekyll` | Evita que GitHub Pages procese los archivos |

## 1. Subir los archivos a GitHub

1. Entra a <https://github.com/new> y crea un repositorio, por ejemplo `solferino-checklist`.
   **Recomendado: privado** (ver "Privacidad" abajo).
2. Pulsa **uploading an existing file** y arrastra **todo el contenido de esta carpeta** (incluida `libs` y `registro`). Haz commit.

## 2. Publicar la página (GitHub Pages)

1. En el repositorio: **Settings → Pages**.
2. En **Build and deployment**, elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`, y guarda.
3. En uno o dos minutos la página queda en `https://TU-USUARIO.github.io/solferino-checklist/`.

## 3. Crear el token para guardar el registro

1. GitHub → tu foto → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. **Repository access:** *Only select repositories* → elige solo `solferino-checklist`.
3. **Permissions → Repository permissions → Contents: Read and write**.
4. Pon una fecha de vencimiento corta (por ejemplo, unos días después del viaje) y copia el token (`github_pat_…`).

## 4. Usar la página

1. Abre la página en el celular o la computadora.
2. Baja a **Guardar en GitHub**, escribe `usuario/solferino-checklist` (si usas GitHub Pages, ya sale solo) y pega el token. Se queda guardado en ese dispositivo.
3. Pasa lista normalmente. Pulsa **Guardar en GitHub**, o activa **Guardar automáticamente**.
4. Con varios dispositivos: cada uno combina su registro con el de GitHub al guardar, sin borrar nada. **Traer de GitHub** descarga lo que registraron los demás.
5. Al terminar: **Descargar PDF** (también CSV y respaldo `.json`).

El registro queda en `registro/registro.json`. Cada guardado es un commit, así que el historial de GitHub conserva todas las versiones.

## Privacidad (importante)

La página contiene nombres y matrículas de alumnos (incluidas notas sobre menores de edad), y `registro.json` también. **No uses un repositorio público.**

- GitHub Pages desde un repositorio privado puede requerir un plan de pago; revisa la documentación de GitHub, o el beneficio de GitHub Education para docentes.
- Si no puedes publicar la página privada, otra opción es abrir `index.html` directamente desde el dispositivo (o alojarla en otro lugar) y usar GitHub solo para guardar el registro en el repositorio privado: la función **Guardar en GitHub** funciona igual.
- El token se guarda en el navegador del dispositivo. No lo compartas y usa **Quitar token de este dispositivo** al terminar.

## Notas

- Sin internet, la página sigue registrando en el dispositivo (los datos están en el navegador). El guardado en GitHub se hace cuando vuelva la señal. Abre la página con señal antes de salir para que cargue completa.
- Para cambiar la lista de alumnos: usa **+ Alumno** y el lápiz de cada tarjeta dentro de la página.
