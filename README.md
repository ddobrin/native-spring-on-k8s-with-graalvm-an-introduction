# native-spring-on-k8s-with-graalvm-an-introduction

This repo contains all the materials required for the `An Introduction to Native Spring on K8s with GraalVM` workshop.

The workshop is designed to help Spring Boot developers build new / modernize existing applications using Spring Native and deploy them in Kubernetes. 
Basic knowledge of Spring Boot and Kubernetes is assumed for successful completion.

This workshop is followed by the `Advanced Spring Native with GraalVM` workshop.

---

## Context

This content contains sample code supporting the workshop agenda, with a focus on building Native Applications using Spring Native and GraalVM.

The content is organized around a number of independent sections, each with a `README.md` file explaining how to build and run the samples, 
or pointing out areas of interest, for further exploration. 

The content focuses on the following main areas:
* [Prerequisite Software Setup and Validation](setup/README.md) 
* Understanding GraalVM
* Building [Spring Native](spring-native/README.md) Applications with GraalVM
* Best Practices for designing native-friendly Spring apps and libraries
* [Complete](complete/README.md) Spring Native examples

The following areas are explored in-depth in the  `Advanced Spring Native` workshop:
* Understanding [GraalVM](graalvm/README.md) 
* Building [Spring Native](spring-native/README.md) Applications with GraalVM
* [Best Practices](best-practices/README.md) for designing native-friendly Spring apps and libraries

----
## Repository

This workshop repository can be cloned to your machine as follows:
```shell
# SSH
> git clone git@github.com:ddobrin/native-spring-on-k8s-with-graalvm-an-introduction.git

# HTTPs
> git clone https://github.com/ddobrin/native-spring-on-k8s-with-graalvm-an-introduction.git 
```

Full samples are provided for each lab or demo! 

All samples are relative to the repository root, for ex.:
```shell
# Petclinic
<repo-root>/complete/petclinic-jdbc
```

---------

## Environment setup and validation
**Please start** by cloning the repo, then **follow** the [environment setup and validation section](setup/README.md) `prior` to the start of the workshop.

---------
## Workshop - Detailed Agenda

1. Introduction
2. [Setup Validation](setup/README.md) - say "Hello Workshop" 
    * **[Hands-on Setup Lab](setup/README.md#Build-Run-App)**
3. Let's get started - How fast are your pets? Let's build some images for them !
    * **[Hands-on Lab](complete/petclinic-jdbc/README.md)**
4. Demystifying Native Images
    * Let's talk about JVM vs Native
    * Introducing ahead-of-time compilation (AOT)
    * Making close-world assumptions
    * When to modernize apps with native images ? Let's see the use-cases 
   * Why not use Native Images everywhere?
5. Understanding GraalVM
    * GraalVM Architecture
    * Native Image technology for ahead-of-time compilation
    * Build configuration for a native image build process
    * Initialization
    * AOT compilation limitations - what do I need to know?
    * Visualization Tools - GraalVM Dashboard
6. Are there any alternatives to GraalVM?
7. What are our competitors saying? 
8. [Building Spring Native Applications](spring-native/README.md) with GraalVM
    * What is Spring Native and why use it ?
    * AOT compilation limitations - how do Native Hints in Spring help bypass them ? -- **[Demo(s)](spring-native/README.md#Demo)**
       * Accessing Resources in Spring Native Images 
         * **[Demo](spring-native/README.md#Lab)**
    * Spring Native's limitations - what do I need to know ?
    * Building with the Spring AOT Maven plugin 
    * Cloud Native Buildpacks -support source-to-image for native images 
        * Building, containerizing and running a Spring Native app and **_diving_** into the built image
            * **[Optional Hands-on Lab](spring-native/README.md#Lab)**
    * Using a container-based Spring Native build environment
    * Troubleshooting tips
9. Performance expectations
10. Any Best Practices for designing native-friendly Spring apps and libraries?
    * Identification of AOT limitations in the app
    * Building a Spring Native Shared Library
    * Comparing Images
11. Spring Native Roadmap

#### Appendix:
* [Complete Spring Native examples](complete/README.md)

