1. index.html


<!DOCTYPE html>
<html>
<head>
    <title>CSS Variables</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>My Design System</h1>
    <div class="card">
        <h2>Welcome!</h2>
        <p>Learning CSS Variables.</p>
        <button>Click Me</button>
    </div>
</body>
</html>

2. style.css


:root {
    --primary: blue;
    --secondary: purple;
    --background: lightgray;
    --text: #222;
    --small: 8px;
    --medium: 16px;
    --large: 24px;
    --font-small: 14px;
    --font-large: 28px;
}
body {
    background: var(--background);
    color: var(--text);
    padding: var(--large);
    font-size: var(--font-small);
}
h1 {
    color: var(--primary);
    font-size: var(--font-large);
}
.card {
    background: white;
    padding: var(--medium);
    margin: var(--large);
    border: 2px solid var(--secondary);
}
button {
    background: var(--primary);
    color: white;
    padding: var(--small);
    border: none;
}

Testing: Change --primary: blue; to --primary: red;. Both the heading and button will change color.