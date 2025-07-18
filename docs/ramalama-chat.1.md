% ramalama-chat 1

## NAME
ramalama\-chat - OpenAI chat with the specified REST API URL

## SYNOPSIS
**ramalama chat** [*options*] [arg...]

positional arguments:
  ARGS                  overrides the default prompt, and the output is
                        returned without entering the chatbot

## DESCRIPTION
Chat with an OpenAI Rest API

## OPTIONS

#### **--api-key**
OpenAI-compatible API key.
Can also be set via the API_KEY environment variable.

#### **--color**
Indicate whether or not to use color in the chat.
Possible values are "never", "always" and "auto". (default: auto)

#### **--help**, **-h**
Show this help message and exit

#### **--prefix**
Prefix for the user prompt (default: 🦭 > )

#### **--url**=URL
The host to send requests to (default: http://127.0.0.1:8080)

## EXAMPLES

Communicate with the default local OpenAI REST API. (http://127.0.0.1:8080)
With Podman containers.
```
$ ramalama chat
🦭 >

Communicate with an alternative OpenAI REST API URL. With Docker containers.
$ ramalama chat --url http://localhost:1234
🐋 >
```

## SEE ALSO
**[ramalama(1)](ramalama.1.md)**

## HISTORY
Jun 2025, Originally compiled by Dan Walsh <dwalsh@redhat.com>
