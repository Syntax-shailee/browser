# browser
a search bar which can redirect to any website
CODE:-
<!DOCTYPE html>
<html>
<head>
  <title>AI-Powered Browser</title>
</head>
<body>
  <!-- Browser UI -->
  <div>
    <input type="text" id="searchInput" placeholder="Enter URL or search query">
    <button onclick="redirect()">Go</button>
  </div>
  <div>
    <button onclick="voiceSearch()">Voice Search</button>
  </div>
  
  <!-- Script to handle user input and redirection -->
  <script>
    function redirect() {
      const userInput = document.getElementById('searchInput').value;
      
      // Basic validation for empty input
      if (userInput.trim() === '') {
        alert('Please enter a URL or search query.');
        return;
      }

      // Perform your AI processing here to determine the user's intent,
      // and if it's a URL, use window.location.href to redirect to it.
      // For simplicity, we'll just open a new tab with the input URL here.
      window.open(userInput, '_blank');
    }

    function voiceSearch() {
      // Implement voice recognition functionality here using
      // speech-to-text APIs or libraries to capture user's voice.
      // Process the speech input and pass it to the redirect() function.
      alert('Voice search is not implemented in this demo.');
    }
  </script>
</body>
</html>
