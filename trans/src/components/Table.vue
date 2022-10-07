<template>
  <div>
    <table>
  <caption>Rates</caption>
  <thead>
    <tr>
      <th scope="col">Departure</th>
      <th scope="col">Arrival</th>
      <th scope="col">Freight</th>
      <th scope="col">Price</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>New York</td>
      <td>Shanghai</td>
      <td>40ft</td>
      <td>$4000</td>
    </tr>
    <tr>
      <td>Los Angeles</td>
      <td>Shanghai</td>
      <td>40ft</td>
      <td>$3500</td>
    </tr>
    <tr>
      <td>New York</td>
      <td>London</td>
      <td>40ft</td>
      <td>$2200</td>
    </tr>
    <tr>
      <td>Le Havre</td>
      <td>Conakry</td>
      <td>40ft</td>
      <td>$1600</td>
    </tr>
    <tr>
      <td>Amsterdam</td>
      <td>Lagos</td>
      <td>40ft</td>
      <td>$2600</td>
    </tr>
    <tr>
      <td>New York</td>
      <td>Beijin</td>
      <td>20ft</td>
      <td>$3650</td>
    </tr>
    <tr>
      <td>Los Angeles</td>
      <td>Shanghai</td>
      <td>20ft</td>
      <td>$3100</td>
    </tr>
    <tr>
      <td>Lagos</td>
      <td>New York</td>
      <td>20ft</td>
      <td>$1985</td>
    </tr>
  </tbody>
</table>
  </div>
</template>

<script>
export default {
name:'Table'
}
</script>

<style>
table {
  border: 1px solid #ccc;
  border-collapse: collapse;
  margin: 0;
  padding: 0;
  table-layout: fixed;
  width: 100%;
  color:black;
}

table tr {
  background-color: #f8f8f8;
  border: 1px solid #ddd;
  padding: .35em;
}

table th,
table td {
  padding: .625em;
  text-align: center;
}
caption{
  font-size: 40px;
  padding: 10px;
}
</style>