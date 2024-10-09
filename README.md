# movil-corte-2-1007258220
# Proyecto de Gestión de Usuarios y Actividades

## Descripción
Este proyecto tiene como objetivo desarrollar un sistema básico de gestión de usuarios y actividades. El sistema permitirá registrar usuarios, asociar una contraseña a los mismos y gestionar actividades que solo los usuarios autenticados podrán crear.

### Requisitos
1. **Crear la entidad Usuario**: Esta entidad debe tener los siguientes atributos:
   - Nombre
   - Apellido
   - Correo
   - Dirección
   - Teléfono
   - Contraseña
   
   > **Nota**: No es necesario normalizar la entidad "Persona". Todos los atributos estarán en la entidad "Usuario".

2. **Proceso de Registro de Usuarios**:
   - El sistema debe mostrar una pantalla para registrar a una persona. Aunque se utilice la misma entidad `Usuario`, en esta pantalla se ingresarán los datos personales de la persona.
   - Al confirmar el registro, se debe mostrar otra pantalla para asociar una contraseña a este usuario.
   - En este momento, el usuario quedará registrado.

3. **Autenticación e Inicio de Sesión**:
   - Una vez registrado, el usuario puede iniciar sesión directamente.
   - Al iniciar sesión, se activarán dos opciones:
     - **Crear Actividades**
     - **Actualizar Perfil**: Permite actualizar los datos personales del usuario.

4. **Crear la entidad Control de Actividades**:
   - Esta entidad debe incluir los siguientes campos:
     - Código de la actividad
     - Fecha
     - Nombre de la actividad
     - Descripción

   > **Nota**: Solo los usuarios autenticados podrán crear actividades. No se permite la creación de actividades sin autenticación.

## Pasos para el desarrollo

### 1. Configurar el ambiente de desarrollo
1. Instala las dependencias del proyecto:
   ```bash
   npm install
