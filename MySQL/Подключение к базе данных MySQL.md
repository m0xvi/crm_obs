`const mysql = require('mysql2/promise');`
`require('dotenv').config();`

`const db = mysql.createPool({` 
	createPool используется для многопоточности и возможности нескольких запросов одновременно
  `host: process.env.DB_HOST,`
  `user: process.env.DB_USER,`
  `password: process.env.DB_PASSWORD,`
  `database: process.env.DB_NAME,`
`});`

`module.exports = db;`
