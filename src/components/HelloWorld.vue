<template>
  <div class="hello container">
    <h2 class="text-center m-4cd ">Tabla</h2>
    <table class="table table-dark">
  <thead>
    <tr>
      <th>#</th>
      <th>Nombre</th>
      <th>Apellido</th>
      <th>Dirección</th>
      <th>Ciudad</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="(user, index) in usuarios" :key="index">
      <th>{{user.id}}</th>
      <td>{{user.name}}</td>
      <td>{{user.lastname}}</td>
      <td>{{user.address}}</td>
      <td>{{user.city}}</td>
    </tr>


  </tbody>
</table>
    
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      usuarios: [
        {id: 1, name: 'Erik', lastname: 'Klein', address: 'Roosevelt Causeway', city: 'South Olen'},
        {id: 2, name: 'Cathryn', lastname: 'Heathcote', address: 'Ernser Gateway', city: 'Winstonville'},
        {id: 3, name: 'Anika', lastname: 'Muller', address: 'Jacobson Center', city: 'Weberhaven'},
        {id: 4, name: 'Eliezer', lastname: 'Kub', address: 'Abernathy Inlet', city: 'Noblefort'},
        {id: 5, name: 'Raegan', lastname: 'Bayer', address: 'Rudy Causeway', city: 'Dietrichton'},
        {id: 6, name: 'Margarita', lastname: 'Cronin', address: 'Deven Island', city: 'East Camden'},
        {id: 7, name: 'Caleb', lastname: 'Bergstrom', address: 'Maximillian Harbors', city: 'Gerlachbury'},
        {id: 8, name: 'Samantha', lastname: 'Schinner', address: 'Bechtelar Lane', city: 'Prohaskamouth'},
        {id: 9, name: 'Anabelle', lastname: 'Cruickshank', address: 'Collins Walks', city: 'Rueckerside'},
        {id: 10, name: 'Dedric', lastname: 'Abshire', address: 'Schmeler Islands', city: 'Streichfurt'},
      ]

    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

