## HTTP and REST | Simple API

### Author: Steven Jones

### Links and Resources
* [PR](https://github.com/charmedsatyr-401-advanced-javascript/simple-api/pull/1)
* [front end](https://codesandbox.io/s/j29j15x2q9)

#### Documentation
* [swagger](docs/swagger.json)

### Modules
N/A

##### Exported Values and Methods
`./data/db.json`

###### Commands run to build records in `./data/db.json`
`echo '{"name":"electronics", "display_name":"Electronics","description":"Things you plug in."}' | http :3000/categories`

`echo '{"name":"fruit", "display_name":"Fruit","description":"Sweet plant bits you eat."}' | http :3000/categories`

`echo '{"name":"radio", "display_name":"RadioMAX","description":"It is too loud.", "category": "electronics"}' | http :3000/products`

`echo '{"name":"strawberry", "display_name":"Juicy, red strawberry","description":"It tastes so good!", "category": "fruit"}' | http :3000/products`

`echo '{"name":"banana", "display_name":"Big Panamanian banana","description":"It is yellow and curvy.", "category": "fruit"}' | http :3000/products`

#### Running the app
* `json-server --watch data/db.json --id=_id`
* Ensure `json-server` is running on port 3000.
* Navigate to `https://codesandbox.io/s/j29j15x2q9`
* Categories and their corresponding products should display when a category is clicked:
  * `electronics` -> `radio`
  * `fruit` -> `strawberry`, `banana`
* If `json-server` is running as indicated, you should be able to make additions or modifications to `./data/db.json` through the `json-server` API or through requests made through the `swagger.io` interface after copying/pasting the documentation at `./docs/swagger.json` into an editor at [https://editor.swagger.io](https://editor.swagger.io).

#### Tests
* How do you run tests?

N/A
* What assertions were made?

N/A
* What assertions need to be / should be made?

N/A

#### UML
N/A