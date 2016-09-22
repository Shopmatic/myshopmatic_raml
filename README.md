# Api Document

- Go to https://5fpro.github.io/raml-api-console/?raml=https://shopmatic.github.io/myshopmatic_raml/index.raml

# Modify RAMLs

- in `./doc/api_mobile/ramls/*.raml`

# Publishing

- `rake raml:publish`

# Debug and preview

- let pow support `api.shopmatic.dev` subdomain.

```
cp ~/.pow/shopmatic ~/.pow/api.shopmatic
```

- let pow support ssl.

```
gem install tunnelss
sudo tunnelss
# or
rvmsudo tunnelss
```

- Start rails server

```
foreman start
# or
rails s
```

- Goto https://5fpro.github.io/raml-api-console/?raml=https://api.shopmatic.dev/raml/index.raml and reload page for developing
