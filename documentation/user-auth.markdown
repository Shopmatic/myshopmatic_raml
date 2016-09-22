These 3 endpoing can get user_token:

- POST /sessions/email
- POST /sessions/facebook
- POST /sessions/googleplus

While login success and get value of `user_token`, please save it localy.

For endponts required login (almost all), put token value to query parameters with key:`user_token` will be works for user login requirement. For examples:
- `POST /images` with form data: `user_token=abcdefg`
- `GET /orders?user_token=abcdefg`
