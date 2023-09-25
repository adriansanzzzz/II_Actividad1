# Práctica 1 - Introducción a Unity
## Asignatura: Interfaces Inteligentes
## Adrián Sanz Fernández - alu0101686400@ull.edu.es

- Incluir objetos 3D básicos.
- Incluir en el proyecto el paquete "Starter Assets".
- Incluir un objeto de la Asset Store que no sea de los "Starter Assets".
- Crear un terreno (opcional).
- Asignar una etiqueta a cada objeto para su identificación.
- Utilizar prefabs de "Starter Asset FPS" o "Third Person".
- Agregar un script que escriba en la consola los objetos utilizados.

### Incluir objetos 3D básicos.
He optado por añadir un cubo. 
1. `GameObject`.
3. `3D Object`.
4. `Cubo`.

###  Incluir en el proyecto el paquete "Starter Assets".
1. `Window`.
3. `Package Manager`.
4. `My assets`.
5. Como en clase se incluyó el Starter Assets - Third Person Character Controller, al importar este se ya se importa el paquete.
<img width="734" alt="image" src="https://github.com/adriansanzzzz/II_Actividad1/assets/74414073/4eb209d1-5123-4bc6-84c6-4368b9e7e3e9">


### Incluir un objeto de la Asset Store que no sea de los "Starter Assets".
He buscado por la Asset Store y he decidido añadir un árbol  https://assetstore.unity.com/packages/3d/vegetation/trees/urp-tree-models-253340
1. `Window`.
3. `Package Manager`.
4. `My assets`.
5. Busco y lo importo.

### Crear un terreno 
1. `GameObject`.
3. `3D Object`.
4. `Terrain`.
Y le he dado una textura a traves de una imagen que incluia el paquete de los arboles, arrastrandole al terreno.

### Asignar una etiqueta a cada objeto para su identificación. 
Desde el menú de jerarquia del proyecto, he ido seleccionado uno a uno y añadiendoles un Tag.
<img width="467" alt="image" src="https://github.com/adriansanzzzz/II_Actividad1/assets/74414073/0aeb8396-ecf6-4fee-b7b4-712ac3391e9f">
<img width="467" alt="image" src="https://github.com/adriansanzzzz/II_Actividad1/assets/74414073/21859cc9-6feb-48bf-ad4f-5be44f466e82">

### Utilizar prefabs de "Starter Asset FPS" o "Third Person".
He añadido el objeto Box_350x250x200_Prefab a los ya existentes.
<img width="1071" alt="image" src="https://github.com/adriansanzzzz/II_Actividad1/assets/74414073/b39d8d2e-a4a3-415d-a786-75caa90f431a">

### Agregar un script que escriba en la consola los objetos utilizados.
Para ello:
1. `Assets`.
3. `Create`.
4. `C# Script`.

```csharp
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class NewBehaviourScript : MonoBehaviour
{
    public string nombre;

    // Start is called before the first frame update
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        Debug.Log("Nombre del objeto: " + nombre);
    }
}
```
Al hacer public el string nombre, nos permite editar directamente desde Unity el nombre.

4. Dentro de cada objeto pulsamos en Add Component y editamos el nombre.
<img width="344" alt="image" src="https://github.com/adriansanzzzz/II_Actividad1/assets/74414073/fcfde699-32cf-48e6-87e1-c331400156b3">
<img width="420" alt="image" src="https://github.com/adriansanzzzz/II_Actividad1/assets/74414073/8c2a1ed0-bf84-4372-9a9b-e6cd0ff4d9fb">

El script nombra los objetos que hay cada vez que se actualiza el frame.

## GIF DEL FUNCIONAMIENTO
![gifv2](https://github.com/adriansanzzzz/II_Actividad1/assets/74414073/8a253271-e335-439f-a6e7-013bb940e1ec)




