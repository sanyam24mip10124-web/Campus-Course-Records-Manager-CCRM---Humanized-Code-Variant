# Campus Course & Records Manager (CCRM)

##  Project Overview

The **Campus Course & Records Manager (CCRM)** is a **console-based Java
SE application** to help institutes manage:\
- **Students** (add, update, enroll/unenroll in courses, view
transcript)\
- **Courses** (create, list, update, search/filter by
department/instructor/semester)\
- **Enrollment & Grading** (enroll students, record marks, compute GPA,
generate transcripts)\
- **File Utilities** (import/export CSV data, backup archives, recursive
utilities)

It demonstrates **OOP principles**, modern **Java SE APIs (NIO.2,
Streams, Date/Time)**, and design patterns (**Singleton, Builder**).

------------------------------------------------------------------------

##  How to Run

1.  Install **JDK 17+**.\

2.  Clone this repository:

    ``` bash
    git clone <repo-link>
    cd CampusCourseRecordsManager
    ```

3.  Compile and run:

    ``` bash
    javac -d bin src/**/*.java
    java -cp bin edu.ccrm.cli.Main
    ```

4.  Alternatively, import into **Eclipse IDE** → *New Java Project* →
    *Run as Java Application*.

------------------------------------------------------------------------

##  Evolution of Java (Quick Timeline)

-   **1995** -- Java 1.0 released (Sun Microsystems).\
-   **2004** -- Java 5: Generics, Enums, Annotations.\
-   **2011** -- Java 7: NIO.2, try-with-resources.\
-   **2014** -- Java 8: Lambdas, Streams, Date/Time API.\
-   **2017+** -- Java 9--17: Modules, var, records, pattern matching,
    modern APIs.

------------------------------------------------------------------------

##  Java Editions Comparison

  -----------------------------------------------------------------------
  Edition              Purpose              Example Use
  -------------------- -------------------- -----------------------------
  **Java ME**          Mobile/embedded      Feature phones, IoT
                       devices              

  **Java SE**          Standard desktop     This project (console app)
                       apps, core libraries 

  **Java EE (Jakarta   Enterprise, web,     Banking, e-commerce systems
  EE)**                distributed apps     
  -----------------------------------------------------------------------

------------------------------------------------------------------------
## 🏗️ Java Architecture (JDK vs JRE vs JVM)

-   **JDK (Java Development Kit)** -- tools + compiler + JRE.\
-   **JRE (Java Runtime Environment)** -- runtime libraries + JVM.\
-   **JVM (Java Virtual Machine)** -- executes bytecode on any platform.

Flow: **Source Code → Compiler → Bytecode → JVM → Machine Execution**.

------------------------------------------------------------------------

##  Installation (Windows)

1.  Download JDK from Oracle/OpenJDK.\

2.  Install & set `JAVA_HOME` in Environment Variables.\

3.  Verify:

    ``` bash
    java -version
    ```

4.  **Eclipse IDE**:

    -   File → New → Java Project → Add source folders (`src`) → Run
        Main class.

*(Screenshots included in `/screenshots` folder as per submission
guidelines)*

------------------------------------------------------------------------

##  Mapping: Syllabus Topic → Project Files

  -----------------------------------------------------------------------
  Topic           Example Implementation
  --------------- -------------------------------------------------------
  Encapsulation   `Student` class with private fields + getters/setters

  Inheritance     `Person` (abstract) → `Student`, `Instructor`

  Abstraction     `Person` abstract methods

  Polymorphism    `TranscriptService` interface with multiple impls

  Interfaces      `Persistable`, `Searchable<T>`

  Lambdas &       Filtering courses by instructor/semester
  Streams         

  Enums           `Semester`, `Grade`

  Singleton       `AppConfig`

  Builder         `Course.Builder`

  Exception       `DuplicateEnrollmentException`,
  Handling        `MaxCreditLimitExceededException`

  File I/O        `ImportExportService`, `BackupService`
  (NIO.2)         

  Recursion       Backup size computation

  Assertions      Non-null IDs, credit limits
  -----------------------------------------------------------------------

------------------------------------------------------------------------

##  Usage (Sample Commands)

-   **Add Student** → Enter details via CLI menu.\
-   **Enroll Student** → Select student + course code.\
-   **Record Grades** → Enter marks → GPA auto-computed.\
-   **Export Data** → Creates CSV files in `/exports`.\
-   **Backup** → Copies exports to `/backup/yyyyMMdd_HHmmss`.

------------------------------------------------------------------------

##  Notes

-   Enable assertions when running:

    ``` bash
    java -ea -cp bin edu.ccrm.cli.Main
    ```

-   Errors vs Exceptions explained in comments & README.\

-   Includes both **checked & unchecked exceptions**.

------------------------------------------------------------------------

##  Deliverables

-   **Source Code** (with packages: `edu.ccrm.domain`,
    `edu.ccrm.service`, `edu.ccrm.io`, etc.)\
-   **README.md** (this file)\
-   **Screenshots folder** (installation, Eclipse setup, program run,
    exports/backups)\
-   **Optional demo video link**\
-   **Sample test-data CSVs**

------------------------------------------------------------------------

##  Acknowledgements

This project was developed as part of the **Programming in Java**
coursework. References: *Java Docs, Oracle Tutorials*.
