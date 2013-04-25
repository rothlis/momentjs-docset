To check if a variable is a moment object, use `moment.isMoment()`.

```javascript
moment.isMoment() // false
moment.isMoment(new Date()) // false
moment.isMoment(moment()) // true
```
