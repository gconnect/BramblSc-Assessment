# BramblSc-Assessment
This documentation contains suggestions and improvements to the existing BramblSc documentation.


## 1.1 README.md Enhancements
### Problem:
The current [README](https://github.com/Topl/BramblSc) is minimal and lacks detailed information on setup, usage, and project structure. This can be challenging for developers, especially newcomers, to navigate the repository.

### Suggested Improvements:
#### Introduction Section:
The introduction section should briefly summarize what Brambl SDK does, its primary use cases, and who can benefit from it.

#### Example:

The Brambl SDK is designed to simplify interaction with Topl’s blockchain, providing cryptographic utilities and tools to build decentralized applications. This SDK powers use cases like asset issuance, transaction monitoring, and key management.

#### Setup Installation Guide:
Quick setup installation steps should be added.

- Required tools e.g., Java, Scala, SBT
- OS-specific setup instructions

#### Note
Java/Scala version ... will be required.


#### Example:
```bash
# Clone the repo
git clone https://github.com/topl/brambl-sc.git
cd brambl-sc

# Install dependencies
sbt update

# Run tests
sbt test
```

## Overview of Each Artifacts

### brambl-sdks
The brambl-sdks are a collection of software development kits that allow developers to interact with the Network. There are currently SDKs for the following languages:

- [Scala (BramblSc)](Link to the sdk)
- [Dart (BramblDart)](Link to the sdk)
  
### crypto
The crypto module provides cryptographic functions like signature verification. Here is a detail guide to learn more about the [Crypto]() artifact.

### service-kit
The service kit is an implementation of several APIs defined in the brambl-sdk. Here is a reference documentation to learn more about [service-kit](https://topl.github.io/BramblSc/docs/current/service-kit/big-picture).

### quivr4s

### 1.2 Usage Examples
#### Problem:
The README doesn't contain code examples to show how the SDK can be used. Examples are essential for developers to quickly get started without diving deep into the codebase.

#### Suggested Improvements:
A Getting Started Example Code is required to show how to use brambl-sdk.

##### Creating a Transaction

```scala
import co.topl.brambl.Transaction

val tx = Transaction.create(sender = "address1", receiver = "address2", amount = 100)
println(s"Transaction: $tx")
```
##### Signing with Crypto

##### Interacting with service-kit


## 1.3 Improve Documentation Directory Structure
### Problem:
The repository has a documentation directory, but the README does not mention it explicitly, making it hard to find relevant documentation.

### Suggested Improvements:
- The link to the documentation should be added to the README with links to key files.
- API reference or module documentation
- Developer guides/tutorials
- Link to the documentation directory for example:
  - Refer to the documentation folder for detailed API usage and advanced guides.

- Provide navigation hints on where to start:
 - For a deep dive into our cryptographic library, visit /crypto/src.
 - To explore integration examples, check /integration/src/test."
   
## 1.4 Troubleshooting and FAQs Section
### Problem:
There’s no mention of common issues or troubleshooting tips. New users might run into errors, especially during installation or setup.

### Suggested Improvements:
Create a Troubleshooting section or FAQ. Example topics:
- **Issue:** Dependency conflicts with Scala version.
- **Solution:** Ensure you are using `Scala version X.X.X.`
- **Issue:** Tests fail with missing dependencies.
- **Solution:** Run `sbt clean && sbt update`.
  
## 1.5 Contribution Guidelines
### Problem:
There's no mention of how external contributors can contribute to the project.

## Suggested Improvements:
Add a "Contributing" section explaining;
- Code style guidelines link to contributing guide.
- How to submit pull requests.
- Running tests before submission.
  
