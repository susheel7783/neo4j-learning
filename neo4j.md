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















