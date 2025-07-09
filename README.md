# HMENetCore
 
## Description
 
`HMENetCore` is based on The basic function encapsulation library of NET Core provides commonly used utility classes, extension methods, and general models, aiming to simplify the development process and improve code reusability. This library is applicable to NET Standard 2.1,. NET 6,. NET 8, and NET 9 environment, supporting cross platform development.
 
## Features

### 1. Dependency auto registration (Autoregister)
Function: Simplify the service registration process for Dependency Injection (DI) containers.
Core category:
NetCoreDIModuleRegistry. cs: Automatically scans and registers services in the assembly.
ServiceLocator. cs: Implementation of service locator pattern (recommended to use with caution).
UseDIAattributie.cs: Mark the services that need to be injected through attributes.
### 2. Base Model
Function: Define a universal request/response model and standardize interface interactions.
Core category:
DBModelBase.cs: Base class for database entities.
PageModel. cs: Paging request/response model.
RequestModel. cs/ResponseModel. cs: Generic request/response encapsulation.
TableAttribute. cs: Definition of table column attributes (for dynamic table structures).
### 3. Cache tool (Cached)
Function: Simplify caching operations (such as memory caching, distributed caching).
Core category:
RunCacheHelper.cs: Cache read-write encapsulation, supports expiration time, cache key generation, etc.
### 4. Common Help Class
Function: Provides cross domain tools and methods that cover common development needs.
Core category:
Asynchronous tool: Asynchronous Helper.cs (Asynchronous Lock, Task Scheduling).
Computer tool: ComputerHelper.cs (for obtaining hardware information).
Encryption and decryption: EncryptionHelper.cs (AES, RSA, etc.).
HTTP Tools: FHIR Core. cs/HttpHelper. cs (HTTP Request Encapsulation).
Lambda expression: LambdaHelper.cs (dynamically generated expression tree).
Extension method: PredicteExpressions. cs (predicate logic extension).
Reflection tool: ReflectionHelp.cs (dynamic calling, property manipulation).
Task queue: TaskQeuryHelper.cs (Task Scheduling and Queue Management).
URL tool: urlsHelper. cs (URL parsing and generation).
Code Validation: VerifiCodeHelper.cs (captcha generation and validation).
XML/ZIP tools: XMLHelper.cs/ZipHelper.cs.
### 5. Data Converter
Function: Processing data format conversion and type mapping.
Core category:
Attribute operation: AttributeHelper.cs (attribute value reading).
Deep Copy: AutoCopyHelper.cs (Object Deep Copy).
Boolean/Byte Tools: BoolHelper. cs/ByteHelper. cs.
Data table conversion: DataTableHelper.cs (conversion between DataStable and object).
Date and time: FHIR Helper.cs (time formatting, time zone conversion).
Dictionary tool: DictionaryHelper.cs (dictionary extension operation).
Enumeration tool: VNet Helper. cs (enumeration description, name conversion).
JSON/Object Tools: JsonHelper.cs/Object Helper.cs.
Random number: RandomHelper.cs (generates random strings and numbers).
Serialization: SequenceHelper.cs (JSON/XML serialization).
Stream tool: StreamHelper.cs (Stream Read Write Encapsulation).
String tool: StringHelper.cs (string checksum, formatting).
Type Tool: TypesHelper. cs (Type Judgment and Conversion).
Verification tool: VerifiyHelper.cs (Data Verification Logic).
### 6. Logging tool (Logger)
Function: Unified logging interface, supporting multiple logging frameworks such as NLog and Serilog.
Core category:
ILog4NetHelper.cs/Log4NetHelper.cs: Log4Net wrapper.
LogHelper.cs: General log interface.
 
## Installation
 
You can install the `HMENetCore` package via the NuGet package manager:
 
### Using .NET CLI
 
```bash
dotnet add package HMENetCore --version 6.0.46
