# QuCens-SSE

## **Datenbanken einrichten**

MySQL-Datenbank:

```sql
CREATE TABLE IF NOT EXISTS projects (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(255) NOT NULL,
    apikey VARCHAR(255) NOT NULL UNIQUE,
    qucenskey VARCHAR(255) NOT NULL,
    name VARCHAR(255) NOT NULL,
    createstamp DATETIME DEFAULT CURRENT_TIMESTAMP
);
```

SQLite-Datenbank:

```sql
CREATE TABLE "licenses" (
	"id"	INTEGER,
	"license_key"	TEXT NOT NULL UNIQUE,
	"backup_code"	TEXT NOT NULL,
	"is_used"	BOOLEAN DEFAULT FALSE,
        "is_disabled".  INTEGER DEFAULT 0;
	PRIMARY KEY("id" AUTOINCREMENT)
);
```

Made with ♥ by @amosjulian
