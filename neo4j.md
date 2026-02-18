<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/aa4ff6f6-3233-4706-88ae-068f4b641adf" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/eb83d474-1333-4be7-8275-b38be63f656b" />
<img width="1940" height="1406" alt="image" src="https://github.com/user-attachments/assets/63393a30-8434-4ff9-b1f9-8a53e84cf14e" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/cf1804bb-fa8a-4c73-9c79-08c9eba27097" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/fdf7c8ac-9848-4bd2-aa11-5461f6f5ef8a" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/68983ffd-9a97-48ff-a2d8-4d79d973adc4" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/5a57a444-696e-4e31-ba95-b08318a3eb3f" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/05766948-7509-4ead-9f38-6b1fe4396dfb" />
# just click on movie we will get all movie and see the code as well and we can select anything and get that nodes and if we select rrelationship option we will get relationship
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/594bd099-45c6-4b0f-9e2b-0d98af15864e" />
### Find all movies Kevin Bacon acted in
This query returns both the Person node and all connected Movie nodes.

```cypher
MATCH (p:Person {name: "Kevin Bacon"})-[:ACTED_IN]->(m:Movie) 
RETURN *
```
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/a98e4572-4179-4ca9-a962-b5898e9a07d2" />
### If you only want to see the **titles** of the movies in a list (instead of the nodes/circles), you should suggest this variation:

```cypher
MATCH (:Person {name: "Kevin Bacon"})-[:ACTED_IN]->(m:Movie)
RETURN m.title
```
let see he didn't directed any movie it shows nothing
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/3ab151d8-6b73-40a0-8cbb-7a6497c3dd87" />
see optional match
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/2eaa023a-0beb-4333-93f3-bbff94f08c9e" />
MATCH: If a movie has no director, the movie is hidden from your list.

OPTIONAL MATCH: If a movie has no director, the movie still shows up, but the director's name will just be empty (null).
in Cypher, OPTIONAL MATCH is like the LEFT JOIN in SQL.

It allows you to look for a pattern, but if that pattern doesn't exist, the query doesn't fail and doesn't remove the rest of the results. Instead, it just fills the missing parts with null.

<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/5ecda3b5-350e-47c6-8ad4-bf1b593e8f5e" />
we can get tabular output as well (by using return statement with property)
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/ce490304-a772-49ad-afab-8e7b136c5e6c" />
## WITH processes or filters that data. filter only p or m or both see in the image
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/4e6e717d-e70e-4700-a4a7-e411d6946611" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/b4e30e0a-811f-48e0-a7c3-0bac915e3155" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/5700a348-f6df-4c50-8ced-0b7def13ef88" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/092773e2-052b-40cc-b1de-18e0873ef9d0" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/f32e9493-414e-4885-b5b7-b29e82c34d2f" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/2d2c7230-3094-41af-8cba-65779e124698" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/e8edba05-0865-43e2-a8d4-acebbf7dd561" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/daf355d8-b799-4c26-a048-cd966f46f5e7" />
## creatign a node
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/ba0a5985-3c4a-4997-93ef-52445ef60837" />
created Movie and relationship
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/cec341fe-b7f9-4237-8a4f-8a15cbe013a9" />

for deleting s node first deleet its relationship
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/e897e9de-186e-49f7-8e42-7da4d0e8ef60" />
deleted a relationships and after deleting relationship you can delete node
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/97c764ff-1bb4-41bd-bf4a-07105e5caf8d" />
by using detach delete we can delete any node without deleting the relationship
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/e69d63b3-7eac-42f7-b553-3499d6a63a1f" />
it deleted the node as well as relationships
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/cb79d364-532c-40de-a4c2-2fa16c549a50" />
adding a director label here 
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/fa18aac3-a1dd-4d2d-b3e3-4e2ba431b923" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/141b1c72-c69d-4713-af8d-5f5aded11004" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/59589ef6-299f-4739-9d00-455d8a527b56" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/a97c6d2b-32cf-43b9-9c79-dc262f547df5" />
<img width="1940" height="994" alt="image" src="https://github.com/user-attachments/assets/290a3a50-e575-4e5c-98dc-c69f00042c99" />
# unwind convert the list into object
<img width="1940" height="994" alt="image" src="https://github.com/user-attachments/assets/63b26178-01eb-4770-927b-fdd3f59cf2de" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/f3db1720-c67c-4719-ba79-5558af201563" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/3d51bccc-8fc1-4739-95f5-7d971afa85f9" />
it is running the subquery on the 10 records
<img width="1940" height="994" alt="image" src="https://github.com/user-attachments/assets/f10be330-436f-4f6c-980e-133f96c6a414" />
<img width="1940" height="994" alt="image" src="https://github.com/user-attachments/assets/87e46c99-4296-43fa-8688-ae0e5731d052" />
<img width="1940" height="1260" alt="image" src="https://github.com/user-attachments/assets/5fde86e0-2a6d-4f67-9bea-8013465e23f9" />
<img width="2452" height="1088" alt="image" src="https://github.com/user-attachments/assets/3c8c4cb0-d966-4c5a-9681-609e852bac9d" />

<img width="2452" height="1260" alt="image" src="https://github.com/user-attachments/assets/657217c9-fb3f-4d99-9a01-b97e7677999e" /> 
<img width="2452" height="1088" alt="image" src="https://github.com/user-attachments/assets/a95ff2fd-0b8e-411c-9ff6-5395066403b6" />
<img width="2046" height="1214" alt="image" src="https://github.com/user-attachments/assets/0ede42fe-2cd5-4809-96ee-45176ebeb495" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/7dd97a9f-edcd-4e38-b4d8-764dbc3ce724" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/41364117-bacf-48fc-be80-07853c9499e1" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/63f5c11b-840e-4502-b50a-94da0af7bc52" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/779f6775-eb53-41c4-9c42-8cc3ea5a5628" />
<img width="2046" height="1214" alt="image" src="https://github.com/user-attachments/assets/e1c37a41-707d-43e2-9ef3-e651723136b6" />
to get a particular person
<img width="2046" height="1214" alt="image" src="https://github.com/user-attachments/assets/2a063f14-ab54-44ba-b582-d5a1bef98e43" />
it will give all the records which contains wallace

## relationship defined in a square bracket []
<img width="2046" height="1214" alt="image" src="https://github.com/user-attachments/assets/368c4610-0c29-4bbb-99d7-d2c40872a626" />
<img width="2046" height="1214" alt="image" src="https://github.com/user-attachments/assets/6bc94111-a4a8-4df6-a926-c81825151411" />
<img width="2590" height="1138" alt="image" src="https://github.com/user-attachments/assets/adb826fe-0bd8-4d0a-b1d7-1a5d3665e9dc" />
<img width="2590" height="1138" alt="image" src="https://github.com/user-attachments/assets/c370038e-9279-47a1-909b-9a3e74ae988b" />
<img width="2590" height="1138" alt="image" src="https://github.com/user-attachments/assets/9f2e3036-8586-4915-a558-ba4e9f2d9602" />
<img width="2590" height="1138" alt="image" src="https://github.com/user-attachments/assets/8f1172c5-22af-40e6-a757-47b5517fece8" />
<img width="2590" height="1138" alt="image" src="https://github.com/user-attachments/assets/16205368-0c4d-41d3-9c37-b219e28ca034" />
<img width="2590" height="1138" alt="image" src="https://github.com/user-attachments/assets/00b3b414-6211-47f0-8749-0c048cef0a7d" />

<img width="2590" height="1138" alt="image" src="https://github.com/user-attachments/assets/1cab9ac4-6daf-440c-ba56-d25cb9f2112e" />

<img width="2590" height="1138" alt="image" src="https://github.com/user-attachments/assets/c1a38beb-ea52-4f2d-a07f-64ffd4424da5" />
<img width="2230" height="1404" alt="image" src="https://github.com/user-attachments/assets/c6810c6d-2b6b-4838-91e5-7f77f956da30" />
<img width="2230" height="1164" alt="image" src="https://github.com/user-attachments/assets/07c37bd6-600f-47f7-82a9-dfcfb0655ab7" />

<img width="2230" height="1404" alt="image" src="https://github.com/user-attachments/assets/a35f0540-7149-49fd-8272-f5dc6029b966" />
<img width="2564" height="1078" alt="image" src="https://github.com/user-attachments/assets/8b070f05-e394-4155-acb5-4a97c1944812" />
It will show all the nodes that have an age < 60, see the query  (if all the nodes satisfy true)
<img width="2564" height="1078" alt="image" src="https://github.com/user-attachments/assets/7ebd14b7-83f2-4686-98dd-d9bf358ef233" />

any - if any nodes are true
<img width="2632" height="1078" alt="image" src="https://github.com/user-attachments/assets/237b01d8-422e-4c5d-a794-432db260d9f6" />
<img width="2632" height="1078" alt="image" src="https://github.com/user-attachments/assets/20861a03-e442-468f-8311-5cf637d44e4a" />
<img width="2748" height="1078" alt="image" src="https://github.com/user-attachments/assets/2a541d5e-2207-4f55-9ec6-bd18c212b10f" />
in this, we are checking whether this actor acted in any movie or not 

<img width="2748" height="1078" alt="image" src="https://github.com/user-attachments/assets/37a8ef91-efb3-4069-80e4-9758cfebb609" />
<img width="2748" height="1078" alt="image" src="https://github.com/user-attachments/assets/ace99c60-b8b5-4d90-830d-c1e0a9d8cb59" />
<img width="2748" height="1078" alt="image" src="https://github.com/user-attachments/assets/e5444add-e3d0-4849-a058-981a4efee1ee" />
<img width="2748" height="1078" alt="image" src="https://github.com/user-attachments/assets/d6843586-fad9-4bc1-b2fc-e056ae411ae8" />










<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/0ac33e47-a33d-4591-9862-b3920681b94d" /># browser overview 
add another col

MATCH (m:Movie)
WHERE m.released > 2000
RETURN m, "Hello" AS anotherColumn
LIMIT 5
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/a3bd517a-9f53-4ba4-a093-4ec32ed84f4c" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/b3555053-346e-4ebd-b1b3-bb7f626134e0" />
# to connect own database select blank sandbox write cretae query for table
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/6279b76e-764e-4b0d-a860-0c52cd4909fa" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/b7b72c3c-a48f-4023-ab2d-7e9482d57611" />
# MATCH in neo4j is like select statement in sql
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/6bfe50b3-8e1d-4235-90e8-7b9f245d2159" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/6d1c62e7-a0e4-46bd-8517-d7abb288f0b5" />


--------------------downloaded neo4j desktop
# create instance 
# connect to instance
# select query option and create database
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/a0fcb772-830c-48f4-aced-18d61a055df0" />
# click on relationship to see the graph relation and we can see the query written
MATCH p=()-[]->() RETURN p LIMIT 25;         --for all relationship
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/adbbe2ab-174a-4b5a-816f-7be4337a7c27" />
------------
MATCH (node1)-[rel]->(node2)
RETURN node1,rel,node2 
LIMIT 1
-----------
MATCH (node1)-[rel]->(node2): This searches for a pattern where a starting node (node1) has a directed relationship (rel) pointing to another node (node2).

RETURN node1, rel, node2: This tells the database to output all three parts of that discovery—the two nodes and the link between them.

LIMIT 1: This stops the search as soon as the very first match is found, preventing the database from scanning your entire graph.
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/84a98ff3-60f8-47d9-ad21-48bb46984c07" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/cbe8dda0-1d4d-4cb4-9cb7-57c5dea1b817" />
Acted or Directed
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/89de0605-0e2a-4fab-b84d-10982f26d06c" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/f9ed153a-8371-44ed-8d09-ce72acf192be" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/afc352d3-dc3c-437f-be8b-b904be09f8b0" />
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/f634cc91-1526-4dac-8fb4-860f82321479" />

MATCH (movie:Movie)
MATCH (director:Person)-[:DIRECTED]->(movie)
RETURN movie.title
(Find me all the movies that have a director assigned to them, and just show me the titles of those movies)
This code is a pattern match that looks for all movies in your database and identifies who directed them. It specifically asks for the titles of those movies.

Here is a simple breakdown of the logic:

MATCH (movie:Movie): Find every node that is labeled as a Movie.

MATCH (director:Person)-[:DIRECTED]->(movie): For those movies found, look for a Person node that has a DIRECTED relationship pointing specifically to that movie.

RETURN movie.title: Instead of showing the circles and lines (the nodes), just give me a list of the text titles of those movies.

---sql code
SELECT m.title 
FROM Movies m
JOIN Directed d ON m.id = d.movie_id
JOIN People p ON d.person_id = p.id;
---
<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/bf641f7d-64f3-45f1-84b8-b0b9292ea228" />

<img width="2940" height="1912" alt="image" src="https://github.com/user-attachments/assets/1f871766-606c-41b9-a5a7-45f7210edd6f" />















