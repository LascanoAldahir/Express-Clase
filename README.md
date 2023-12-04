# Express-Clase
// //estructura del servidor web en Express

// //invocar la libreria de express
// const express = require('express')
// //creamos una instancia 
// const app= express()
// // se ejecutara en el puerto 3000
// app.listen(3000)
// console .log ("Web server ejecutandose en el puerto 3000")

// //el metodo get tiene dos cosas la ruta y que va a ejecutar en la funcion flecha es el request y response
// //todo eso es una RUTA
// //resquest es lo que quiero mandar a la ruta
// //cuando ingrese a / (ruta) dara lo siguiente
// app.get('/',(req,res)=>{
//     res.send("Bienvenidos")
// })

// app.get('/dashboard',(req,res)=>{
//     res.send("Dashboard principal")
// })

// app.use((req,res)=>{
//     res.send("404 - Not Found")
// })

// app.get(3000)


//-----------------------------------
//REQUEST

//Creacion de un servidor web en Express
//const express = require('express')
//creamos una instancia 
//  const app= express()

//  //OJO
// //  GET = obtener
// //  Post = registrar
// //  put = Actualizar
// //  Delete =eliminar

//  //Mandar infor en formato JSON
//  app.use(express.json())
// //post es para Registrar
//  app.post('/register',(req,res)=>{
//     const {pedido, solicitado} = req.body //Desestructuracion JS
//     res.send(`El pedido de ${pedido} es realizado por ${solicitado}`) //Backting
//  })

//  app.listen(3000)

 //--------------------------------------------------
 //PARAMS
//  //Creacion de un servidor web en Express}
// const express = require('express')

// //creamos una instancia 
// const app= express()

// //Mandar infor en formato JSON
//  app.use(express.json())

//  app.get('/pedido/:tipo',(req,res)=>{
//     res.send(`El pedido es hamburguesa ${req.params.tipo}`)
//  })

//  app.listen(3000)

//----------------------------------------------------------------

 //QUERY PARAMS
 //pedir texto
 //Creacion de un servidor web en Express}
//  const express = require('express')

//  //creamos una instancia 
//  const app= express()
 
//  //Mandar infor en formato JSON
//   app.use(express.json())

//   app.listen(3000)
//   console .log ("Web server ejecutandose en el puerto 3000")
 
// app.get('/hamburguesa/simple',(req,res)=>{
//     res.send("Hamburguesa - simple")
// })
 
//ahora fotos

//  //Creacion de un servidor web en Express}
//  const express = require('express')

//  //creamos una instancia 
//  const app= express()
 
//  //Mandar infor en formato JSON
//   app.use(express.json())

//   app.listen(3000)
//   console .log ("Web server ejecutandose en el puerto 3000")
 
// app.get('/hamburguesa/simple',(req,res)=>{
//     res.send("Hamburguesa - simple")
// })

// console.log(__dirname)

// app.get('/hamburguesa/doble',(req,res)=>{
//     res.sendFile('./Krabbenburger.JPG.webp',{
//         root:__dirname
//     })
// })

//DEVOLVER CONTENIDO DE ARCHIVO WORLD

 //Creacion de un servidor web en Express}
//  const express = require('express')

//  //creamos una instancia 
//  const app= express()
 
//  //Mandar infor en formato JSON
//   app.use(express.json())

//   app.listen(3000)
//   console .log ("Web server ejecutandose en el puerto 3000")
 
// app.get('/hamburguesa/simple',(req,res)=>{
//     res.send("Hamburguesa - simple")
// })

// console.log(__dirname)

// app.get('/hamburguesa/doble',(req,res)=>{
//     res.sendFile('./triple.docx',{
//         root:__dirname
//     })
// })


//--------------------------------------------------------------
// //devolver como json
//  //Creacion de un servidor web en Express}
//  const express = require('express')

//  //creamos una instancia 
//  const app= express()
 
//  //Mandar infor en formato JSON
//   app.use(express.json())

//   app.listen(3000)
//   console .log ("Web server ejecutandose en el puerto 3000")
 
// app.get('/hamburguesa/simple',(req,res)=>{
//     res.send("Hamburguesa - simple")
// })

// console.log(__dirname)

// app.get('/hamburguesa/mixta',(req,res)=>{
//     res.status(200).json({
//         "tipo": "Mixta",
//         "extra": "No"
//     })
// })

//--------------------------------------------------------------------------

//DEVOLVER UNA PAGINA
//Creacion de un servidor web en Express}
const express = require('express')
const {engine}=require('express-handlebars')

import{engine} from 'express-handlebars'; //ESMODULES

//utilizar un motor de plantillas
app.engine(`handlebars`,engine())

//ubicacion del directorio views
app.set('views', './src/vies')



//extension de las paginas
app.set('view engine','handle')

//creamos una instancia 
const app= express()


//Mandar infor en formato JSON
 app.use(express.json())

 app.listen(3000)
 console .log ("Web server ejecutandose en el puerto 3000")

app.get('/hamburguesa/simple',(req,res)=>{
   res.send("Hamburguesa - simple")
})

console.log(__dirname)
