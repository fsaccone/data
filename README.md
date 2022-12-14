# Data
The repository used by me as a HTTP API to get static data.

# Endpoints
## About me
```http
GET https://fsaccone.github.io/data/me/about-me
```

### Returns
| Key             | Type   | Description
| ----------------|--------|--------------------
| `icon_url`      | string | The URL of my icon.
| `description`   | string | My description.
| `contact_email` | string | My contact email.

#### Used by my [website](https://github.com/fsaccone/website).

## Social media
```http
GET https://fsaccone.github.io/data/me/social-media
```

### Returns _an array of_
  | Key          | Type   | Description
  | -------------|--------|--------------------
  | `name`       | string | The name of the social media.
  | `url`        | string | The link to the profile.
  | `image_path` | string | The URL of the social icon.

#### Used by my [website](https://github.com/fsaccone/website).

## Skills
```http
GET https://fsaccone.github.io/data/me/skills
```

### Returns _an array of_
  | Key          | Type             | Description
  | -------------|------------------|--------------------
  | `title`      | string           | The name of the skill.
  | `images`     | _Array<_`Image`_>_ | An array containing `Image`.
### `Image`
  | Key   | Type   | Description
  |-------|--------|-----------------
  | title | string | The alt of the image
  | url   | string | The URL.

## Project configurations
```http
GET https://fsaccone.github.io/data/packages/project-configurations
```

### Returns _an array of_
  | Key             | Type                  | Description
  | ----------------|-----------------------|--------------------
  | `name`          | string                | The name of the configuration.
  | `url`           | string                | The URL to the archive.
  | `done_message`? | string \| _undefined_ | The message logged after the writing succeded.

#### Used by my [CLI](https://github.com/fsaccone/cli).
