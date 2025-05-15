# Day 29 of SQL + Data Journey 🚄

Today, I learned how to create my own database schema from scratch using SQLite.

### 🧠 What I Practiced:
- Creating tables with `CREATE TABLE`
- Assigning a `PRIMARY KEY` to uniquely identify each row
- Connecting tables using `FOREIGN KEY` constraints

### 🏗️ Tables I Designed:
```sql
CREATE TABLE "riders" (
    "id" INTEGER,
    "name" TEXT,
    PRIMARY KEY ("id")
);

CREATE TABLE "stations" (
    "id" INTEGER,
    "name" TEXT,
    "line" TEXT,
    PRIMARY KEY ("id")
);

CREATE TABLE "visits" (
    "rider_id" INTEGER,
    "station_id" INTEGER,
    FOREIGN KEY ("rider_id") REFERENCES "riders" ("id"),
    FOREIGN KEY ("station_id") REFERENCES "stations" ("id")
);


🧩 Lesson Learned:
Even if I hit errors like syntax mistakes or conflicting table names, I'm learning how to troubleshoot, drop and rebuild tables, and fine-tune foreign key references.

📍Progress like this builds the foundation for more advanced relational database projects. Tomorrow, I’ll focus on inserting data and querying across my new schema.

#100DaysOfSQL #DataEngineering #SQLLearning #MenInTech #DatabaseDesign
