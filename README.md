# [Building a Three-Tier Web Application with ASP.NET 2.0, C#, Spring.Net, and NHibernate (2010)](https://stahe.github.io/en-pam-aspnet-juin-2010/)

This document presents the step-by-step development of **SimuPaie**, a .NET application designed to simulate the calculation of child care providers’ pay. The focus is twofold: **establishing a clear software architecture** and **implementing the solution using the .NET technologies available at the time**. In particular, the document describes a **three-tier architecture** consisting of a data access layer (DAO), a business layer, and a presentation layer, all integrated using **Spring IoC**.

## Course Objectives

The purpose of this case study is to demonstrate how to design a maintainable web application by clearly separating responsibilities:

- **Layer 1 - DAO**: access to data stored in the database.
- **Layer 2 - Business**: payroll calculations and business rules.
- **Layer 3 - UI**: user interaction and display of results.
- **Integration** of the layers via **.NET interfaces** and **dependency injection with Spring IoC**.

The document also outlines the user request processing cycle: the request is received by the application, forwarded if necessary to the business layer and then to the data access layer, before an appropriate response is sent back to the client.

## Successive versions of the application

The documentation is not limited to a single implementation. It offers several variations of SimuPaie to illustrate different architectural and interface approaches:

1. a **single-form ASP.NET** version with a single-tier architecture;
2. an equivalent version enhanced with **Ajax**;
3. a **three-tier ASP.NET** version with **NHibernate** for data access;
4. a **multi-view, single-page** version;
5. a server-side **web service**-oriented version;
6. an ASP.NET client version consuming this service;
7. a **multi-view, multi-page** version;
8. a client version of the web service;
9. a three-tier variant relying more heavily on Spring classes to facilitate the use of NHibernate;
10. a **FLEX** client version.

## Prerequisites

This document is intended for an **intermediate** level. It assumes a basic understanding of:
- **ASP.NET**
- **C# 2008**: classes, interfaces, inheritance, polymorphism
- **Spring IoC / dependency injection**
- **three-tier web architecture** and the **MVC** model.

## Tools and technologies covered

The case study is based on a coherent set of tools and frameworks:

- **Visual C# 2008**
- **Visual Web Developer Express 2008**
- **SQL Server Express 2005**
- **Spring.Net / Spring IoC**
- **NHibernate**
- **NUnit** for unit testing.

## What this repository offers

This resource will be of particular interest to readers who want to:

- understand the implementation of a **n-tier architecture** in a .NET environment;
- see how to **decouple** the presentation, business logic, and data access layers;
- discover how to use **Spring.Net** for component assembly;
- study the integration of **NHibernate** into an ASP.NET web application;
- follow a step-by-step learning path progressing from a simple version to more production-ready versions.

## Course Content

The document outlines the application’s general architecture and, starting on the first page, uses a diagram to illustrate the roles of the user, the application, the three layers, and Spring IoC in orchestrating the whole system. It therefore serves as both an **architecture course**, a **design guide**, and a **working foundation for practical implementation**.

