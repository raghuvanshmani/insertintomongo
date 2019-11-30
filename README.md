# insertintomongo
import pymongo
uri = "mongodb://127.0.0.1:27017"
connection =pymongo.MongoClient(uri)
database = connection['gla']
collection = database['student1']
data =[
    {"id":1, "name":"raghuvansh","roll":2,"age":21},
{"id":2, "name":"rag","roll":40,"age":22},
{"id":3, "name":"ragh","roll":20,"age":23},
{"id":4, "name":"raghu","roll":22,"age":24},
{"id":5, "name":"raghuv","roll":24,"age":25}
]
collection.insert_many(data)
