#  Exemplo Python MySQL CRUD

Steps:

1. Instalar Python.

```
sudo apt-get install python3 -y
```

2. Instalar dependencias.

```
pip3 install flask_table
pip3 install pymysql
pip3 install flask-mysql
```

3. Criar tabela no banco de dados:

```
CREATE TABLE `tbl_user` (
  `user_id` bigint(20) NOT NULL AUTO_INCREMENT,
  `user_name` varchar(45) COLLATE utf8_unicode_ci DEFAULT NULL,
  `user_email` varchar(45) COLLATE utf8_unicode_ci DEFAULT NULL,
  `user_password` varchar(255) COLLATE utf8_unicode_ci DEFAULT NULL,
  PRIMARY KEY (`user_id`)
) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8 COLLATE=utf8_unicode_ci;
```

4. iniciar o servidor rodando o codigo python:
```
python main.py
```

5. Acesse a URL no browser:
```
http://localhost:5000/
```
