# Smart Campus Parking & Traffic Intelligence System — AWT Edition

100% Java AWT + JDBC + MySQL. **No Swing is used anywhere.**

## Features
1. Smart parking slot recommendation
2. Interactive graphical parking map using AWT Canvas/Graphics
3. Traffic congestion meter and traffic records
4. Historical occupancy analytics / prediction estimate
5. Intelligent dashboard with alerts and analytics
6. User and vehicle CRUD
7. Reservations with conflict checking
8. Vehicle entry/exit and automatic fee calculation
9. Digital parking passes
10. Violations and payments
11. Reports and database-backed analytics

## Requirements
- JDK 17+
- MySQL 8+
- MySQL Workbench
- MySQL Connector/J 8.x JAR

## 1. Database
Open `sql/smart_campus_parking.sql` in MySQL Workbench and execute it.

## 2. Configure JDBC
Edit `src/smartcampus/DB.java` and set your MySQL username/password.

## 3. Compile (Windows)
`javac -cp "mysql-connector-j-8.x.x.jar" -d out src/smartcampus/*.java`

## 4. Run (Windows)
`java -cp "out;mysql-connector-j-8.x.x.jar" smartcampus.Main`

Linux/macOS: replace `;` with `:`.

## Login
Username: `admin`
Password: `admin123`

## AWT-only verification
The source imports `java.awt.*` and `java.awt.event.*` plus JDBC. It contains no `javax.swing` imports or Swing widgets.
