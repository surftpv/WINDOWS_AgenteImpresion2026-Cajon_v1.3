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
