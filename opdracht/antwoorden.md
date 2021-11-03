# Antwoorden Eindopdracht

1. Copy paste je gemaakte SQL query hieronder

   SELECT races.name, races.date, races.year, circuits.name, circuits.location FROM races
    JOIN circuits ON races.circuitId = circuits.circuitId 
    WHERE races.year = 2018;

2. Copy paste je gemaakte SQL query hieronder

   SELECT races.name, races.date, races.year, circuits.name, circuits.location, drivers.surname, driver_standing.points FROM races
    JOIN circuits ON races.circuitId = circuits.circuitId 
    JOIN driver_standing ON races.raceId = driver_standing.raceId
    JOIN drivers ON driver_standing.driverId = drivers.driverId
    WHERE races.year = 2017 AND driver_standing.points = 10;

3. Copy paste je gemaakte SQL query hieronder
   
    SELECT drivers.forename, drivers.surname, pitstops.time FROM drivers
    JOIN pitstops ON drivers.driverId = pitstops.driverId
    WHERE pitstops.duration > 25;

4. Copy paste je gemaakte SQL query hieronder
   
    SELECT constructors.name, constructors.nationality, races.name, races.year FROM constructors
    JOIN constructor_standing ON constructors.constructorId = constructor_standing.constructorId
    JOIN races ON constructor_standing.raceId = races.raceId
    WHERE races.year = 2010 AND constructors.name = 'McLaren';

5. Copy paste je gemaakte SQL query hieronder
   
    SELECT circuits.name, circuits.country, races.name, races.year, drivers.surname FROM circuits
    JOIN races ON circuits.circuitId = races.circuitId
    JOIN driver_standing ON races.raceId = driver_standing.raceId
    JOIN drivers ON driver_standing.driverId = drivers.driverId
    WHERE races.year = 1950 AND drivers.surname LIKE 'F%'
   