# ¿Qué es CVE-2024-28397?

Es una vulnerabilidad de ejecución de código en js2py (intérprete/traductor de JavaScript en Python). Afecta a versiones ≤ 0.74 y se origina en el componente disable_pyimport(). Permite a un atacante eludir las restricciones del “sandbox” y ejecutar comandos arbitrarios mediante una llamada de API manipulada. 

El fallo posibilita escapar del entorno JS, obtener referencias a objetos Python, y terminar invocando APIs sensibles (por ejemplo, subprocess.Popen) para ejecutar comandos del sistema.


# Configuración

Edita las variables en el script para adaptarlas a tu entorno:


    attacker_ip: IP desde donde quieres recibir el comado.

    target_url: URL base del servidor objetivo (ejemplo: http://victimsite.com).

    jwt_cookie: Token JWT válido para autenticación en el servidor.


### Uso

Ejecuta el script:

```python send_payload.py```

-----

# Advertencia

Este script es solo para fines educativos y pruebas autorizadas. No uses este código en sistemas sin permiso explícito.
