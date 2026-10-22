
<style>
  body{background:#080809;}
  input{border-radius:50px;width:100%;padding:10px;text-align:center;margin-top:0px;margin-bottom:20px;font-size:20px;border:1px solid #846887;background:#ffffff;color:white}
  #li{color:#7ed433;margin-bottom:20px;font-weight:bold;font-size:20px;font-family:times new roman}
  .carte{border-radius:10px;border:2px solid #43d113;margin:20px;padding:20px;background:dimgray;}
  img{white:20px;height:300px;margin-left:60px;border:none}
</style>
<body>
  <ul id="li"></ul>
  <img src="photo.jpg"  alt="El Widalo">
    <div class="carte">
  <input placeholder="nom du produit">
  <input placeholder="prix du priduit">
  <input placeholder="image du produit">
    </div>
  <script>
    let li = document.getElementById("li");
    let phrase = ["Je Fais un simple test"];
    let m = 0;
    let l = 0;
    function assayer() {
      let rel = phrase[m];
      li.innerText = rel.substring(0,l) + " | " + l++;
      if (l > rel.length) {
        l = 0;
      }
    }
    setInterval(assayer,200);
  </script>
</body>