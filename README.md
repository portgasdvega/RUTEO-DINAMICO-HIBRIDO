# Ruteo Dinámico Híbrido: RIP v2 + OSPF con Redistribución

Este proyecto implementa una red empresarial segmentada en tres áreas (Administración, RRHH y Cómputo) conectadas mediante tres routers. Se usa ruteo dinámico con **RIP v2** y **OSPF**, y se realiza **redistribución de rutas** en el router intermedio (`ROUTER-COM`) para lograr conectividad total entre todos los nodos.

##  Topología Lógica

- Administración: 192.168.1.0/24
- RRHH: 172.16.1.0/24
- Cómputo: 10.10.1.0/24
- Enlaces entre routers:
  - 192.168.2.0/24
  - 10.10.2.0/24
  - 172.16.2.0/24


## Protocolos Usados

- **RIP v2** en `ROUTER-ADM` y `ROUTER-RRHH`
- **OSPF (Area 0)** en `ROUTER-COM`
- Redistribución:
  - De RIP hacia OSPF
  - De OSPF hacia RIP

## Configuraciones

Las configuraciones completas de cada router están disponibles.



