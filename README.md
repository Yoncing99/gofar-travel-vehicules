## Exporter une base de donnée mysql
```
mysqldump -u username -p database_name > data-dump.sql
```

## Importer une base de donnée mysql 

Se connecter :
```
mysql -u root -p
```
Créer une nouvelle base donnée :
```
CREATE DATABASE new_database;
```
Quitter mysql en faisant ```CTRL+D``` puis importer la base de donnée :
```
mysql -u username -p new_database < data-dump.sql

```

## Insertions:

### Vehicles
```
INSERT INTO `gofar`.`Vehicle` (`id`, `vin`, `name`, `model`, `year`, `manufacturer_name`, `manufacturer_amount_price`, `state`, `price`) VALUES ('2', '4242154', 'BMW', 'M3', 0, 'BMW', '44444', 'NEuve', '4444');
```

### Persons
```
INSERT INTO `gofar`.`Person` (`id`, `name`, `address`, `phone_number`, `isCustomer`) VALUES ('3', 'Philipp', '3 ch dse', '213545122', '0');
```

### Saler

```
INSERT INTO `gofar`.`Saler` (`id`, `name`, `experienced`, `phone_number`, `address`) VALUES ('2', 'Morris', '1 ', '221221', '1 chzguez');
```
