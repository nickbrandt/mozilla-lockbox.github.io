## Initialization

* Local IndexedDB version mismatch
* Local IndexedDB initialization failures
* Local BrowserStorage loading failures

## Telemetry

* telemetry event recording failed
* telemetry scalar recording failed

## Network (common to sign-in, sync)

* device offline
* network-level failures (e.g., "client can't reach the server")
* server-side failures (e.g., "500 internal error")

## Sign-in

* [all network conditions](#network)
* authentication failures
    - User gave up
* application key mismatch
    - user reset password
    - user signs in with a different account
* local BrowserStorage saving failures

## Entries/Items

* Validation failures
    - too many origins
    - title/site name/username/password too long
* Local database failures
    - out of space
    - generic failures

## Sync failures

* [all network conditions](#network)
* authorization failures
    - "access token" expired
    - "access token" revoked
        + user changed password
        + user revoked device/app
* conflicts cannot be resolved
    - datastore locked (user signed out)
