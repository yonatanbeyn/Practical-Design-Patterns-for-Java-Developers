# Practical-Design-Patterns-for-Java-Developers
Practical Design Patterns for Java Developers, published by Packt

#### how to compile a code
```bash
$ javac --release 17 --enable-preview -g -cp out -sourcepath java -d out ./<CHAPTER_NUMBER>/<CHAPTER_IDENTIFIER>/*.java

# example 
$ javac --release 17 --enable-preview -g -cp out -sourcepath java -d out ./Chapter01/apie/*.java

# create module jar
$ jar --create --file module-example.jar  -C out .
```

### how to execute example
```bash
$ java --enable-preview -cp out/<CHAPTER_IDENTIFIER> <EXAMPLE_NUMBER_MAIN>

# example
$ java --enable-preview -cp out/apie Example1_2Main

# run module path 
$ java --module-path ./Chapter02/module-example.jar --module module.example/example.ExampleMain
```

## Chapter 1 - examples
The examples are 
Runnable examples:
- Example1_2Main
- Example1_6Main
- Example1_7Main
- Example1_8Main
- Example1_9Main

## Chapter 2 - creatinoal pattern examples

## Chapter 3 - structural examples 
```bash
# Factory Method: creating instances 
$ javac --release 17 --enable-preview -g -cp out/Chapter03/fm -sourcepath java -d out/Chapter03/fm ./Chapter03/factory_method/*.java
$ java --enable-preview -cp out/Chapter03/fm FactoryMethodMain
$ java --enable-preview -cp out/Chapter03/fm -XX:StartFlightRecording=filename=FactoryMethod.jfr,dumponexit-true,settings=profile FactoryMethodMain

# Abstract Factory: instancise proper factory to create desired instances
$ javac --release 17 --enable-preview -g -cp out/Chapter03/af -sourcepath java -d out/Chapter03/af ./Chapter03/abstract_factory/*.java
$ java --enable-preview -cp out/Chapter03/af AbstractFactoryMain

# Builder
$ javac --release 17 --enable-preview -g -cp out/Chapter03/builder -sourcepath java -d out/Chapter03/builder ./Chapter03/builder/*.java
$ java --enable-preview -cp out/Chapter03/builder BuilderMain

# Prototype
$ javac --release 17 --enable-preview -g -cp out/Chapter03/prototype -sourcepath java -d out/Chapter03/prototype ./Chapter03/prototype/*.java
$ java --enable-preview -cp out/Chapter03/prototype PrototypeMain

# Singleton 
$ javac --release 17 --enable-preview -g -cp out/Chapter03/singleton -sourcepath java -d out/Chapter03/singleton ./Chapter03/singleton/*.java
$ java --enable-preview -cp out/Chapter03/singleton SingletonMain


# Object Pool
$ javac --release 17 --enable-preview -g -cp out/Chapter03/object_pool -sourcepath java -d out/Chapter03/object_pool ./Chapter03/object_pool/*.java
$ java --enable-preview -cp out/Chapter03/object_pool ObjectPoolMain

# Lazy Initialization
$ javac --release 17 --enable-preview -g -cp out/Chapter03/lazy_initialization -sourcepath java -d out/Chapter03/lazy_initialization ./Chapter03/lazy_initialization/*.java
$ java --enable-preview -cp out/Chapter03/lazy_initialization LazyInitializationMain

# Dependency Injection
$ javac --release 17 --enable-preview -g -cp out/Chapter03/dependency_injection -sourcepath java -d out/Chapter03/dependency_injection ./Chapter03/dependency_injection/*.java
$ java --enable-preview -cp out/Chapter03/dependency_injection DependencyInjectionMain
```

```bash 
# Starting the JavaFlightRecorder for the patterns
# Recordings are done on Java 17
$ java -XX:StartFlightRecording=filename=<PATTERN_NAME_MAIN>.jfr,dumponexit-true,settings=profile <MAIN_CLASS>
```

## Chapter 4 - Behavioral pattern

```bash
# Adapter 
$ javac --release 17 --enable-preview -g -cp out/Chapter04/adapter -sourcepath java -d out/Chapter04/adapter ./Chapter04/adapter/*.java
$ java --enable-preview -cp out/Chapter04/adapter AdapterMain

# Bridge
$ javac --release 17 --enable-preview -g -cp out/Chapter04/bridge -sourcepath java -d out/Chapter04/bridge ./Chapter04/bridge/*.java
$ java --enable-preview -cp out/Chapter04/bridge BridgeMain

# Composite
$ javac --release 17 --enable-preview -g -cp out/Chapter04/composite -sourcepath java -d out/Chapter04/composite ./Chapter04/composite/*.java
$ java --enable-preview -cp out/Chapter04/composite CompositeMain

# Decorator
$ javac --release 17 --enable-preview -g -cp out/Chapter04/decorator -sourcepath java -d out/Chapter04/decorator ./Chapter04/decorator/*.java
$ java --enable-preview -cp out/Chapter04/decorator DecoratorMain

# Facade
$ javac --release 17 --enable-preview -g -cp out/Chapter04/facade -sourcepath java -d out/Chapter04/facade ./Chapter04/facade/*.java
$ java --enable-preview -cp out/Chapter04/facade FacadeMain

# Filter
$ javac --release 17 --enable-preview -g -cp out/Chapter04/filter -sourcepath java -d out/Chapter04/filter ./Chapter04/filter/*.java
$ java --enable-preview -cp out/Chapter04/filter FilterMain

# Flyweight
$ javac --release 17 --enable-preview -g -cp out/Chapter04/flyweight -sourcepath java -d out/Chapter04/flyweight ./Chapter04/flyweight/*.java
$ java --enable-preview -cp out/Chapter04/flyweight FlyweightMain

# Front controller
$ javac --release 17 --enable-preview -g -cp out/Chapter04/front_controller -sourcepath java -d out/Chapter04/front_controller ./Chapter04/front_controller/*.java
$ java --enable-preview -cp out/Chapter04/front_controller FrontControllerMain

# Marker
$ javac --release 17 --enable-preview -g -cp out/Chapter04/marker -sourcepath java -d out/Chapter04/marker ./Chapter04/marker/*.java
$ java --enable-preview -cp out/Chapter04/marker MarkerMain

# Module
$ javac --release 17 --enable-preview -g -cp out/Chapter04/module -sourcepath java -d out/Chapter04/module ./Chapter04/module/*.java
$ java --enable-preview -cp out/Chapter04/module ModuleMain

# Proxy
$ javac --release 17 --enable-preview -g -cp out/Chapter04/proxy -sourcepath java -d out/Chapter04/proxy ./Chapter04/proxy/*.java
$ java --enable-preview -cp out/Chapter04/proxy ProxyMain

# Twin
$ javac --release 17 --enable-preview -g -cp out/Chapter04/twin -sourcepath java -d out/Chapter04/twin ./Chapter04/twin/*.java
$ java --enable-preview -cp out/Chapter04/twin TwinMain
```