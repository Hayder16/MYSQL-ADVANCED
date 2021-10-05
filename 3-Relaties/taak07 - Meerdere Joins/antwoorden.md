# Antwoorden

1. Copy paste je gemaakte SQL query hieronder

   SELECT game.name, platform.platform, genre.genre FROM `game`
    LEFT JOIN platform ON game.platform_id = platform_id
    LEFT JOIN genre ON game.genre_id = genre_id
    WHERE game.name LIKE "b%";

2. Copy paste je gemaakte SQL query hieronder

    SELECT game.name, platform.platform, publisher.publisher, game.year FROM game 
    LEFT JOIN platform ON game.platform_id = platform_id 
    LEFT JOIN publisher ON game.publisher_id = publisher_id 
    WHERE year = '2013'

3. Copy paste je gemaakte SQL query hieronder

    SELECT game.name, genre.genre, publisher.publisher, game.year, game.global_sales FROM game
    LEFT JOIN genre ON game.genre_id = genre_id
    LEFT JOIN publisher ON game.publisher_id = publisher_id
    WHERE genre_id = 5 AND year > '2000'

4. Copy paste je gemaakte SQL query hieronder

    SELECT platform.platform, game.year, genre.genre, publisher.publisher, game.jp_sales FROM game
    LEFT JOIN platform ON game.platform_id = platform_id
    LEFT JOIN genre ON game.genre_id = genre_id
    LEFT JOIN publisher ON game.publisher_id = publisher_id
    WHERE game.name LIKE 'mario%';

5. Copy paste je gemaakte SQL query hieronder
   
    SELECT game.name, genre.genre, publisher.publisher, game.year FROM game 
    LEFT JOIN genre ON game.genre_id = genre_id 
    LEFT JOIN publisher ON game.publisher_id = publisher_id 
    WHERE platform_id = 15