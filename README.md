# Api Document

- Goto staging raml: https://5fpro.github.io/raml-api-console/?raml=https://shopmatic.github.io/myshopmatic_raml/index.raml

# Modify RAMLs

- repo: https://github.com/Shopmatic/myshopmatic/
- in `./doc/api_mobile/ramls/*.raml`

# Offical MD of RAML 1.0

- https://github.com/raml-org/raml-spec/blob/master/versions/raml-10/raml-10.md/

# Publishing

- in repo: https://github.com/Shopmatic/myshopmatic/
- `rake raml:publish`

# Published repo

- https://github.com/Shopmatic/myshopmatic_raml

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

- Load raml from local

```
edit /doc/api-mobile/ramls/index.raml
change "baseUri" host for local
```

- Goto local raml: https://5fpro.github.io/raml-api-console/?raml=https://api.shopmatic.dev/raml/index.raml
