# Help2Code Join Page

This directory contains the web pages that handle Help2Code session invitation links.

## How it works

1. When a host shares a session link, it points to `https://help2code.github.io/join?token=YOUR_TOKEN`
2. This page extracts the token from the URL and displays it to the collaborator
3. The collaborator can copy the token and use it to join the session in VS Code

## Deployment

These pages are designed to be deployed to GitHub Pages. To deploy:

1. Push this `docs` directory to the `main` branch of the `help2code/help2code.github.io` repository
2. GitHub Pages will automatically serve the content

## Customization

If you want to use your own server instead of GitHub Pages:

1. Deploy these HTML files to your web server
2. Update the `help2code.joinLinkBaseUrl` setting in VS Code to point to your server

## Local Testing

To test locally:

1. Open the HTML files directly in your browser
2. Add `?token=test-token` to the URL to simulate a real invitation link