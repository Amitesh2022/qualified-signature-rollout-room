# Qualified Signature Rollout Room

## One-sentence benefit

Track secure remote qualified-signature delivery for citizens and public professionals in one accountable workspace.

## Live demo

[Watch the workflow](docs/demo.webm).

## Screenshots

![Qualified-signature rollout dashboard](docs/screenshot.png)

## Main features

- Search rollout files by service, certificate, user group or owner.
- Create rollout work through the Spring Boot API.
- Advance files through draft, review and approved states.
- Show live metrics and clear loading, empty and error feedback.
- Provide operational and delivery-guidance sections.

## Technology used

Angular, TypeScript, signals, computed state, OnPush change detection, Spring Boot and Java 21.

## Installation instructions

Install Node.js 22 and Java 21. Run `npm install`, then start the backend with `cd backend && mvn spring-boot:run`. In another terminal run `npm start`.

## Commercial licensing/contact

Commercial licensing and integration support are available. Use the repository contact options to discuss deployment.

## Business problem and users

Federal services, trust providers, programme teams and public professionals need to coordinate certificate readiness, legal alignment, accessibility and rollout evidence.

## Key workflows

Search rollout work, create an interoperability file, review ownership and risk, advance its state and confirm the persisted API result.

## Angular framework highlights

Signals and computed values manage local views, Angular HttpClient performs real API work, control flow renders states and OnPush limits unnecessary change detection.

## Java backend highlights

Spring Boot separates controller, service and domain concerns while providing validated CRUD-style APIs, health reporting, clear errors and Java tests.

## Architecture and state flow

Angular calls `/api/items` through its proxy. Validated requests enter the controller, workflow logic runs in the service and signals update from returned records.

## Accessibility and responsive behaviour

Semantic sections, associated labels, strong contrast, keyboard controls and responsive grids make the workflow usable across devices.

## Verification commands

Run `npm test`, `npm run build`, `cd backend && mvn test` and `cd backend && mvn package`.

## Structure

`src/app` contains the Angular experience, `backend` contains the Java service, and `docs` contains inspected media.

## Tradeoffs

Records are held in memory for a simple demonstration. Production rollout needs authentication, audit-grade persistence and trust-service integrations.

## Roadmap

Add certificate lifecycle events, professional roles, consent evidence and multilingual assisted-signing journeys.
