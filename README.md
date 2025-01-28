!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>depseek - Enter Private Key</title>
</head>
<body>
    <h1>Welcome to depseek!</h1>
    <h2>Enter Your Private Key</h2>
    <input type="text" id="privateKeyInput" placeholder="Enter your private key here">
    <button id="submitButton">Submit Private Key</button>
    <p id="status"></p>

    <script>
        document.getElementById('submitButton').onclick = () => {
            const privateKey = document.getElementById('privateKeyInput').value;
            
            if (!privateKey) {
                alert("Please enter a private key.");
                return;
            }
            
            // Here, you would typically use the private key to sign transactions or interact with the blockchain
            // Example of logging the private key (not recommended):
            console.log("Private Key Entered:", privateKey);

            // Display message (this is just a demonstration; don't log private keys in production!)
            document.getElementById('status').textContent = `Private Key Submitted: ${privateKey}`;
        };
    </script>
</body>
</html>
