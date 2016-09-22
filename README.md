## Testing raml files in localhost

### Solution 1

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

- Goto https://5fpro.github.io/raml-api-console/?raml=https://api.shopmatic.dev/raml/index.raml and reload page for developing :)

### Solution 2

- install raml2html

```
npm install raml2html/raml2html#89a4dee02d39f04af0b6df13e37af69ab6b92e97 -g
```

- convert to index.html

```
raml2html -i doc/api-mobile/ramls/index.raml -o doc/api-mobile/ramls/index.html
```
