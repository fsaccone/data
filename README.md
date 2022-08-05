# Data
The repository used by me as a HTTP API to get static data.

## Endpoints
```http
GET https://fsaccone.github.io/data/me/about-me
```
Returns
* `icon_url`: string
* `description`: string
* `contact_email`: string

---


```http
GET https://fsaccone.github.io/data/me/social-media
```
Returns
* An array of
  * `name`: string
  * `url`: string
  * `image_path`: string
