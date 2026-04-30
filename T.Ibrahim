<!DOCTYPE html>
<html lang="en" dir="ltr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unit 7 English Quiz</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body { font-family: 'Segoe UI', sans-serif; background-color: #f0f4f8; }
        .quiz-card { background: white; border-radius: 1rem; box-shadow: 0 4px 20px rgba(0,0,0,0.08); }
        .question { border-bottom: 1px solid #edf2f7; padding: 1.5rem 0; }
        .question:last-child { border-bottom: none; }
        .hidden { display: none; }
        input[type="radio"]:checked + span { color: #2563eb; font-weight: bold; }
    </style>
</head>
<body class="p-4 md:p-8">

    <div class="max-w-3xl mx-auto quiz-card p-6 md:p-10">
        <!-- Start Screen -->
        <div id="start-screen" class="text-center py-10">
            <h1 class="text-3xl font-bold text-blue-800 mb-4">Unit 7 Quiz: Communication</h1>
            <p class="text-gray-600 mb-8">Please enter your information to start the exam (Total: 10 Marks)</p>
            <div class="space-y-4 max-w-sm mx-auto">
                <input type="text" id="student-name" class="w-full p-3 border rounded-lg outline-none focus:ring-2 focus:ring-blue-400" placeholder="Student Full Name">
                <input type="text" id="teacher-phone" class="w-full p-3 border rounded-lg outline-none focus:ring-2 focus:ring-green-400" placeholder="Teacher WhatsApp (e.g. 97150xxxxxxx)">
                <button onclick="initQuiz()" class="w-full bg-blue-600 text-white py-3 rounded-lg font-bold hover:bg-blue-700 transition">Start Exam</button>
            </div>
            <p class="text-xs text-gray-400 mt-6">* Note: You can only submit once.</p>
        </div>

        <!-- Quiz Screen -->
        <div id="quiz-screen" class="hidden">
            <div class="flex justify-between items-center mb-6 sticky top-0 bg-white py-2 border-b">
                <span class="font-bold text-blue-700" id="display-name"></span>
                <span class="bg-blue-100 text-blue-800 px-3 py-1 rounded-full text-sm font-bold">10 Marks</span>
            </div>

            <form id="quiz-form">
                <!-- Vocabulary (3 Marks) -->
                <div class="mb-8">
                    <h3 class="text-lg font-bold text-gray-800 mb-4 bg-gray-50 p-2 rounded">Part 1: Vocabulary</h3>
                    
                    <div class="question">
                        <p class="font-medium mb-3">1. I'm going to ________ to a podcast about technology.</p>
                        <div class="grid grid-cols-1 gap-2">
                            <label class="flex items-center space-x-3 p-2 hover:bg-gray-50 rounded cursor-pointer"><input type="radio" name="q1" value="insert"> <span class="ml-2">insert</span></label>
                            <label class="flex items-center space-x-3 p-2 hover:bg-gray-50 rounded cursor-pointer"><input type="radio" name="q1" value="listen"> <span class="ml-2">listen</span></label>
                            <label class="flex items-center space-x-3 p-2 hover:bg-gray-50 rounded cursor-pointer"><input type="radio" name="q1" value="use"> <span class="ml-2">use</span></label>
                        </div>
                    </div>

                    <div class="question">
                        <p class="font-medium mb-3">2. If I don't ________ a promise, I usually feel bad about it.</p>
                        <div class="grid grid-cols-1 gap-2">
                            <label class="flex items-center space-x-3 p-2 hover:bg-gray-50 rounded cursor-pointer"><input type="radio" name="q2" value="get"> <span class="ml-2">get</span></label>
                            <label class="flex items-center space-x-3 p-2 hover:bg-gray-50 rounded cursor-pointer"><input type="radio" name="q2" value="keep"> <span class="ml-2">keep</span></label>
                            <label class="flex items-center space-x-3 p-2 hover:bg-gray-50 rounded cursor-pointer"><input type="radio" name="q2" value="have"> <span class="ml-2">have</span></label>
                        </div>
                    </div>

                    <div class="question">
                        <p class="font-medium mb-3">3. Did you ________ an argument with anyone yesterday?</p>
                        <div class="grid grid-cols-1 gap-2">
                            <label class="flex items-center space-x-3 p-2 hover:bg-gray-50 rounded cursor-pointer"><input type="radio" name="q3" value="have"> <span class="ml-2">have</span></label>
                            <label class="flex items-center space-x-3 p-2 hover:bg-gray-50 rounded cursor-pointer"><input type="radio" name="q3" value="tell"> <span class="ml-2">tell</span></label>
                            <label class="flex items-center space-x-3 p-2 hover:bg-gray-50 rounded cursor-pointer"><input type="radio" name="q3" value="keep"> <span class="ml-2">keep</span></label>
                        </div>
                    </div>
                </div>

                <!-- Opposites (2 Marks) -->
                <div class="mb-8">
                    <h3 class="text-lg font-bold text-gray-800 mb-4 bg-gray-50 p-2 rounded">Part 2: Opposites</h3>
                    <div class="question">
                        <p class="font-medium mb-3">4. Choose the opposite: "I can't receive or ________ a message."</p>
                        <div class="flex space-x-6">
                            <label><input type="radio" name="q4" value="send"> send</label>
                            <label><input type="radio" name="q4" value="keep"> keep</label>
                        </div>
                    </div>
                    <div class="question">
                        <p class="font-medium mb-3">5. "Truth" is the opposite of ________.</p>
                        <div class="flex space-x-6">
                            <label><input type="radio" name="q5" value="secret"> secret</label>
                            <label><input type="radio" name="q5" value="lie"> lie</label>
                        </div>
                    </div>
                </div>

                <!-- Reading Timeline (5 Marks) -->
                <div class="mb-8">
                    <h3 class="text-lg font-bold text-gray-800 mb-4 bg-gray-50 p-2 rounded">Part 3: Sheku's Timeline</h3>
                    <div class="space-y-6">
                        <div class="question">
                            <p class="font-medium mb-2">6. In 1999, Sheku Kanneh-Mason was ________.</p>
                            <select name="q6" class="w-full p-2 border rounded">
                                <option value="">Select...</option>
                                <option value="born">born</option>
                                <option value="winning">winning</option>
                            </select>
                        </div>
                        <div class="question">
                            <p class="font-medium mb-2">7. He started playing the cello when he was ________.</p>
                            <select name="q7" class="w-full p-2 border rounded">
                                <option value="">Select age...</option>
                                <option value="5">five</option>
                                <option value="6">six</option>
                                <option value="9">nine</option>
                            </select>
                        </div>
                        <div class="question">
                            <p class="font-medium mb-2">8. He won the UK young musician competition in ________.</p>
                            <input type="number" name="q8" class="w-full p-2 border rounded" placeholder="Enter year...">
                        </div>
                        <div class="question">
                            <p class="font-medium mb-2">9. In 2017, he played at the ________ and television awards.</p>
                            <input type="text" name="q9" class="w-full p-2 border rounded" placeholder="Write one word...">
                        </div>
                        <div class="question">
                            <p class="font-medium mb-2">10. Millions watched him play in London in May ________.</p>
                            <input type="number" name="q10" class="w-full p-2 border rounded" placeholder="Enter year...">
                        </div>
                    </div>
                </div>

                <button type="button" onclick="submitToWhatsApp()" class="w-full bg-green-500 text-white py-4 rounded-xl font-bold text-xl hover:bg-green-600 transition shadow-lg">Submit Results</button>
            </form>
        </div>

        <!-- Finish Screen -->
        <div id="finish-screen" class="hidden text-center py-10">
            <div class="text-6xl mb-4">✅</div>
            <h2 class="text-2xl font-bold text-gray-800 mb-2">Quiz Finished!</h2>
            <p id="score-display" class="text-3xl text-blue-600 font-bold mb-4"></p>
            <p class="text-gray-500">Your results have been generated. Thank you!</p>
        </div>
    </div>

    <script>
        const STORAGE_KEY = 'unit7_quiz_final_lock';

        function initQuiz() {
            const name = document.getElementById('student-name').value;
            const phone = document.getElementById('teacher-phone').value;
            
            if (!name.trim() || !phone.trim()) {
                alert("Please enter your name and teacher's phone number!");
                return;
            }

            if (localStorage.getItem(STORAGE_KEY)) {
                alert("You have already submitted this quiz.");
                showFinish();
                return;
            }

            document.getElementById('start-screen').classList.add('hidden');
            document.getElementById('quiz-screen').classList.remove('hidden');
            document.getElementById('display-name').innerText = "Student: " + name;
            window.scrollTo(0,0);
        }

        function calculateScore() {
            const form = document.getElementById('quiz-form');
            const data = new FormData(form);
            let score = 0;

            if (data.get('q1') === 'listen') score++;
            if (data.get('q2') === 'keep') score++;
            if (data.get('q3') === 'have') score++;
            if (data.get('q4') === 'send') score++;
            if (data.get('q5') === 'lie') score++;
            if (data.get('q6') === 'born') score++;
            if (data.get('q7') === '6') score++;
            if (data.get('q8') === '2016') score++;
            if (data.get('q9')?.toLowerCase().includes('film')) score++;
            if (data.get('q10') === '2018') score++;

            return score;
        }

        function submitToWhatsApp() {
            const score = calculateScore();
            const name = document.getElementById('student-name').value;
            const phone = document.getElementById('teacher-phone').value;

            // Create Message
            const message = `*English Quiz Result (Unit 7)*%0A` +
                            `--------------------------%0A` +
                            `*Student Name:* ${name}%0A` +
                            `*Final Score:* ${score} / 10%0A` +
                            `--------------------------%0A` +
                            `Status: Submitted Successfully ✅`;

            // Open WhatsApp
            const whatsappUrl = `https://wa.me/${phone}?text=${message}`;
            window.open(whatsappUrl, '_blank');

            // Lock the quiz
            localStorage.setItem(STORAGE_KEY, score);
            showFinish(score);
        }

        function showFinish(score) {
            const savedScore = localStorage.getItem(STORAGE_KEY);
            document.getElementById('quiz-screen').classList.add('hidden');
            document.getElementById('start-screen').classList.add('hidden');
            document.getElementById('finish-screen').classList.remove('hidden');
            document.getElementById('score-display').innerText = `Score: ${savedScore} / 10`;
        }

        window.onload = () => {
            if (localStorage.getItem(STORAGE_KEY)) {
                showFinish();
            }
        };
    </script>
</body>
</html>
