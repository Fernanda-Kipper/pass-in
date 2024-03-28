# Pass.In API

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)

This project is an API built using **Java, Java Spring, Flyway Migrations, HSQLDB as the database.**

This project simulates the operation of an in-person event management dashboard, built during [Next Level Week Unite](https://www.rocketseat.com.br/eventos/nlw?utm_source=kipperdev&utm_medium=organic&utm_campaign=lead&utm_term=evento-nlw&utm_content=pagevento-lp_evento_nlw_unite_inscricao), a free event where I built the project from scratch to teach the community of developers starting in the area.

## Table of Contents

- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)


## Requirements

### Functional requirements

[x] The organizer must be able to register a new event.

[x] The organizer must be able to view event data.

[x] The organizer must be able to view the list of participants.

[x] The participant must be able to register for an event.

[x] The participant must be able to view their registration badge.

[x] The participant must be able to check-in at the event.

### Business rules

[x] Participants can only register for an event once.

[x] Participants can only register for events with available places.

[x] Participants can only check-in to an event once.

### Non-functional requirements

[x] Check-in at the event will be carried out using a QRCode.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/Fernanda-Kipper/pass-in.git
```

2. Install dependencies with Maven

## Usage

1. Start the application with Maven
2. The API will be accessible at http://localhost:8080

## API Endpoints
The API provides the following endpoints:

```markdown
POST /events - Register a new event.

GET /events/{eventId} - Retrieve event details.

GET /events/attendees/{eventId} - Retrieve the list of participants registered for specified event.

POST /events/{eventId}/attendees - Register a new participant to event.

POST /attendees/{attendeeId}/badge - Retrieves participant badge to access the event.

POST /attendees/{attendeeId}/check-in - Check in participant in the event.
```



