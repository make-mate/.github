# MakeMate

**Build continuously running digital mates.**

MakeMate is an open ecosystem for building **digital mates**—software systems that continuously perform operational responsibilities on behalf of people, devices and services.

Unlike traditional applications that are started, used and closed, a digital mate runs continuously. It reacts to events, executes scheduled work, maintains state, communicates with external systems and provides web-based user interfaces whenever needed.

A few examples of digital mates are:

* EV Charging Mate
* Pool Mate
* Irrigation Mate
* Home Energy Mate
* Building Monitoring Mate

---

## What is a digital mate?

A digital mate is an operational software companion responsible for a specific domain.

A mate may:

* monitor sensors and external systems
* make decisions
* control devices
* serve web pages and APIs
* notify users
* persist application data
* run scheduled tasks
* cooperate with other mates

Digital mates are designed to run continuously, often for months or years without interruption.

---

## How MakeMate works

MakeMate separates **execution**, **capabilities** and **solutions**.

* **Runtime** executes models.
* **Models** provide reusable capabilities.
* **Mates** combine one or more models into complete operational solutions.

This separation makes models reusable across many different applications while allowing each mate to focus on solving a specific operational problem.

---

## Repository overview

| Repository           | Purpose                                                                              |
| -------------------- | ------------------------------------------------------------------------------------ |
| **runtime**          | Execution platform for loading and running models.                                   |
| **lab-model**        | Development, diagnostics and runtime management environment.                         |
| **portal-model**     | Configurable portal and application entry point.                                     |
| **users-model**      | Authentication, authorization and user management.                                   |
| **assets-model**     | Shared representation of physical and logical assets.                                |
| **dataeditor-model** | Generic browser-based editing of persistent application data.                        |
| **charging-model**   | Reference implementation of a complete digital mate for EV charging.                 |
| **examples**         | Runnable examples demonstrating model composition and recommended project structure. |

---

## Design principles

MakeMate is built around a few simple ideas.

* Long-running operational software rather than request/response applications.
* Configuration over programming whenever practical.
* Reusable models with clearly defined responsibilities.
* Event-driven execution combined with scheduled processing.
* Browser-based operation and administration.
* Security built into the platform rather than individual applications.
* Incremental composition of larger systems from small reusable models.

---

## Technology

The MakeMate runtime is implemented in Go.

Applications are primarily described using declarative models written in YAML together with Bloblang expressions, HTML templates and SQL where appropriate. Most digital mates require little or no traditional programming.

---

## Getting started

If you're new to MakeMate, the recommended path is:

1. Start with the **runtime** repository.
2. Read the Runtime README.
3. Run one of the examples.
4. Explore the Lab model.
5. Build your first digital mate by combining existing models.
6. Extend the platform with your own models as needed.

---

## Vision

Our goal is to make operational software easier to build than traditional applications.

Instead of repeatedly developing authentication, scheduling, persistence, dashboards, web servers and infrastructure for every project, MakeMate lets you assemble reusable models into digital mates that solve real operational problems.
