[![NPM Version][npm-image]][npm-url]
[![NPM Downloads][downloads-image]][downloads-url]
[![GitHub stars]()](https://github.com/WaleedAshraf/hubot-double-parking)

[![NPM][npm-download-image]][npm-url]

# hubot-double-parking

A hubot script that solves double parking issue.

See [`src/doubleParking.coffee`](src/doubleParking.coffee) for full documentation.

## Installation

In hubot project repo, run:

`npm install hubot-double-parking --save`

Then add **hubot-double-parking** to your `external-scripts.json`:

```json
[
  "hubot-double-parking"
]
```

## Sample Interaction

### Commands

```
hubot>> car find <number> - Will send message to owner of the car to visit parking.
hubot>> car add <number> <description> - Car with <number> will be added in the list against <user> name who run commnad.
hubot>> car update <number> <description> - Will update description of car mentioned.
hubot>> car remove <number> - Car with <number> will be removed from the list.
hubot>> car list - List all the cars.

```

#### Add Car
```
user1>> hubot car add 1234 Honda City
hubot>> Car Added: 1234 : user1 : user one : Honda City
```

#### Find Car
```
user2>> hubot car find 1234
hubot>> user1 please visit car parking. user2 is looking for you.
```

#### Update Car
```
user1>> hubot car update 1234 Toyota Corolla
hubot>> Car Updated: 1234 : user1 : user one : Toyota Corolla
```

#### List Car
```
user1>> hubot car list
hubot>> Number	| Owner		| Description
		1234 	| user one 	  Toyota Corolla
```

#### Remove Car
```
user1>> hubot car remove 1234
hubot>> Car removed: 1234
```

[npm-image]: https://img.shields.io/npm/v/hubot-double-parking.svg
[npm-url]: https://www.npmjs.com/package/hubot-double-parking
[npm-download-image]: https://nodei.co/npm/hubot-double-parking.png?downloads=true&downloadRank=true
[downloads-image]: https://img.shields.io/npm/dm/hubot-double-parking.svg
[downloads-url]: https://www.npmjs.com/package/hubot-double-parking
[star-image]: https://img.shields.io/github/waleedashraf/hubot-double-parking.svg?style=social&label=Star&maxAge=2592000
[star-url]: https://github.com/WaleedAshraf/hubot-double-parking