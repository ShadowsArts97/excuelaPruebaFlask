# Flask API Project

## Instalación

1. Clona el repositorio:
    ```sh
    git clone <url-del-repositorio>
    cd flask_api_project
    ```

2. Crea y activa el entorno virtual:
    ```sh
    python3 -m venv venv
    source venv/bin/activate

    # otros 
    deactivate
    source venv/bin/activate
    ```

3. Instala las dependencias:
    ```sh
    pip install -r requirements.txt
    ```

4. Configura la base de datos:
    ```sh
    flask db init
    flask db migrate -m "Initial migration."
    flask db upgrade
    ```

5. Ejecuta la aplicación:
    ```sh
    python run.py
    ```

## Endpoints

- `POST /register`: Registro de usuario.
- `POST /login`: Login de usuario.
- `GET /user`: Obtener información del usuario autenticado.
- `PUT /user`: Actualizar información del usuario.
- `DELETE /user`: Eliminar usuario.

## Autenticación

Usa JWT para proteger las rutas que requieren autenticación. Agrega el token en el header `Authorization` como `Bearer <token>`.
