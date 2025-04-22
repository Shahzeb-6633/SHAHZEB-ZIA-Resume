# Shahzeb-Zia-Resume
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Shahzeb Zia | Resume</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            display: ["Poppins", "sans-serif"],
            body: ["Inter", "sans-serif"]
          },
          colors: {
            primary: '#4f46e5',
            secondary: '#9333ea',
          }
        }
      }
    };
  </script>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&family=Poppins:wght@600&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Inter', sans-serif;
    }
  </style>
</head>
<body class="bg-gradient-to-br from-gray-100 to-purple-100 dark:from-gray-900 dark:to-gray-800 text-gray-800 dark:text-white transition-colors duration-300">

  <!-- Header -->
  <header class="text-center py-8 bg-gradient-to-r from-purple-500 via-indigo-500 to-blue-500 text-white">
      <!-- Profile Image -->
  <img 
    src="DSC. COPY.jpg" 
    alt="Shahzeb Zia" 
    class="mx-auto rounded-full w-32 h-32 sm:w-40 sm:h-40 border-4 border-white shadow-lg mb-4 transition-transform duration-300 hover:scale-105"
  >

  <!-- Name & Title -->

    <h1 class="text-4xl font-display font-bold">Shahzeb Zia</h1>
    <p class="text-lg mt-1">Aspiring Entrepreneur | Focused on Studies & Innovation</p>
    <p class="text-sm mt-2">Student at IIM Bangalore</p>
  </header>

  <!-- Dark/Light Toggle -->
  <div class="flex justify-end px-6 mt-4">
    <button onclick="toggleTheme()" class="bg-gray-200 dark:bg-gray-700 px-4 py-2 rounded-full shadow-md text-sm">
      Toggle Theme
    </button>
  </div>

  <!-- Tab Navigation -->
  <nav class="flex justify-center mt-4 space-x-4">
    <button onclick="showTab('about')" class="tab-btn px-4 py-2 bg-primary text-white rounded-full">About Me</button>
    <button onclick="showTab('skills')" class="tab-btn px-4 py-2 bg-primary text-white rounded-full">Skills</button>
    <button onclick="showTab('education')" class="tab-btn px-4 py-2 bg-primary text-white rounded-full">Education</button>
    <button onclick="showTab('contact')" class="tab-btn px-4 py-2 bg-primary text-white rounded-full">Contact</button>
  </nav>

  <!-- Tabs Content -->
  <section class="mt-8 max-w-4xl mx-auto px-6 space-y-6">

    <div id="about" class="tab-content">
      <h2 class="text-2xl font-bold mb-2">🧠 About Me</h2>
      <p>
        I’m a motivated <strong>BBA (Digital Business & Entrepreneurship)</strong> student at IIM Bangalore, also pursuing a <strong>B.Com</strong> at Government Autonomous College, Rourkela.
        I have a deep interest in accounting and a strong passion for idea generation, leadership, and creative problem-solving. I aim to grow into a respectful, successful, and financially strong individual through continuous learning and innovation.
      </p>
    </div>

    <div id="skills" class="tab-content hidden">
      <h2 class="text-2xl font-bold mb-2">🛠 Skills</h2>
      <ul class="list-disc list-inside space-y-1">
        <li>Accounting</li>
        <li>FinTech</li>
        <li>Computer & Technology</li>
        <li>Management</li>
        <li>Generative AI</li>
        <li>Business Idea Generation</li>
      </ul>
    </div>

    <div id="education" class="tab-content hidden">
      <h2 class="text-2xl font-bold mb-2">🎓 Education</h2>
      <ul class="space-y-2">
        <li><strong>BBA (Digital Business & Entrepreneurship)</strong> – IIM Bangalore (currently pursuing)</li>
        <li><strong>B.COM</strong> – Government Autonomous College, Rourkela (currently pursuing)</li>
        <li><strong>10th & 12th</strong> – Deepika English Medium School, Rourkela (completed)</li>
      </ul>
    </div>

    <div id="contact" class="tab-content hidden">
      <h2 class="text-2xl font-bold mb-2">📬 Contact Info</h2>
      <p>Email: <a href="mailto:shahzeb.zia24@iimb.ac.in" class="text-blue-600 dark:text-blue-400 underline">shahzeb.zia24@iimb.ac.in</a></p>
    </div>

  </section>

  <!-- Footer -->
  <footer class="text-center mt-12 py-6 bg-gray-200 dark:bg-gray-900 text-sm text-gray-700 dark:text-gray-400">
    &copy; 2025 Shahzeb Zia. All rights reserved.
  </footer>

  <!-- JavaScript -->
  <script>
    function showTab(tabId) {
      const tabs = document.querySelectorAll('.tab-content');
      tabs.forEach(tab => tab.classList.add('hidden'));
      document.getElementById(tabId).classList.remove('hidden');

      const buttons = document.querySelectorAll('.tab-btn');
      buttons.forEach(btn => btn.classList.remove('bg-secondary'));
      event.target.classList.add('bg-secondary');
    }

    function toggleTheme() {
      document.documentElement.classList.toggle('dark');
    }
  </script>

</body>
