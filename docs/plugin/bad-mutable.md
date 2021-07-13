---
id: bad-mutable
title: BadMutable
---

Day.js is designed to be immutable, however, in order to make it fully compatible with moment.js in some legacy projects we introduced a plugin 🚨 BadMutable 🚨 to make Day.js mutable.

> This is __NOT__ good and __NOT__ recommended for most projects.

With this plugin enabled, all setters will update the instance itself.

```javascript
var badMutable = require('dayjs/plugin/badMutable')
dayjs.extend(badMutable)
// with 🚨 BadMutable 🚨 plugin
const today = dayjs()
today.add(1, 'day')
console.log(today) // update itself, value will be tomorrow
```
