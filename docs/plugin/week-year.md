---
id: week-year
title: WeekYear
---
WeekYear adds `.weekYear()` API to get locale aware week of the year.

```javascript
var weekYear = require('dayjs/plugin/weekYear') // dependent on weekOfYear plugin
var weekOfYear = require('dayjs/plugin/weekOfYear')
dayjs.extend(weekOfYear)
dayjs.extend(weekYear)

dayjs().weekYear()
```
