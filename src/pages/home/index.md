---
sidebar_position: 1
---
# Manual de usuario
# Configuración
El nuevo sistema de becas funciona de manera diferente, especialmente en lo que respecta a la configuración. A continuación, se explica cómo funciona y cómo afecta al inicio de sesión de los estudiantes.

## Desde la visión del administrador:

- **Regímenes y ciclos**:
  - Se mantiene la funcionalidad de activar varios regímenes y ciclos a la vez, pero **no es posible activar dos ciclos del mismo régimen**. Esto ayuda a evitar conflictos en el sistema.

- **Renovación y nuevas solicitudes**:
  - Hasta ahora, la renovación se activaba de manera general para todos los tipos de becas activos. No activarla significaba acceso solo a nuevas solicitudes.
  - Ahora, por cada tipo de beca, el administrador puede decidir si acepta **solo renovaciones** o **solo nuevas solicitudes**, lo que permite tener dos tipos de periodos activos para diferentes tipos de becas.

- **Configuración de periodos**:
  - Se mantiene la elección de día, mes, año, hora, minutos y segundos para el inicio y fin del periodo activo.

- **Apertura para estudiantes específicos**:
  - El sistema permite habilitar el acceso solo a ciertos estudiantes específicos, lo que significa que **solo ellos** podrán realizar nuevas solicitudes o renovaciones, dependiendo de los tipos de becas activos.
  - Es obligatorio seleccionar el régimen al que pertenecen esos estudiantes, además del ciclo que se les habilitará.
  - Aunque el sistema esté habilitado solo para algunos estudiantes, **todos los estudiantes** pueden iniciar sesión para revisar el estado de sus solicitudes, siempre y cuando su régimen académico coincida con uno de los habilitados en el sistema.

## Desde la visión del estudiante:

La lógica del sistema para realizar solicitudes se mantiene. Al iniciar sesión, el estudiante verá todas las solicitudes que ha realizado en el año lectivo actual, en orden descendente (la más reciente primero).

### Puntos importantes:

- **Ciclo I**:
  - Si el sistema está habilitado para el **ciclo I** de cualquier régimen, aunque haya tipos de becas habilitados para renovación, no se mostrará el botón de renovación. Esto se debe a que en el ciclo I **no es posible renovar** siendo este el primer ciclo del año lectivo.

- **Validación de solicitudes**:
  - Al iniciar sesión, se validan todas las solicitudes del estudiante realizadas en el año para verificar qué gestión puede realizar.
  - Si alguna solicitud fue aprobada, se compara el tipo de beca de esa solicitud con las becas activas. Solo podrá **renovar** si coincide, y si no coincide con ninguna, solo podrá hacer **solicitudes nuevas**.

- **Gestión permitida**:
  - Al estudiante solo se le mostrarán los tipos de becas que coincidan con la gestión que está realizando. Por ejemplo, si está renovando, solo verá los tipos de becas que tengan activada la renovación.
  - De esta manera, se evita que los estudiantes que deben renovar soliciten una beca nueva a la que no solicitaron antes.

- **Estudiantes habilitados específicamente**:
  - Aunque haya becas activas que coincidan con la gestión del estudiante, no se le permitirá realizar la solicitud si hay al menos un estudiante en la lista de los que se habilitan específicamente.
