---
lab:
    title: 'Explore Azure Synapse Analytics'
    module: 'Module 1: Get Started with Data Engineering'
---

# Explore Azure Synapse Analytics

Azure Synapse Analytics proporciona una plataforma de análisis de datos única y consolidada para análisis de datos de extremo a extremo. En este laboratorio, explorará varias formas de ingerir y explorar datos. Este laboratorio está diseñado como una descripción general de alto nivel de las diversas funcionalidades principales de Azure Synapse Analytics; que explorarás con más profundidad en laboratorios posteriores.

Este laboratorio tardará aproximadamente **90** minutos en completarse.

## Antes de empezar

Necesitará una [suscripción de Azure](https://azure.microsoft.com/free) en la que tenga acceso de nivel administrativo.

## Aprovisionamiento de un área de trabajo de Azure Synapse Analytics

Un *área de trabajo* de Azure Synapse Analytics proporciona un punto central para administrar los tiempos de ejecución de datos y procesamiento de datos. Puede aprovisionar un área de trabajo mediante la interfaz interactiva del Portal de Azure o puede implementar un área de trabajo y recursos dentro de ella mediante un script o una plantilla.

1. Inicie sesión en [Azure Portal](https://portal.azure.com).
2. Use el botón **[>_]** a la derecha de la barra de búsqueda en la parte superior de la página para crear un nuevo Cloud Shell en Azure Portal, seleccionando un entorno ***PowerShell*** y creando almacenamiento si se le solicita. El shell en la nube proporciona una interfaz de línea de comandos en un panel en la parte inferior de Azure Portal.
3. Tenga en cuenta que puede cambiar el tamaño del shell de la nube arrastrando la barra separadora en la parte superior del panel o utilizando los iconos **—**, *◻* y **X** en la parte superior derecha del panel para minimizar, maximizar y cerrar el panel. Para obtener más información sobre el uso de Azure Cloud Shell, consulte la [documentación de Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview).
4. En el panel de PowerShell, escriba los siguientes comandos para clonar este repositorio:

    ```
    rm -r dp-000 -f
    git clone https://github.com/GraemeMalcolm/data-engineer-es dp-000
    ```
5. Una vez clonado el repositorio, escriba los siguientes comandos para cambiar a la carpeta de este laboratorio y ejecute el script **setup.ps1** que contiene:

    ```
    cd dp-000/Allfiles/Labs/01
    ./setup.ps1
    ```

6. Cuando se le solicite, escriba una contraseña adecuada para establecer para el grupo de SQL de Azure Synapse.

> **Nota**: ¡Asegúrese de recordar esta contraseña!
