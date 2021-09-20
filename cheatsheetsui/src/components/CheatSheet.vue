<template>

  <div class="cheatsheet">
    <h1>C# Datetime formats </h1>
    <br />
    Variants DateTimeOffset ru-RU sv-SE el-GR
    <br />
    <br />
    <table class="table">
      <caption class="visually-hidden">
        Table of format specifiers
        <br />
        <br />
      </caption>
      <thead>
        <tr>
          <th>Format specifier</th>
          <th>Description</th>
          <th>Examples</th>
          <th>Result</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>"d"</td>
          <td>Short date pattern.</td>
          <td>2009-06-15T13:45:30</td>
          <td>6/15/2009</td>
        </tr>
        <tr>
          <td>"D"</td>
          <td>Long date pattern.</td>
          <td>2009-06-15T13:45:30</td>
          <td>Monday, June 15, 2009 </td>
        </tr>
        <tr>
          <td>"f"</td>
          <td>Full date/time pattern (short time).</td>
          <td>2009-06-15T13:45:30</td>
          <td>Monday, June 15, 2009 1:45 PM </td>
        </tr>
        <tr>
          <td>"F"</td>
          <td>Full date/time pattern (long time).</td>
          <td>2009-06-15T13:45:30</td>
          <td>Monday, June 15, 2009 1:45:30 PM</td>
        </tr>
        <tr>
          <td>"g"</td>
          <td>General date/time pattern (short time).</td>
          <td>2009-06-15T13:45:30</td>
          <td>6/15/2009 1:45 PM </td>
        </tr>
        <tr>
          <td>"G"</td>
          <td>General date/time pattern (long time).</td>
          <td>2009-06-15T13:45:30</td>
          <td>6/15/2009 1:45:30 PM </td>
        </tr>
        <tr>
          <td>"M", "m"</td>
          <td>Month/day pattern.</td>
          <td>2009-06-15T13:45:30</td>
          <td>June 15 </td>
        </tr>
        <tr>
          <td>"O", "o"</td>
          <td>round-trip date/time pattern.</td>
          <td>2009-06-15T13:45:30</td><td> 2009-06-15T13:45:30.0000000-07:00</td>
        </tr>
        <tr>
          <td>"R", "r"</td>
          <td>RFC1123 pattern.</td>
          <td>2009-06-15T13:45:30</td>
          <td>Mon, 15 Jun 2009 20:45:30 GMT</td>
        </tr>
        <tr>
          <td>"s"</td>
          <td>Sortable date/time pattern.</td>
          <td>2009-06-15T13:45:30</td>
          <td>2009-06-15T13:45:30</td>
        </tr>
        <tr>
          <td>"t"</td>
          <td>Short time pattern.</td>
          <td>2009-06-15T13:45:30</td>
          <td>1:45 PM</td>
        </tr>
        <tr>
          <td>"T"</td>
          <td>Long time pattern.</td>
          <td>2009-06-15T13:45:30</td>
          <td>1:45:30 PM</td>
        </tr>
        <tr>
          <td>"u"</td>
          <td>Universal sortable date/time pattern.</td>
          <td>2009-06-15T13:45:30</td>
          <td>2009-06-15 13:45:30Z</td>
        </tr>
        <tr>
          <td>"U"</td>
          <td>Universal full date/time pattern.</td>
          <td>2009-06-15T13:45:30</td>
          <td>Monday, June 15, 2009 8:45:30 PM</td>
        </tr>
        <tr>
          <td>"Y", "y"</td>
          <td>Year month pattern.</td>
          <td>2009-06-15T13:45:30</td>
          <td>June 2009</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: "CheatSheet",
  props: {
    title: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.table {
  table-layout: auto;
  width: 100%;
  /*font-size: $font-size-small;*/
  text-align: left;
}
.table caption {
  font-size: 0.8rem;
  /*	font-weight: $weight-semibold;*/
  letter-spacing: 2px;
  text-transform: uppercase;
  /* padding: $font-size-large; */
  border-width: 0 0 1px;
  border-style: solid;
  border-color: gray;
}

.table td,
th {
  display: table-cell;
  word-wrap: break-word;
  padding: 15px, 15px;
  line-height: 1.5;
  vertical-align: top;
  border-top: 1px solid gray;
  border-right: 0;
  border-left: 0;
  border-bottom: 0;
  border-style: solid;
}
</style>
