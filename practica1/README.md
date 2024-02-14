## DOCUMENTACION SOBRE LA PRACTICA 1

### Tabla comparativa de tiempos de convergencia

| Escenario | Protocolo STP | Red Primaria | Red Basicos | Red Diversificado |
|-----------|----------------|--------------|-------------|-------------------|
| 1         | PVST           | 59.77 segundos | 59.17 segundos | 59.99 segundos |
| 2         | Rapid PVST     | 43.52 segundos | 0 segundos | 8.37 segundos |


### Protocolo PVST

##### VLAN Primaria
- Ping desde 192.168.11.5 hasta 192.168.11.2
- En el switch root se desactiva la interfaz 0/1
- El protocolo tarda en restaurar la conexión 59.77 segundos

##### VLAN Basicos
- Ping desde 192.168.21.3 hasta 192.168.21.2
- En el switch root se desactiva la interfaz 0/1
- El protocolo tarda en restaurar la conexión 59.17 segundo

##### VLAN Diversificado
- Ping desde 192.168.31.5 hasta 192.168.31.2
- En el switch root se desactiva la interfaz 0/1
- El protocolo tarda en restaurar la conexión 59.19 segundos

### Protocolo Rapid PVST

##### VLAN Primaria
- Ping desde 192.168.11.5 hasta 192.168.11.2
- En el switch root se desactiva la interfaz 0/1
- El protocolo tarda en restaurar la conexión 43.52 segundos

##### VLAN Basicos
- Ping desde 192.168.21.3 hasta 192.168.21.2
- En el switch root se desactiva la interfaz 0/1
- El protocolo tarda en restaurar la conexión 0 segundos

##### VLAN Diversificado
- Ping desde 192.168.31.5 hasta 192.168.31.2
- En el switch root se desactiva la interfaz 0/1
- El protocolo tarda en restaurar la conexión 8.37 segundos

### Conclusion:
El mejor escenario es cuando se elige el protocolo **Rápido PVST** porque los tiempos de convergencia son mucho más rápidos, y de esta forma se evita la pérdida de paquetes en las comunicaciones.
