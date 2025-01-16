# Expo useLinking Hook: Query Parameter Parsing Issue

This repository demonstrates a bug in Expo's `useLinking` hook where query parameters in deep links are not parsed correctly. The bug results in the query parameters being unavailable or misinterpreted within the application.

## Bug Description

The `useLinking` hook, when provided a deep link URL containing query parameters, fails to extract these parameters accurately. This leads to unexpected behavior in the application, potentially causing crashes or incorrect data handling.

## Reproduction Steps

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Start the Expo development server.
4. Open the app on a device or simulator.
5. Try navigating to a deep link with query parameters (e.g., `myapp://myroute?param1=value1&param2=value2`).
6. Observe that the query parameters are not correctly parsed or are missing entirely.

## Solution

A workaround involves manually parsing the URL after obtaining the initial route from `useLinking`. This ensures that query parameters are correctly extracted and processed.

## Related Issues

- [Link to any relevant Expo issues](link)

## License

MIT