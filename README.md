# base64-custom-pattern
checked for base 64 as per a post - needs to be validated as pattern

This is a pattern I developed using GitHub Copilot for base64:
`(?:.{1,124})(?:(?i)(?:[A-Z0-9+/]{4}){20,}(?:[A-Z0-9+/]{2}==|[A-Z0-9+/]{3}=)?)(?:.{0,})`

NOTE: Because short strings like `base` and `post` are valid base64 encoded values I have setup the regex to find base64 strings between 10 and 149 chars in length.

These are some valid base64 encoded strings to test
dGVzdAo=
c2RmYXNmZGRzZmZzZA==
dGVzdGEK
c2Rma2hqc2FkZmhrc2hhZGZramhhc2RmamhERlNqbGtoYWZka2psaGZhamxraGRhZmxraGRhc2Zqa2xkc2ZoamFrbHNkaGZqa2RzYWhmbGprYWRzaGZrbGFkamhmamtsYXNoYQ==
