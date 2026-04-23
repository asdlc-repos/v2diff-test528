# Overview

An API that accepts a long URL and returns a short code that redirects to the original URL when visited.

# Personas

- Developer — integrates the API into their application to shorten URLs.
- End user — clicks a short link and gets redirected to the original destination.

# Features

- A developer sends a long URL to the API and receives a unique short code.
- When someone visits the short URL, they're redirected to the original long URL.
- Short codes are unique and don't collide with existing ones.
- The same long URL can be shortened multiple times and will get a new code each time.
- Short codes are compact, using letters and numbers.

Additionally, the system must record every redirect event (source IP, user-agent, timestamp) into a separate Analytics Service that exposes a GET /stats/{code} endpoint.

