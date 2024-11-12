# leur-et-leurs
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exercices - Leur vs Leurs</title>
    <style>
        .correct { color: green; }
        .incorrect { color: red; }
        .feedback { margin-top: 5px; }
    </style>
    <script>
        function verifier() {
            let reponsesCorrectes = ["leur", "leurs", "leur", "leur", "leurs", "leur", "leurs", "leur", "leur", "leurs", "leurs", "leur", "leur", "leurs", "leur", "leurs", "leur", "leurs", "leur", "leurs"];
            let score = 0;

            for (let i = 0; i < reponsesCorrectes.length; i++) {
                let userInput = document.getElementById('reponse' + (i + 1)).value.trim().toLowerCase();
                let feedback = document.getElementById('feedback' + (i + 1));

                if (userInput === reponsesCorrectes[i]) {
                    feedback.innerText = "✅ Correct";
                    feedback.className = "correct feedback";
                    score++;
                } else {
                    feedback.innerText = `❌ Incorrect. La bonne réponse est "${reponsesCorrectes[i]}". Rappel : "leur" est un pronom ou un adjectif possessif singulier, tandis que "leurs" est un adjectif possessif pluriel.`;
                    feedback.className = "incorrect feedback";
                }
            }

            document.getElementById('score').innerText = `Votre score : ${score}/${reponsesCorrectes.length}`;
        }
    </script>
</head>
<body>
    <h2>Exercices - Complétez avec "leur" ou "leurs"</h2>

    <p><strong>Règle :</strong> "Leur" peut être un pronom ou un adjectif possessif singulier qui signifie "à eux/elles" (ex : Je leur ai parlé) ou qui désigne la possession d'un seul objet (ex : leur maison). "Leurs" est un adjectif possessif qui s'emploie pour indiquer la possession de plusieurs objets par plusieurs personnes (ex : leurs livres).</p>

    <form>
        <ol>
            <li>Ils ont apporté ___ chien au parc. <input type="text" id="reponse1"> <span id="feedback1"></span></li>
            <li>Les enfants ont rangé ___ jouets. <input type="text" id="reponse2"> <span id="feedback2"></span></li>
            <li>J'ai donné ___ opinion à chacun d'entre eux. <input type="text" id="reponse3"> <span id="feedback3"></span></li>
            <li>Elle va leur montrer ___ maison. <input type="text" id="reponse4"> <span id="feedback4"></span></li>
            <li>Ils ont préparé ___ affaires pour le voyage. <input type="text" id="reponse5"> <span id="feedback5"></span></li>
            <li>Je vais ___ demander de venir. <input type="text" id="reponse6"> <span id="feedback6"></span></li>
            <li>Les enfants ont perdu ___ chaussures. <input type="text" id="reponse7"> <span id="feedback7"></span></li>
            <li>Il prête souvent ___ voiture à ses amis. <input type="text" id="reponse8"> <span id="feedback8"></span></li>
            <li>Elle va parler à ___ professeur demain. <input type="text" id="reponse9"> <span id="feedback9"></span></li>
            <li>Les parents ont lavé ___ voitures. <input type="text" id="reponse10"> <span id="feedback10"></span></li>
            <li>Ils ont oublié ___ cahiers à l'école. <input type="text" id="reponse11"> <span id="feedback11"></span></li>
            <li>Je vais ___ donner un conseil. <input type="text" id="reponse12"> <span id="feedback12"></span></li>
            <li>Je leur ai parlé de ___ problème. <input type="text" id="reponse13"> <span id="feedback13"></span></li>
            <li>Ils ont perdu ___ clés. <input type="text" id="reponse14"> <span id="feedback14"></span></li>
            <li>Il faut que je ___ dise la vérité. <input type="text" id="reponse15"> <span id="feedback15"></span></li>
            <li>Les élèves ont fini ___ devoirs. <input type="text" id="reponse16"> <span id="feedback16"></span></li>
            <li>Je vais ___ prêter mon stylo. <input type="text" id="reponse17"> <span id="feedback17"></span></li>
            <li>Ils ont perdu ___ jouets dans le parc. <input type="text" id="reponse18"> <span id="feedback18"></span></li>
            <li>Elle va leur montrer ___ jardin. <input type="text" id="reponse19"> <span id="feedback19"></span></li>
            <li>Les enfants ont pris ___ livres. <input type="text" id="reponse20"> <span id="feedback20"></span></li>
        </ol>

        <button type="button" onclick="verifier()">Vérifier</button>
    </form>

    <p id="score"></p>
</body>
</html>
