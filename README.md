# MFA_para_roles_administrativos.

Esta recomendación de Secure Score en Azure, denominada "Requerir MFA para roles administrativos" tiene un impacto de +17.86% en la seguridad. 

## Descripción. 
Requerir autenticación multifactor (MFA) para todos los roles administrativos hace que sea más difícil para los atacantes obtener acceso a las cuentas. Los roles administrativos tienen permisos superiores a los usuarios normales. Si alguna de estas cuentas se ve comprometida, será posible atacar datos y dispositivos críticos.

## Impacto en los usuarios.
Low

## Implementación

En la página de acceso condicional, hacemos clic en el botón "New Policy".
![New Policy](./img/202303140952.png)

1. Seleccione + Nueva directiva
2.Vaya a Asignaciones > Usuarios y grupos > Incluir >  elija Seleccionar usuarios y grupos  > marque Roles de directorio
3. Como mínimo, seleccione los siguientes roles:
Administrador de seguridad
Administrador del servicio de Exchange
Administrador global
Administrador de acceso condicional
Administrador de SharePoint
Administrador del servicio de asistencia técnica
Administrador de facturación
Administrador de usuarios
Administrador de autenticación
4. Vaya a Aplicaciones en la nube o acciones > Aplicaciones en la nube > Incluir > seleccione Todas las aplicaciones en la nube (sin excluir ninguna aplicación)
5. En Controles de acceso > Conceder > seleccione  Conceder acceso > marque Requerir autenticación multifactor  (nada más)
6. Habilitar directiva > Activado
7. Crear

Nota: no se puntúan las directivas de acceso condicional clásico. Siga los pasos recomendados para recibir crédito.
Cuentas de acceso de emergencia: si la organización ha configurado cuentas de administrador global adicionales para escenarios de emergencia que no están protegidas por MFA, se recomienda que establezca el estado de control en "Riesgo aceptado".
HOW WILL IT AFFECT MY USERS? 
Primero, los usuarios con roles administrativos deben registrarse para la MFA. Después de que se registre cada administrador, las directivas determinan cuándo se les solicitan los factores de autenticación adicionales.

Get Started
Secure score updates can take up to 48 hours.