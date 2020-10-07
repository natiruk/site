# My site

## Nothing here so far
<script>//alert('Welcome');</script> 

But, what did you expect

<script>
function calculator() {
  var expression = document.getElementById("expression").value;
  var result = document.getElementById("result");
  try { result.value = eval("with(Math){" + expression + "}"); }
  catch (e) { alert(e) }
}
</script>
<style>
  input {background: #8cf;}
</style>

<!--textarea rows="1" id="expression"> </textarea-->
<input size="18" id="expression" />
<button id="calculator" value="Eval" onclick="calculator();">Eval</button>
<input size="18" id="result" readonly/>



