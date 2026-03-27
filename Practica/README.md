# Configuración Wazuh de un EDR

# Distribución

Tengo dos maquinas una maquina con Wazuh instalado con una IP 10.0.2.11 y otra maquina Kali con IP 10.0.2.6


# Ejecución

# 1. Instalar y configurar el agente de Wazuh
Acceso desde la maquina Kali mediante el navegador a la IP 10.0.2.11 que es la de nuestra maquina con Wazuh y vemos un boton el cual nos permite crear un agente.
![Create new agent](/images/create_new_agent_1.png)

Despues tenemos una pagina de configuracion del agente en el cual añadimos el SO y la IP de la maquina Wazuh, tambien añadimos un nombre al agente, y nos da unos comandos que hay que ejecutar en el endpoint(maquina Kali)

![Configurar agente 1](/images/config_agent_1.png)

![Configurar agente 2](/images/config_agent_2.png)

Volvemos al dashboard y entramos en la seccion de agentes y vemos que hay un agente creado con el nombre que le pusimos y con la ip de la maquina con Wazuh.

![Confirmacion agente](/images/confirmacion_agent.png)


# 2. Simulación de amenazas

Creamos un documento de texto y en el agent vemos como hay un registro sobre ese comando

En la parte principal nos informa del uso de sudo

![Prueba de texto ](/images/agente_prueba_texto.png)

Cuando pedimos mas informacion nos informa de que comando se esta usando con el sudo

![Informacion del comando](/images/agente_prueba_texto_1.png)


