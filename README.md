# MongoDb-Kata

run docker compose
`docker-compose -f docker/docker-compose.yml -p mongoKata up`

run the below to import data:

`brew install mongodb/brew/mongodb-database-tools`

`mongoimport --db mongo_kata --collection Students --file ./data/Students.json`
`mongoimport --db mongo_kata --collection Hobbies --file ./data/Hobbies.json`


## Questions

1. Find any 10 students and their marks 

2. Find the list of students sorted alphabetically by their name (A-Z)

3. Find all students who scored > 50 in homework

4. Find all students who scored <20 in homework and exam

5. How many students have a quiz, homework and exam score > 85

6. Find the top 10 students with the best exam score

7. Find the bottom 10 students based on quiz score

8. Find each student’s average mark across all areas

9. What is the overall average exam score for all students


# Part 2 (Hobbies)

## Insert / Update / Delete

1. Insert a document for William. He has no hobbies.

2. Using one query - add 3 more people to list: 
    - 'Beethoven' who loves 'music' 
    - 'Bugs Bunny' who eats 'carrots' all day
    - 'Snoopy' who has no hobbies

3. Update William's document to include a hobby :'jigsaw puzzles'

4. Update everyone's records to include another column `likes_dessert` = true 

Bonus Q : update the above if they have 2 or more hobbies

5. Delete the document for `Bugs Bunny`

6. Delete all the people from the DB if they have 0 hobbies


## Search (regex + string search)

1. Find all the people who have a space in their name

2. Find everyone whose Name starts with a vowel

3. Find everyone whose name starts with a consonant 

Bonus Q: Find everyone whoes name ends with a vowel too

4. Search for everyone whose name contains `Nicolas`

5. Search for everyone who has the name Nicolas - case-insensitive 


## Indexes

1. Create an index on the name. Look for it in the list of indexes


## Complex aggregations (Hobbies and Students)

1. Find everyone who is a student and has hobbies

2. Find the student with the most hobbies and the highest exam score

3. Find the students with 2 hobbies and the has the lowest homework score
