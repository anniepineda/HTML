<html>
   <body style="background-color:grey;">
      <h1>Tips For Programmers</h1>
      <p style = "font-family:optima">
         Hello I want to share 7 great tips I found online for programmers.</p>
        <p style = "font-family:optima">
           <ul style="list-style-type:none;">
           <li>1. Learn by doing. Always play with the code while learning.</li>
           <li>2. Grasp the fundementals for long-term benefits</li>
        <li>3. Code by hand. It sharpens proficinecy.</li>
        <li>4. Ask for help.</li>
        <li>5. Seek out online resources.</li>
        <li>6. Dont just read the sample code. Tinker with it.</li> 
        <li>7. Take breaks when debugging.</li> 
         </ul>
</p>           
  <form name="selectForm">
  <p>
    <label for="musicTypes">Choose some music types, then click the button below:</label>
    <select id="musicTypes" name="musicTypes" multiple="multiple">
      <option selected="selected">R&B</option>
      <option>Jazz</option>
      <option>Blues</option>
      <option>New Age</option>
      <option>Classical</option>
      <option>Opera</option>
    </select>
  </p>
  <p><input id="btn" type="button" value="How many are selected?" /></p>
</form>

<script>
function howMany(selectObject) {
  let numberSelected = 0;
  for (let i = 0; i < selectObject.options.length; i++) {
    if (selectObject.options[i].selected) {
      numberSelected++;
    }
  }
  return numberSelected;
}

let btn = document.getElementById('btn');
btn.addEventListener('click', function() {
  alert('Number of options selected: ' + howMany(document.selectForm.musicTypes));
});
</script>
   </body>
</html>
