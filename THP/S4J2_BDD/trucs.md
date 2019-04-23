##Créer l'album de ton artiste favori en base, en renseignant correctement les trois tables albums, artists et tracks

INSERT INTO artists (Name) VALUES ('Rosalía'); INSERT INTO albums (Title, ArtistId) VALUES ('El mal querer', 276); INSERT INTO tracks (Name, AlbumId, MediaTypeId, GenreId, Composer, Milliseconds, UnitPrice) VALUES ('Malamente - Cap 1: Augurio', 348, 1, 17, 'Rosalía Vila Tobella', 120000, 0.99), ('Que no salga la luna - Cap 2: Boda', 348, 1, 17, 'Rosalía Vila Tobella', 120000, 0.99), ('Pienso en tu mirá - Cap 3: Celos', 348, 1, 17, 'Rosalía Vila Tobella', 120000, 0.99), ('De aquí no sales - Cap 4: Disputa', 348, 1, 17, 'Rosalía Vila Tobella', 120000, 0.99), ('Reniego - Cap 5: Lamento', 348, 1, 17, 'Rosalía Vila Tobella', 120000, 0.99), ('Preso - Cap 6: Clausura', 348, 1, 17, 'Rosalía Vila Tobella', 120000, 0.99), ('Bagdad - Cap 7: Liturgia', 348, 1, 17, 'Rosalía Vila Tobella', 120000, 0.99), ('Di mi nombre - Cap 8: Éxtasis', 348, 1, 17, 'Rosalía Vila Tobella', 120000, 0.99), ('Nana - Cap 9: Concepción', 348, 1, 17, 'Rosalía Vila Tobella', 120000, 0.99), ('Nana - Cap 9: Concepción', 348, 1, 17, 'Rosalía Vila Tobella', 120000, 0.99), ('A ningún hombre - Cap 11: Poder', 348, 1, 17, 'Rosalía Vila Tobella', 120000, 0.99);




CREATE TABLE courses (
id INTEGER PRIMARY KEY AUTOINCREMENT, title TEXT,
description TEXT
);

CREATE TABLE lessons (
id INTEGER PRIMARY KEY AUTOINCREMENT, title TEXT,
body TEXT, course_id INTEGER,
FOREIGN KEY(course_id) REFERENCES courses(id)
);

INSERT INTO courses (title, description) VALUES ('how to code', 'subscribe to openclassrooms');

INSERT INTO lessons (title, body, course_id) VALUES ('the wheel','keep rollin, rollin, rollin', 2);