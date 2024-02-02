# Config

Within the Crytonix directory, there is a file called `config.json`. This file contains all of the configuration options for Crytonix. Below is a list of all the options and their descriptions.

## `captcha_settings`

This includes all of the settings for the captcha solver.

### `service`

The service to use for solving captchas. The available options can be found below.

> ![NOTE]
>
> Capitalisation does matter.

- `CapSolver`
- `CapBypass`
- `AutoCap`
- `HexoSolver`
- `Custom` (see more information below)

### `api_key`

If you are not using the `Custom` service, simply put your API key here.

If you are using the `Custom` service, put the URL to your captcha solving service and the API key in the following format:

> ![NOTE]
>
> Crytonix assumes the solver's API is exactly the same as `CapBypass`, but with a different base URI. 

```json
["https://example.com", "API_KEY"]
```

## `files`

Configure the input and output files here.

### `cookie_file`

The file path to the [cookies](./cookies.md) file.

### `proxy_file`

The file path to the [proxies](./proxies.md) file.

### `output_folder`

The directory path to save the output files.