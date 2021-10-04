# Antwoorden

1. Copy paste je gemaakte SQL query hieronder
   SELECT * FROM `game` JOIN platform ON platform_id = platform
2. Copy paste je gemaakte SQL query hieronder
   SELECT * FROM `game` JOIN platform ON platform_id = platform WHERE game.id <= 10 
3. Copy paste je gemaakte SQL query hieronder
   SELECT name, platform FROM `game` JOIN platform ON platform_id WHERE game.name = "Call of Duty: Advanced Warfare"
4. Copy paste je gemaakte SQL query hieronder
   SELECT platform, name FROM `game` JOIN platform ON platform_id WHERE name LIKE "FIFA"
5. Copy paste je gemaakte SQL query hieronder
   SELECT name, platform FROM `game` JOIN platform ON platform_id WHERE name = 'Borderlands' OR 'Borderlands 2'