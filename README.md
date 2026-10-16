# Nordic Microalgae: Content

![CI workflow](https://github.com/nordicmicroalgae/content/actions/workflows/ci.yml/badge.svg)

This repository contains all content used in Nordic Microalgae with the exception of contributed images of species.

The most common format for content is plain-text, although the `assets` folder contains some multi-media files that are referenced to from some of the Markdown articles.

## Species

All species related content is stored in the `species` folder. This is data that has been pre-processed in our data pipeline and is ready for ingestion by our backend service.

When files in `species` are changed, a CI workflow verifies that they can be imported by the backend. Changes are fetched by the web servers within 15 minutes, but are not visible on the website until a synchronization has been run from the administration interface.

## Pages & News

Generic information pages and news articles consist of a bunch of Markdown documents and are found within this repo as well. Pages are located at root level of this repository and news inside the `_posts` folder. This also adheres to the common setup for e.g GitHub pages.

Pages, news and files in `assets` are read directly from this repository and are visible on the website within 15 minutes after a push.
