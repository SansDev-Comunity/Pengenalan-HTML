# HTML 5 Drag

```
<!DOCTYPE html>
	<head>
		<title>Drag and Drop</title>		
	</head>
	<body>	
		<form>
			<input type="file" id="input" name="input_file"/>			
		</form>
		

		<div id="dropbox">
		  <img width="300px" id="image" src="drop.png"/>
		</div>

		<script type="text/javascript">
			let dropbox;

			dropbox = document.getElementById("dropbox");
			dropbox.addEventListener("dragenter", dragenter, false);
			dropbox.addEventListener("dragover", dragover, false);
			dropbox.addEventListener("drop", drop, false);
		
			function dragenter(e) {
			  e.stopPropagation();
			  e.preventDefault();
			}

			function dragover(e) {
			  e.stopPropagation();
			  e.preventDefault();			  
			}

			function drop(e) {
			  e.stopPropagation();
			  e.preventDefault();

			  const dt = e.dataTransfer;
			  const files = dt.files;

			  document.getElementById("input").files = files;
			}
		</script>
	</body>
</html>
```


![image]()
