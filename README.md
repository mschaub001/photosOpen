# photosOpen

Photos is a JSF/PrimeFaces JEE 7 demo web application. It demonstrates use of several PrimeFaces components mainly the highly functioning p:dataTable. Also included are p:fileUpload and p:ring used to upload and preview images into the application. 

User Management is also supported. This includes registration, authetication, authorization, monitoring and profiles. Passwords are hashed, salted and iterated. Within the database, they end up looking something like this:  500000:IvRY2w5McPoEvoMMBH0BeUB9XPoUqeyYTI5Frq9/jeG/UgGp9DwZHe0si5j5bOAIea68twHVbLMfp39hhVSPC+qFwGtTDIY5HJn/Y6uotfAVjQR59xE6+FIuOFx69xO9jnohQgoifYAoHNWSxMAxl6GAY/Ul3K+5rNboPJ/z/zo=:GlN+z6/IW5d4NYziSiM+XQ==

See https://github.com/heather92115/photosOpen/blob/master/src/main/java/com/tf/photos/util/KryptoUtil.java for details of password cryptography.

MongoDB is used to store all user information and images with corresponding meta data.

### Run

Try out this web application here: https://www.totalfruition.com/photoApp/home/overview.jsf

### Build

Maven 3 is required.

Run `mvn install` to create the war file. This will also run the unit tests.

### Running Unit Tests

Run `mvn test`

### Todo 

Unit and integration tests are lacking.

### Running the application locally

This application requires MongoDB and Maven 3.

Once access to a MongoDB database has been configured, update this source file with the proper username, password, database name, ip address and port:

https://github.com/heather92115/photosOpen/blob/master/src/main/java/com/tf/photos/service/MongoApplicationContextConfig.java



