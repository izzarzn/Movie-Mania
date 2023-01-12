---- Procedures--
CREATE DEFINER=`root`@`localhost` PROCEDURE `getmovies_genre` (IN `genre` VARCHAR(20))   BEGIN    select movies.id, movies.title, movies.actor, movies.producer, movies.director   from movies JOIN genre ON movies.genre=genre.id WHERE genre.title = genre;    end;
