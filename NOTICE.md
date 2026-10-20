# Notice

## No licence is granted

This repository is a distribution channel. It contains a README and signed APK
builds — no source code.

No open-source licence is granted for anything here, and none is implied by the
absence of one. You may download a build and install it on your own devices for
your own use. You may not copy, redistribute, modify, rebrand or sell it, or
present a modified build as this project.

## No warranty

Each APK is provided **as is**, with no warranty of any kind, express or
implied, including fitness for a particular purpose.

## No content, no affiliation

iLive TV is a client application. It hosts no streams, no channel content and no
television events. It runs no streaming infrastructure and stores no media. The
channel catalogue, the guide data, event listings and every stream URL are
fetched at runtime from public third-party web services and public IPTV sources.

Playback therefore depends entirely on those external sources and on the
consumer's own network connection. Availability, legality, reliability and
quality of any third-party stream are outside this project's control and are not
guaranteed by it. This project has no affiliation with, endorsement of, or
control over any broadcaster, channel operator, stream host or rights holder,
and the inclusion of a listing does not imply that the underlying stream may
lawfully be viewed from the consumer's location.

Responsibility for observing applicable law in the consumer's own jurisdiction
rests with the consumer.

## Trademarks

Channel names, network names, sports bodies, event names and logos referenced by
the listings are the property of their respective owners. Their appearance here
is incidental and does not imply any endorsement, affiliation or authorisation.

## Versions

Releases are published under tags of the form `vMAJOR.MINOR` — for example
`v1.02`. The tag is what the in-app updater compares against, so a build's
`versionName` in `app/build.gradle.kts` must match the tag it is published as.

A build's `versionCode` is enforced by Android on install and must always be
**higher** than the versionCode already installed. Bump both before tagging a
release: the updater compares `versionName`, but Android rejects the install if
`versionCode` did not move forward.