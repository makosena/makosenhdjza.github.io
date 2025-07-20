<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Demande de Remboursement PayPal</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
        }
        .container {
            background-color: #fff;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 500px;
        }
        h1 {
            text-align: center;
            color: #003087; /* Couleur bleue de PayPal */
            margin-bottom: 25px;
        }
        .form-group {
            margin-bottom: 18px;
        }
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: #333;
        }
        input[type="text"],
        input[type="email"],
        textarea {
            width: calc(100% - 20px);
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            font-size: 16px;
        }
        textarea {
            resize: vertical;
            min-height: 100px;
        }
        button {
            background-color: #0070BA; /* Bleu de PayPal */
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 18px;
            width: 100%;
            transition: background-color 0.3s ease;
        }
        button:hover {
            background-color: #005ea6; /* Bleu plus foncé au survol */
        }
        .note {
            font-size: 14px;
            color: #666;
            margin-top: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Demande de Remboursement PayPal</h1>
        <p class="note">Veuillez remplir le formulaire ci-dessous pour soumettre votre demande de remboursement. Les demandes sont traitées manuellement par notre équipe.</p>

        <form action="#" method="POST"> <div class="form-group">
                <label for="transactionId">ID de Transaction PayPal :</label>
                <input type="text" id="transactionId" name="transactionId" placeholder="Ex: 123ABC456DEF" required>
            </div>

            <div class="form-group">
                <label for="payerEmail">Votre adresse e-mail PayPal :</label>
                <input type="email" id="payerEmail" name="payerEmail" placeholder="votre.email@example.com" required>
            </div>

            <div class="form-group">
                <label for="amount">Montant à rembourser (Ex: 25.00) :</label>
                <input type="text" id="amount" name="amount" placeholder="Ex: 25.00" required pattern="^\d+(\.\d{1,2})?$">
            </div>

            <div class="form-group">
                <label for="currency">Devise (Ex: EUR, USD) :</label>
                <input type="text" id="currency" name="currency" placeholder="Ex: EUR" maxlength="3" required>
            </div>

            <div class="form-group">
                <label for="reason">Raison du remboursement :</label>
                <textarea id="reason" name="reason" rows="5" placeholder="Décrivez la raison de votre demande de remboursement..." required></textarea>
            </div>

            <button type="submit">Soumettre la demande</button>
        </form>

        <p class="note">
            En soumettant ce formulaire, vous acceptez nos conditions de traitement des remboursements.
            Ceci n'est pas une transaction PayPal directe. Un membre de notre équipe vous contactera.
        </p>
    </div>
</body>
</html>
