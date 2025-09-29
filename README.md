<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Compound Interest Calculator</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="calculator">
        <h2>Compound Interest Calculator</h2>
        <form id="ci-form" onsubmit="event.preventDefault(); calculateCompoundInterest();">
            <label>
                Principal Amount:
                <input type="number" id="principal" min="0" step="0.01" required>
            </label>
            <label>
                Annual Interest Rate (%):
                <input type="number" id="rate" min="0" step="0.01" required>
            </label>
            <label>
                Number of Years:
                <input type="number" id="years" min="1" step="1" required>
            </label>
            <label>
                Compounding Frequency:
                <select id="frequency" required>
                    <option value="1">Yearly</option>
                    <option value="4">Quarterly</option>
                    <option value="12">Monthly</option>
                    <option value="365">Daily</option>
                </select>
            </label>
            <button type="submit">Calculate</button>
        </form>
        <div id="result" class="result"></div>
    </div>
    <script src="compound-interest.js"></script>
</body>
</html>
