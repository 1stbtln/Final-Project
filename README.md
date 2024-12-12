System Requirements
•	Java Development Kit (JDK): Version 17 or later
•	JavaFX SDK: Tested with JavaFX 23.0.1 (https://gluonhq.com/products/javafx/)
o	Extract the SDK to a directory like (C:\javafx-sdk-23.0.1)
•	JSON Library: json-20210307.jar (https://repo1.maven.org/maven2/org/json/json/20210307/)

Setup Instructions
1.	Install JavaFX
1. Download the JavaFX SDK from (https://gluonhq.com/products/javafx/)
2. Extract the SDK to a directory like (C:\javafx-sdk-23.0.1) 
2.	Ensure that the config.txt is properly formatted with the following content.
API_KEY=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJqdGkiOiI0ZjQwOTgxMC0yZTRjLTAxM2MtMWFjMi0wNjAzNzFjMDFlZTQiLCJpc3MiOiJnYW1lbG9ja2VyIiwiaWF0IjoxNjkzOTQwMzg4LCJwdWIiOiJibHVlaG9sZSIsInRpdGxlIjoicHViZyIsImFwcCI6ImtpbGwtcmVjb3JkLXYxIn0.UmtcORtJXnGlxT5CBIcz24BtM338rQzlYU3oWJ81Nc8
BASE_URL=https://api.pubg.com/shards/steam/players/

Compilation Instructions via the command line
1.	Open a terminal
2.	Navigate to the source directory
3.	Compile all .java files
javac --module-path "C:\javafx-sdk-23.0.1\lib" --add-modules javafx.controls,javafx.fxml -cp ../Compiled/lib/json-20210307.jar *.java

Running the Program via the command line
1.	Navigate to the compiled folder
2.	Run the application
java --module-path "C:\javafx-sdk-23.0.1\lib" --add-modules javafx.controls,javafx.fxml -cp ".;lib/json-20210307.jar" PlayerStatsApp

Testing the Application
1.	Enter a valid player name (case sensitive) in the input field e.g. “1stbtln”
2.	Click Fetch Stats to retrieve and display player statistics.
