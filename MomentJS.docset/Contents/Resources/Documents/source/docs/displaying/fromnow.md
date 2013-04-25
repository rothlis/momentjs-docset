A common way of displaying time is handled by `moment#fromNow`. This is sometimes called timeago or relative time.

```javascript
moment([2007, 0, 29]).fromNow(); // 4 years ago
```

If you pass `true`, you can get the value without the suffix.

```javascript
moment([2007, 0, 29]).fromNow();     // 4 years ago
moment([2007, 0, 29]).fromNow(true); // 4 years
```

The base strings are [customized by the current language](#/customization/relative-time/).

The breakdown of which string is displayed for each length of time is outlined in the table below.

<table class="table table-striped table-bordered">
  <thead>
    <tr>
      <th>Range</th>
      <th>Key</th>
      <th>Sample Output</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>0 to 45 seconds</td>
      <td>s</td>
      <td>seconds ago</td>
    </tr>
    <tr>
      <td>45 to 90 seconds</td>
      <td>m</td>
      <td>a minute ago</td>
    </tr>
    <tr>
      <td>90 seconds to 45 minutes</td>
      <td>mm</td>
      <td>2 minutes ago ... 45 minutes ago</td>
    </tr>
    <tr>
      <td>45 to 90 minutes</td>
      <td>h</td>
      <td>an hour ago</td>
    </tr>
    <tr>
      <td>90 minutes to 22 hours </td>
      <td>hh</td>
      <td>2 hours ago ... 22 hours ago</td>
    </tr>
    <tr>
      <td>22 to 36 hours</td>
      <td>d</td>
      <td>a day ago</td>
    </tr>
    <tr>
      <td>36 hours to 25 days</td>
      <td>dd</td>
      <td>2 days ago ... 25 days ago</td>
    </tr>
    <tr>
      <td>25 to 45 days</td>
      <td>M</td>
      <td>a month ago</td>
    </tr>
    <tr>
      <td>45 to 345 days</td>
      <td>MM</td>
      <td>2 months ago ... 11 months ago</td>
    </tr>
    <tr>
      <td>345 to 547 days (1.5 years)</td>
      <td>y</td>
      <td>a year ago</td>
    </tr>
    <tr>
      <td>548 days+</td>
      <td>yy</td>
      <td>2 years ago ... 20 years ago</td>
    </tr>
  </tbody>
</table>
