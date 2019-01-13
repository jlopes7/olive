# Olive Oil Intelligent Load Distribution (aka OOILD)
Olive is a modern open source Load Balancer written in Java to solve key HA patterns and standards. It uses server introspection and intelligent load distribution to determine (compute) the right load path for your backend applications.

> **OOILD** is based on Apache's _Http Components_ to serve its HTTP asymptomatic requests, and several APIs to maintain its functions.

## Basic Architecture
Besides supporting common LD algorithms including _hashing_, _round robin_, OOILD goes further and implements the concept of "inteligent loading" by resolving the health of one's particular system during any given time. It implements that by using the idea of  "_Running Agents_". The core responsiblity of the Agents, is to continously instrospect the system's internal usage and safely send healthcheck pings to the Olive Server.


