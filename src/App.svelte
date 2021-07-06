<script>
let str = '',toTranslate = ''
$:{
	str = ''
	for(let i = 0; i<toTranslate.length ; i++){
		if(toTranslate[i]=='A' || toTranslate[i] == 'a'){
			if(toTranslate[i]=='A'){
				str+='B'
			}
			else{
				str += 'b'
			}
		}
		else if(toTranslate[i]=='B' || toTranslate[i] == 'b'){
			if(toTranslate[i]=='B'){
				str+='A'
			}
			else{
				str += 'a'
			}
		}
		else if(toTranslate[i]=='E' || toTranslate[i] == 'e'){
			if(toTranslate[i]=='E'){
				str+='F'
			}
			else{
				str += 'f'
			}
		}
		else if(toTranslate[i]=='F' || toTranslate[i] == 'f'){
			if(toTranslate[i]=='F'){
				str+='E'
			}
			else{
				str += 'e'
			}
		}
		else if(toTranslate[i]=='I' || toTranslate[i] == 'i'){
			if(toTranslate[i]=='I'){
				str+='J'
			}
			else{
				str += 'j'
			}
		}
		else if(toTranslate[i]=='J' || toTranslate[i] == 'j'){
			if(toTranslate[i]=='J'){
				str+='I'
			}
			else{
				str += 'i'
			}
		}
		else if(toTranslate[i]=='O' || toTranslate[i] == 'o'){
			if(toTranslate[i]=='O'){
				str+='N'
			}
			else{
				str += 'n'
			}
		}
		else if(toTranslate[i]=='N' || toTranslate[i] == 'n'){
			if(toTranslate[i]=='N'){
				str+='O'
			}
			else{
				str += 'o'
			}
		}
		else if(toTranslate[i]=='U' || toTranslate[i] == 'u'){
			if(toTranslate[i]=='U'){
				str+='V'
			}
			else{
				str += 'v'
			}
		}
		else if(toTranslate[i]=='V' || toTranslate[i] == 'v'){
			if(toTranslate[i]=='V'){
				str+='u'
			}
			else{
				str += 'u'
			}
		}
		else if(toTranslate[i]=='T' || toTranslate[i] == 't'){
			if(toTranslate[i]=='T'){
				str+='Y'
			}
			else{
				str += 'y'
			}
		}
		else if(toTranslate[i]=='Y' || toTranslate[i] == 'y'){
			if(toTranslate[i]=='Y'){
				str+='T'
			}
			else{
				str += 't'
			}
		}
		else if(toTranslate[i]=='S' || toTranslate[i] == 's'){
			if(toTranslate[i]=='S'){
				str+='D'
			}
			else{
				str += 'd'
			}
		}
		else if(toTranslate[i]=='D' || toTranslate[i] == 'd'){
			if(toTranslate[i]=='D'){
				str+='S'
			}
			else{
				str += 's'
			}
		}
		else {
			str+= toTranslate[i]
		}
	}
}
function cod(){
alert('Copied')
document.getElementById('co').select()
document.execCommand('copy')
}
</script>

<main>
	<h3>Translate</h3>
	<textarea bind:value={toTranslate}></textarea>
	<textarea id='co'>{str}</textarea>
	<button on:click={cod}>
		Copy
	</button>
</main>

<style>
	main{
		display:flex;
		flex-direction: column;
		height: 90vh;
		width:100vw;
		justify-content: center;
		align-items: center;
	}
	textarea{
		width:400px;
		min-height: 200px;
		height:auto;
	}
	#co{
		height:250px;
		width:400px;
		word-wrap: inherit;
	}
</style>
