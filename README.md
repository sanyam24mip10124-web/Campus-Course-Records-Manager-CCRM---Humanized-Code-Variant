# Campus Course & Records Manager (CCRM)

Yo, this is my Java project for class! It’s a console app called CCRM to manage students, courses, grades, and backups for a campus. Built with Java SE, it uses OOP, NIO.2, streams, and more. Code’s organized into packages and runs locally.

## Project Overview

The app lets you:
- Add/update/list/deactivate students and courses.
- Enroll/unenroll students with credit limits.
- Record grades, compute GPA, and print transcripts.
- Import/export CSV data and create timestamped backups.

It shows off OOP (encapsulation, inheritance, etc.), exception handling, lambdas, enums, and design patterns (Singleton, Builder). Check the code for the full scoop!

## How to Run

### Requirements
- JDK 21 (used for this project).
- Eclipse IDE (optional but handy).

### Command Line
1. Clone: `git clone <repo-url>`
2. Navigate: `cd src`
3. Compile: `javac edu/ccrm/cli/Main.java`
4. Run: `java edu.ccrm.cli.Main`

### Eclipse
- Import as Java project.
- Run `edu.ccrm.cli.Main`.

Menu pops up on start—use numbers to navigate.

## Evolution of Java

- 1995: Java 1.0 released.
- 2004: Java 5 adds generics, enums.
- 2014: Java 8 brings lambdas, streams.
- 2017: Java 9 introduces modules.

## Java Editions Comparison

- **Java ME**: For small devices (e.g., old phones), limited APIs.
- **Java SE**: Core for desktop apps (used here), includes NIO, streams.
- **Java EE**: For enterprise apps (e.g., web servers), adds servlets.

## Java Architecture: JDK, JRE, JVM

- **JVM**: Runs bytecode, handles memory.
- **JRE**: JVM + core libraries to run apps.
- **JDK**: JRE + tools (javac) to write code.
- Interaction: Write .java, compile to .class, JVM runs it.

## Installing Java on Windows

1. Download JDK 21 from https://adoptium.net/.
2. Run .msi installer.
3. Add to PATH: `C:\Program Files\Eclipse Adoptium\jdk-21\bin`.
4. Verify: `java -version`.

![JDK Verification](screenshots/jdk-verification.png)

## Eclipse Setup

1. Download from https://www.eclipse.org/downloads/.
2. Select "Java Developers" edition.
3. New Java Project: "CCRM", run `edu.ccrm.cli.Main`.

![Eclipse Setup](screenshots/eclipse-setup.png)

## Syllabus Mapping

| Topic                  | Location                     |
|------------------------|------------------------------|
| Primitive variables    | `edu.ccrm.domain.Student`    |
| Decision structures    | `edu.ccrm.cli.Menu`          |
| Loops                  | `edu.ccrm.service.StudentService` |
| Encapsulation          | `edu.ccrm.domain.Student`    |
| Inheritance            | `edu.ccrm.domain.Person`     |
| Singleton              | `edu.ccrm.config.AppConfig`  |
| Exceptions             | Custom exceptions in services |

## Enabling Assertions

Use `java -ea edu.ccrm.cli.Main` for assertions (e.g., non-null checks).

## Usage

### Sample Commands
Menu options: 1. Manage Students, 2. Courses, etc.  
Add student: Select 1, then 1, enter "123, REG001, John Doe, john@example.com".

### Data Files
See `test-data/students.csv` for import samples.

## Screenshots
- JDK: screenshots/jdk-verification.png
- Eclipse: screenshots/eclipse-setup.png
- Menu: screenshots/program-menu.png
- Backups: screenshots/backups-folder.png

## Acknowledgements
All my work. Referenced Oracle Java docs and class notes—no LLMs!
