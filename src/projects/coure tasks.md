---
title: "Course tasks"
summary: "Task solutions"
image: /images/course-tasks.jpg
imageAlt: "Screenshots of couse tasks app"
tech:
  - "HTML"
  - "CSS"
  - "JS"
siteUrl: "#"
repoUrl: "#"
---

### Table challenge

[Click here to open CodePen](https://codepen.io/StanislavPetrov/pen/wvXRePo?editors=1100)
#### HTML Code
~~~
<html>
  <head>
    <title>Table challenge</title>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <link href='https://fonts.googleapis.com/css?family=Rock Salt' rel='stylesheet'>
    <link rel="preconnect" href="https://fonts.googleapis.com">

    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Flex:opsz,wght@8..144,400;8..144,700&display=swap" rel="stylesheet">

    <link rel="stylesheet" href="./style.css">
  </head>

  <body>
    <table>
        <thead>
          <tr>
            <td style="width: 30%;">Band</td>
            <td style="width: 20%;">Year formed</td>
            <td style="width: 20%;">No. of Albums</td>
            <td style="width: 30%;">Most famous song</td>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><b>Buzzcocks</b></td>
            <td>1976</td>
            <td>9</td>
            <td>Ever fallen In love (with someone you shouldn't've)</td>
          </tr>
          <tr>
            <td><b>The Clash</b></td>
            <td>1976</td>
            <td>6</td>
            <td>London Calling</td>
          </tr>
          <tr>
            <td><b>The Damned</b></td>
            <td>1976</td>
            <td>10</td>
            <td>Smash it up</td>
          </tr>
          <tr>
            <td><b>Sex Pistols</b></td>
            <td>1975</td>
            <td>1</td>
            <td>Anarchy in the UK</td>
          </tr>
          <tr>
            <td><b>Sham 69</b></td>
            <td>1976</td>
            <td>13</td>
            <td>If The Kids Are United</td>
          </tr>
          <tr>
            <td><b>Siouxsie and the Banshees</b></td>
            <td>1976</td>
            <td>11</td>
            <td>Hong Kong Garden</td>
          </tr>
          <tr>
            <td><b>Stiff Little Fingers</b></td>
            <td>1977</td>
            <td>10</td>
            <td>Suspect Device</td>
          </tr>
          <tr>
            <td><b>The Stranglers</b></td>
            <td>1974</td>
            <td>17</td>
            <td>No More Heroes</td>
          </tr>
        </tbody>
        <tfoot>
          <tr>
            <td class="total" colspan="2">Total albums</td>
            <td class="total-count" colspan="2">77</td>
          </tr>
        </tfoot>
      </table>
      <p class="end-paragraph">A summary of the UK's most famous punk bands</p>
  </body>
</html>
~~~

#### CSS code
~~~
body {
  margin: 2em;
}

table {
  border: 2px solid#800080;
  border-collapse: collapse;
  text-align: center;
  width: 100%;
}

thead {
  font-family: "Rock Salt";
  color: #fff;
  background: linear-gradient(rgba(0,0,0,0.1),  rgba(0,0,0,0.5)), url("https://cdn.glitch.com/8b1beacc-937c-4072-93d6-4ae825ab1a7a%2Fleopardskin.jpg?1527763317245");
}

thead td {
  border: 2px solid #800080;
  padding: 3px;
}

tbody {
  font-family: 'Roboto Flex', sans-serif;
}

tbody tr:nth-child(even) {
  background: url("https://cdn.glitch.com/8b1beacc-937c-4072-93d6-4ae825ab1a7a%2Fnoise.png"), #e495e4;
}

tbody tr:nth-child(odd) {
  background: url("https://cdn.glitch.com/8b1beacc-937c-4072-93d6-4ae825ab1a7a%2Fnoise.png"), #ff33cc;
}

tbody td {
  padding: 8px;
  font-size: 14px;
}

tfoot {
  color: #fff;
  background: linear-gradient(rgba(0,0,0,0.1),  rgba(0,0,0,0.5)), url("https://cdn.glitch.com/8b1beacc-937c-4072-93d6-4ae825ab1a7a%2Fleopardskin.jpg?1527763317245");
}

tfoot td {
  padding: 3px;
  border: 2px solid #800080;
}

.total {
  font-family: 'Rock Salt';
  padding-right: 10px;
  text-align: right;
}

.total-count {
  font-family: 'Roboto Flex', sans-serif;
  padding-left: 10px;
  text-align: left;
}

.end-paragraph {
  text-align: right;
  font-family: 'Rock Salt';
  font-size: 14px;
}
~~~
#### And the result:
<img src="/images/table-challenge.jpg" alt="Table picture" />