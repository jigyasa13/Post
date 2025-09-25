# Student Information System (Java + MySQL + JDBC)

This is a simple **GitHub-ready** Java (Maven) Student Information System project that demonstrates:
- Student personal records
- Academic records (enrollment, marks, grades)
- Attendance tracking
- JDBC connectivity to MySQL
- Sample queries: grade report, GPA, attendance percentage

## How to run (quick)
1. Install MySQL and create a database using `sql/init.sql`.
   - Example: `mysql -u root -p < sql/init.sql`
2. Update DB credentials in `src/main/java/com/sis/util/DBConnection.java`.
3. Build with Maven:
   ```bash
   mvn package
   ```
4. Run:
   ```bash
   mvn exec:java -Dexec.mainClass="com.sis.Main"
   ```
   or run the compiled jar/class in your IDE.

## Files included
- `pom.xml` — Maven configuration (includes MySQL connector).
- `src/main/java/com/sis/...` — Source code (DBConnection, models, DAOs, Main).
- `sql/init.sql` — Schema and sample data (creates tables + trigger).
- `.gitignore`

## Note
- Change DB username/password in `DBConnection.java` before running.
- This is a minimal demo suitable for local testing and for uploading to GitHub.
