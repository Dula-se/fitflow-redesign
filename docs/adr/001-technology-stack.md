# ADR 001: FitFlow Technology Stack

## Status

Accepted

## Context

FitFlow needs a modern technology stack that supports cross-platform mobile development, AI-powered personalization, nutrition tracking, real-time social features, and secure health-related data management.

The solution must also support fast development, scalability, maintainability, and privacy.

## Decision

The following technology stack was selected:

- Frontend: React Native
- Backend: Node.js + Express
- Authentication: Firebase Authentication
- Real-time/Social Database: Firebase Firestore
- Structured/Health Database: PostgreSQL
- AI/ML: TensorFlow Lite + ML Kit
- Caching: Redis

## Rationale

React Native provides efficient cross-platform development for iOS and Android with React Native Web available for the optional web client.

Node.js and Express provide a simple API layer with strong real-time support and JavaScript/TypeScript consistency.

Firebase Firestore is suitable for real-time social features, while PostgreSQL provides strong relational integrity and auditability for sensitive health data.

Firebase Authentication provides fast integration and strong OAuth support.

TensorFlow Lite and ML Kit support on-device personalization and computer vision while reducing unnecessary health-data transmission.

## Consequences

The solution enables fast cross-platform delivery, real-time community features, AI capabilities, and secure structured health-data storage.

The main trade-off is the operational complexity of using two databases. Clear data ownership, a shared user identifier, monitoring, and documented synchronization rules are required.
