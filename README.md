# Proyecto: Desarrollo de una aplicación web para estudiantes
## Objetivo.
Los estudiantes podrán accesar facilmente información a la aplicación a través de sus dispositivos para llevar un mapeo y un historial de sus conocimientos así como generar terjetas de estudio que les permitan recordar más facilmente la imformación o tenerla disponible en cualquier momento.
## Descripción.
Este proyecto planea combinar las ventajas de diversas aplicaciones de estudio como Notion, Obsidian o Anky, _tales como poder generar nodos que dirijan la información de un concepto a otro, poder incertar imágenes, generar tarjetas de memoria y demás,_ a fin de concentrar en un solo espacio diversas funciones que satisfagan a todos los usuarios.

![image](https://github.com/user-attachments/assets/4e56acb7-5ccc-4cc4-8230-5c1b18f74fb0)

## ¿Qué nos permite la aplicación?

1. Crear páginas donde poder almacenar información sin límite
2. Inseter imágenes en estas páginas desde la web.
3. Insertar tablas y listas.
4. Crear páginas dentro de páginas ya existentes.
5. Crear calendarios y rutinas que el usuario proponga.
6. Generar hipervinculos a páginas desde la web.
7. Generar notas con apuntes escritos con stylus.
8. Generar targetas de estudio con la información dentro de la aplicación.
9. Lectura y modificación de pdf.
10. Insertar código de cualquier lenguaje y mostrarlo con colores
## Configuraciones
- La aplicación acepta ***modo normal*** y ***modo obscuro***
- Configuración para el tamaño y tipo de letra
- Inmersión en la ***pantalla copleta*** o sincronización con otras aplicaciónes para ***pantalla dividida*** o en ***segundo plano***.
- Sincronización para trabajar entre varios dispositivos ya sean de computadora o de telefono.

## Ejemplo de inserción de código en la plataforma.
```ruby
using System;
using System.Threading;
namespace Expendedoras_2025_1
{
    public class Expendedora
    {
        #region Atributos

        private string _marca;
        private sbyte _temperatura;
        private ushort _cantProductos;
        private float _precio;

        public sbyte Temperatura { get => _temperatura; 
            set 
            {
                if (value >= 10 && value < 21)
                { 
                    _temperatura = value; 
                }
                else
                    _temperatura = 18;
            }
        }

        public string Marca { get => _marca; set => _marca = value; }
        #endregion

        public void Saludar()
        { 
        
            Console.WriteLine("{0} Bienvenido, elige tu producto \n Temperatura {1} °C", Marca, Temperatura);

        }
        #region Constructores
        public abstract Expendedora()
        {
        
            //_temperatura = 25;
            //_precio = 15;
            //Marca = "AWS";
            //Saludar();
            //ClearDisplay();
            //string codigo = MostrarProducto();
            //Thread.Sleep(5000);
            //Console.Clear();
            //MostrarPrecio(codigo);
        }
        public Expendedora(bool mantenimiento)
        {
            if (mantenimiento)
            {
                Console.WriteLine("Hola, Ingrea la nueva temperatura:");
                    _temperatura = sbyte.Parse(Console.ReadLine());
                Console.WriteLine("Temperatura actualizada {0}",_temperatura);
            }
            else
            {
                Console.WriteLine("Modo estandar");
            }
        }
        #endregion
        public void ClearDisplay()
        {
            Thread.Sleep(5000);
            Console.Clear();
        }
        public string MostrarProducto()
        {
            string codigo;
            Console.WriteLine("2A: Papas \t 3C: Chocolate");
            Console.WriteLine("Ingrese el código del producto");
            codigo = Console.ReadLine();   
            return codigo;
        }

        public void MostrarPrecio (string codigo)
        {
            switch (codigo)
            {
                case "2A":
                    Console.WriteLine("Precio: ${0}", _precio);
                    break;
                case "3C":
                    Console.WriteLine("Precio: ${0}", _precio +=5);
                    break;
                default:
                    Console.WriteLine("Producto no encontrado");
                    break;
            }
            }
    }
}
```
## Creador

Héctor Abad Rodríguez.

### Contactos 

📫: har472004@gmail.com.

😄: [Facebook](https://www.facebook.com/hector.abadrodriguez.94)
### Proyecto generado por y para la Facultad de Ingeniería
![image](https://github.com/user-attachments/assets/8533cd40-0017-4f00-b130-7ace1afea818)

## Contributing

Nuevos contribuidores al proyecto siempre son bienvenidos!

Mandar un mensaje a `har472004@gmail.com` para formar parte del proyecto. Poner el correo `Asunto: Contribución para proyecto web`.

## Licencias


[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
