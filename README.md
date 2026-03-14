# AgenteImpresion2026-Cajon_v1.3

AGENTE DE IMPRESIÓN

1- Ejecutar el script como ADMINISTRADOR : installServAgenteImpSurfTpv_V1.2.bat

2- Se crea una estructura con todos los archivos en C:\SurfTPV

3- Se instala el servicio de AgenteDeImpresión automaticamente, comprobar funcionamiento tras instalación.

4- Si no se ejecuta servicio SurfTpv_printagent, reinstalar paquete "python-escpos" en entorno.

&gt; **Nota importante:** Si encuentras el error `ModuleNotFoundError: No module named 'pkg_resources'`, ejecuta:

Abre **CMD** como Administrador:

```cmd
cd C:\SurfTPV\AgenteImpresionTPV
C:\SurfTPV\.venv\Scripts\activate.bat
pip install --upgrade setuptools wheel

pip uninstall python-escpos -y

pip install python-escpos
```

5- Edita el fichero:  print_agent_beep.py (añade subdominio, api key, Ip impresoras)

-------------------------------------------------------------------------------------------------
CAJÓN Portamonedas en WINDOWS

1- Instalar AutoHotKey, Se encuentra en C:\SurfTPV\CajonPortamonedas\InstaladorAutoHotKey\AutoHotkey_2.0.19_setup.exe


2- Configurar C:\SurfTPV\CajonPortamonedas\cajon.py con la ip correcta de la impresora donde está conectado el cajón portamonedas.


3- Pulsa TECLA WINDOWS + R y ejecutar :    shell:startup


4- Mover ahí cajon.ahk para que la app AutoHotKey se auto arranque con el sistema y esté escuchando el F3 para abrir el cajón, editar este archivo si se quiere cambiar la tecla


5- Poner acceso directo en Windows de apetura de cajón por si acaso. C:\SurfTPV\CajonPortamonedas\AccesoDirectoEscritorioWin10_11\AbreCajon.lnk
