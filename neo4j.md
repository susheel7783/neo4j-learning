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

---sql code
SELECT m.title 
FROM Movies m
JOIN Directed d ON m.id = d.movie_id
JOIN People p ON d.person_id = p.id;
---

















