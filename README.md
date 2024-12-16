<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bookmarklets</title>
</head>
<body>
    <h1>Bookmarklets</h1>
    <p>Faites glisser les liens suivants dans votre barre de favoris.</p>

    <a href="javascript:fetch('https://raw.githubusercontent.com/Dossky/test/refs/heads/main/test.json').then(e=>e.json()).then(e=>{let t=0;!function s(){let n=document.getElementById('cemantix-guess'),l=document.getElementById('cemantix-guess-btn');if(t>=e.length){alert('Tous les mots ont été testés !');return}n.value=e[t],l.disabled=!1,l.click(),t++,setTimeout(s,50)}()}).catch(e=>alert('Erreur lors du chargement de la liste de mots : '+e));" title="Bookmarklet 1">
        <button>Bookmarklet cemantix</button>
    </a>

    <br><br>

    <a href="javascript:fetch('https://raw.githubusercontent.com/Dossky/test/refs/heads/main/test.json').then(e=>e.json()).then(e=>{let t=0;!function s(){let n=document.getElementById('pedantix-guess'),l=document.getElementById('pedantix-guess-btn');if(t>=e.length){alert('Tous les mots ont été testés !');return}n.value=e[t],l.disabled=!1,l.click(),t++,setTimeout(s,50)}()}).catch(e=>alert('Erreur lors du chargement de la liste de mots : '+e));" title="Bookmarklet 2">
        <button>Bookmarklet pedantix</button>
    </a>

</body>
</html>
