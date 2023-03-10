# Interview_Questions_Answers

## Maven Project
+ Maven has the ability to download dependencies automatically based on the dependencies block you put in respective maven project’s pom.xml file.Maven is a powerful project management tool that is based on POM (project object model). It is used for projects build, dependency and documentation.POM is an acronym for Project Object Model. It contains information about project and configuration of the project such as dependencies, build directory, source directory, test source directory, plugins, goal, etc. Maven reads pom.xml and then executes goal.
+ Open Source Build Tool developed by the Apache Group
+ Take cares of the Builds, Dependencies, Reports, Distribution, Releases & Mailing List
+ Helps in getting the right JAR files for each project from (mvnrespository.com)


## Dependency Injection
Dependency injection (DI) is the concept in which objects get other required objects from outside.DI can be implemented in any programming language. The general concept behind dependency injection is called Inversion of Control.
A Java class has a dependency on another class, if it uses an instance of this class. We call this a class dependency. For example, a class which accesses a logger service has a dependency on this service class.

Ideally Java classes should be as independent as possible from other Java classes. This increases the possibility of reusing these classes and to be able to test them independently from other classes.

There are three different types of dependency injections:

### Constructor injection
Constructor injection is shown in the first code example. The dependent class receives the object it requires as a parameter of the constructor.

### Setter injection
The dependent class has a public setter method through which the dependency is injected. An example is given in the code below:

<pre><code>
class Building {
    private Room room;

    public setRoom(Room room){
        this.room = room;
    }
}
</pre></code>

### Interface injection
An interface provides an injector method that is responsible for injecting the dependency to any class that may require it. The client class has to implement the interface and override the injector method. For example:

<pre><code>
public interface Injector {
  public void injectDependency(Dependency object);
}

public class Client implements Injector {
  private Dependency dependentObject;

  @Override
  public void injectDependency(Dependency object){
    this.dependentObject = object;
    }
</pre></code>

### Advantages of dependency injection 

+ Makes testing easier by enabling the use of mock objects or stubs
+ Reduces coupling between client and dependency classes
+ Reduces boilerplate code since the initialization of all dependencies is done once by the injector
+ The code is easier to maintain and reuse

Detailed: (https://www.youtube.com/watch?v=Eqi-hYX50MI)

### Sort Of Array (or) ArrayList In Ascending Order Java

<pre><code>
List<Integer> list = Arrays.asList(10, 4, 2, 6, 5, 8);
Collections.sort(list);
System.out.println(list);
</pre></code>

(OR)

<pre><code>
list.stream().sorted().collect(Collectors.toList());
</pre></code>

### OSLC API
The Open Services for Lifecycle Collaboration Change Management (OSLC-CM) specification defines a lightweight, RESTful API for software change management systems. It acts as a common language for Application Lifecycle Management (ALM) tools.

#### OSLC API
Interfaces can be REST based interfaces.
OSLC when incepted was based on using the REST paradigm.

https://open-services.net/

#### REST API
Rest is a number of rules and patradigms that are used. There can be many interfaces that are conform. What these interfaces  provide can be totally different. They can have rules on top of what REST requests and be specialised on some domain.

