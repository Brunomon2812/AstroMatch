# AstroMatch

A dating-app clone built with React, backed by a REST API that serves the profiles and records
each match.

**Live demo:** https://instinctive-aunt.surge.sh/

## About

AstroMatch presents one profile at a time. The user swipes through them by choosing to like or
pass:

- Liking a profile slides the card to the right; passing slides it to the left.
- When a like is reciprocated, a toast notification announces the match.
- The header icon switches to the matches list, which shows everyone matched so far.
- The matches list can be cleared, which resets the deck on the server.

The UI is composed with Chakra UI for the interactive pieces (buttons, toasts, images) and
styled-components for the layout shell.

## Tech stack

- [React](https://react.dev/)
- [Chakra UI](https://chakra-ui.com/)
- [Styled Components](https://styled-components.com/docs)
- [Axios](https://axios-http.com/docs/intro)

## API

Profiles, matches and the reset action come from the AstroMatch API:

| Method | Endpoint | Purpose |
| --- | --- | --- |
| `GET` | `/person` | Fetch the next profile to display |
| `POST` | `/choose-person` | Record a like or a pass, and report whether it was a match |
| `GET` | `/matches` | List every profile matched so far |
| `PUT` | `/clear` | Clear the match list and reset the deck |

## Running it locally

Requires Node.js.

```bash
git clone https://github.com/Brunomon2812/AstroMatch.git
cd AstroMatch
npm install
npm start
```

The app runs on http://localhost:3000 by default.

## Screenshots

<img width="379" alt="Profile screen with like and pass buttons" src="https://user-images.githubusercontent.com/104601906/188015078-d88b8f11-cbfe-4ef3-b32c-91a1cf2c2ae1.png">

<img width="376" alt="Matches list screen" src="https://user-images.githubusercontent.com/104601906/188015093-29f4a265-480c-4efb-b66d-c97ad642bf51.png">

## Author

Bruno Monteiro — [GitHub](https://github.com/Brunomon2812) · [LinkedIn](https://www.linkedin.com/in/brunoarmonteiro/)
