# Timer

### Usage example
```javascript
new Timer({
  'duration': '00:00:05',
  'onStart': function(){
    console.log('Empieza!')
  },
  'onTick': function(time, timeDiff){
    console.log(time, timeDiff)
  },
  'onEnd': function(){
    console.log('Fin!')
  }
})
```

### Options

|Param|value|description
|---|---|---|
duration|`string` Format: `00:00:00`| Regressive count. If `null`, `undefined` or `00:00:00` the timer will be infinite (ascendent)
onStart|`function`|Function executed at the start
onTick|`function`|Function executed each tick (`time`, `timeDiff` milliseconds difference since las tick)
onEnd|`function`|Function executed at the end
