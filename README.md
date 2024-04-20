<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script >
   // This function should return an array of names
function getNames() {
  // Get the array of names
  const names = ['joe', 'Bob', 'Jill', 'Sara', 'james'];

  // Map the array of names to an array of objects
  const namesWithGreetings = names.map(name => {
    // Determine the greeting based on whether the name starts with a letter j or J
    const greeting = name.charAt(0).toLowerCase() === 'j'? 'Goodbye' : 'Hello';

    // Return an object with the name and greeting properties
    return { name, greeting };
  });

  // Return the array of objects
  return namesWithGreetings;
}

module.exports = getNames;
    </script>
</body>
</html>
