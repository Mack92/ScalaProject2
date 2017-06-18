# Liga Zagadek
The program searches WalMart and eBay for a product that is entered by a user in the selected category.
The result is a list of results for both online stores and the cheapest products with a link to the shop.
 
## Getting Started
You can run app from the sbt console with (Folder: \src\main\scala):
```
scalac GUI.scala
```
 
## Running the tests
Test are in folder src/test/scala. You can run all of them from the sbt console with:
```
> test
```
 
## Built With
 
* [ScalaFX](http://www.scalafx.org/) - UI DSL written within the Scala Language
* [SBT]http://www.scala-sbt.org/) - Open source build tool for Scala and Java projects, similar to Java's Maven or Ant.
* [ScalaTest](http://scalatest.org/) - Testing tool in the Scala ecosystem
* [Akka](http://akka.io/) -  Open-source toolkit and runtime simplifying the construction of concurrent and distributed applications on the JVM. (RestApi Connection)
## SBT file 
```
name := "AppTest1"

version := "1.0"

scalaVersion := "2.11.8"

libraryDependencies += "org.scalafx" %% "scalafx" % "8.0.102-R11"
resolvers += "Newman" at "https://dl.bintray.com/megamsys/scala"
libraryDependencies += "io.megam" %% "newman" % "1.3.11"
libraryDependencies += "org.scala-lang" % "scala-swing" % "2.10.2"
libraryDependencies ++= Seq(
  "com.typesafe.akka" %% "akka-http" % "10.0.7",
  "com.typesafe.akka" %% "akka-http-testkit" % "10.0.7" % Test
)
libraryDependencies ++= Seq(
  "com.typesafe.akka" %% "akka-stream" % "2.5.2",
  "com.typesafe.akka" %% "akka-stream-testkit" % "2.5.2" % Test
)
libraryDependencies += "io.spray" %% "spray-can" % "1.3.x"
libraryDependencies += "org.apache.commons" % "commons-math3" % "3.3"

libraryDependencies += "org.scalactic" %% "scalactic" % "3.0.1"
libraryDependencies += "org.scalatest" %% "scalatest" % "3.0.1" % "test"
```
## Authors
 Mciej Moradewicz
 
## License
 
This project is licensed under the MIT License
