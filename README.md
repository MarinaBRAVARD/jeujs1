# jeujs1
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form action="#">
        Essayez de deviner le chiffre: <input type="text" name="valeur" id="valeur">
        <input type="button" onclick="resultat()" Value="Entrée">
    </form>
    <div id="reponse"></div>
</body>
<script>
    let chiffre=Math.floor(Math.random()*11)+1;
    function resultat(){
        let valeur=parseInt(document.getElementById("valeur").value);
        switch(true){
            case valeur<chiffre:
                document.getElementById("reponse").innerHTML=`Trop petit !!`;
                break;
            case valeur>chiffre:
                document.getElementById("reponse").innerHTML=`Trop grand !!`;
                break;
            case valeur===chiffre:
                document.getElementById("reponse").innerHTML=`Gagné !!`;
                break;
        }
    }
</script>
</html>
