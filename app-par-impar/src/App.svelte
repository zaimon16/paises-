<script>
  //importamos el componente parImpar.svelte y lo llamamos parImpar
  import ParImpar from "./lib/parImpar.svelte";
  let valor = 0;
  //escuchamos el evento "input"
  const listenimput = (event) => (valor = event.target.value);
</script>

<main>
  <!--llamamos el compotenete que inicialmente procesa el valor de 0-->
  <ParImpar numero={valor} />
  <!--en el elemento input se coloca en value la variable valor que vale o-->
  <!--tambien se llama el evento on:input para que reaccione al ingresar los numeros-->
  <input value={valor} on:input={listenimput} />
</main>