#Introdução ao MongoDB
*MongoDB é um banco de dados orientado a documentos, de código aberto, e que fornece alto desempenho,
alta disponibilidade e escala automática. MongoDB elimina a necessidade um Mapeamento por Objeto Relacional(ORM)
facilitando assim o desenvolvimento.*

## Documentos
*Um registo no MongoDB é um documento,que é uma estrutura de dados composta de pares de campo e de valor.
Documentos MongoBD podem ser comparados a objetos JSON. Os valores dos campos podem incluir outros documentos,
matrizes e matrizes de documentos.

```{
   "_id" : ObjectId("54c955492b7c8eb21818bd09"),
   "address" : {
      "street" : "2 Avenue",
      "zipcode" : "10075",
      "building" : "1480",
      "coord" : [ -73.9557413, 40.7720266 ]
   },
   "borough" : "Manhattan",
   "cuisine" : "Italian",
   "grades" : [
      {
         "date" : ISODate("2014-10-01T00:00:00Z"),
         "grade" : "A",
         "score" : 11
      },
      {
         "date" : ISODate("2014-01-16T00:00:00Z"),
         "grade" : "B",
         "score" : 17
      }
   ],
   "name" : "Vella",
   "restaurant_id" : "41704620"
}``` 




