# Coinflip Command

## Example
```js
module.exports = {
    name: "coinflip",
    category: 'Leaf',
    code: `$djsEval[(async () => {
    const { Coinflip } = require('leaf-utils')
      
await Coinflip({
    message: message,
    embed: {
      title: 'Coinflip',
      color: 'RED',
    },
    buttons: {
      heads: 'Heads',
      tails: 'Tails',
    },
    colors: {
      heads: 'DANGER',
      tails: 'PRIMARY',
    },
    startMessage: 'The coin is in the air Choose heads or tails below.',
    winMessage: 'GG, <@{{winner}}> The coin landed on **{{result}}**',
    loseMessage: '<@{{player}}> You lose The coin landed on **{{result}}**',
    ongoingMessage: 'A game is already runnning in <#{{channel}}>. You cant start a new one',
    othersMessage: 'Only <@{{author}}> can use buttons'
})
})()]
$suppressErrors`
}
```

## Button Styles
![button](https://user-images.githubusercontent.com/70775569/136095482-f0a34325-bf48-41a1-ada0-45c46e448d3e.jpg)

