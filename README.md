# Buildpack: Go Binary

> A buildpack that executes a binary on Heroku, and identifies it as a Go application.

The `go-binary-buildpack` is heavily based on the [Ø buildpack](https://github.com/ryandotsmith/null-buildpack)
with the only change being that the detected language is `Go` instead of `Null`

## Note

You need to provide a binary that can be executed by 64 bit Linux (`GOOS=linux GOARCH=amd64`)
and a **Procfile** with `web: ./name-of-the-binary`
