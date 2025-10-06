<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Digital Readiness Assessment Quiz</title>
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom styles for hidden steps */
        .step {
            display: none;
            animation: fadeIn 0.4s ease-out;
        }
        .step.active {
            display: block;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        /* Style for radio button containers */
        .radio-option {
            transition: all 0.2s ease;
        }
        /* Visually style selected radio buttons */
        input[type="radio"]:checked + span {
            border-color: #3b82f6; /* Blue-500 */
            background-color: #eff6ff; /* Blue-50 */
            box-shadow: 0 0 0 2px #93c5fd; /* Blue-300 ring */
        }
    </style>
</head>
<body class="bg-gray-50 flex items-center justify-center min-h-screen p-4">

    <!-- Quiz Container -->
    <div class="bg-white p-6 md:p-10 rounded-xl shadow-2xl w-full max-w-lg">
        <h1 class="text-3xl font-extrabold text-gray-900 mb-6 text-center">
            Digital Readiness Assessment
        </h1>
        <p class="text-center text-sm text-gray-500 mb-8">
            Answer two quick questions to see your maturity score.
        </p>

        <form id="prospectQuiz">

            <!-- QUIZ STEP 1: Digital Infrastructure Maturity -->
            <div class="step active" id="step1">
                <h2 class="text-xl font-semibold text-gray-800 mb-4">
                    1. How would you rate your current <span class="text-blue-600">Digital Infrastructure Maturity</span>?
                </h2>
                
                <div class="space-y-4">
                    <label class="radio-option block">
                        <input type="radio" name="q1_maturity" value="Basic/Legacy" class="hidden" required>
                        <span class="block p-4 border border-gray-200 rounded-lg cursor-pointer hover:border-blue-400">
                            <span class="font-medium text-gray-700">Basic/Legacy</span>
                            <span class="block text-sm text-gray-500">Manual processes & disparate systems.</span>
                        </span>
                    </label>
                    <label class="radio-option block">
                        <input type="radio" name="q1_maturity" value="Moderate" class="hidden">
                        <span class="block p-4 border border-gray-200 rounded-lg cursor-pointer hover:border-blue-400">
                            <span class="font-medium text-gray-700">Moderate</span>
                            <span class="block text-sm text-gray-500">Some integrated systems & early automation.</span>
                        </span>
                    </label>
                    <label class="radio-option block">
                        <input type="radio" name="q1_maturity" value="Advanced" class="hidden">
                        <span class="block p-4 border border-gray-200 rounded-lg cursor-pointer hover:border-blue-400">
                            <span class="font-medium text-gray-700">Advanced</span>
                            <span class="block text-sm text-gray-500">Fully automated, data-driven, and integrated.</span>
                        </span>
                    </label>
                </div>
                
                <div class="mt-8 flex justify-end">
                    <button type="button" onclick="nextStep(2)" 
                            class="bg-blue-600 text-white px-6 py-2 rounded-lg font-semibold hover:bg-blue-700 transition duration-200 shadow-md">
                        Next Question &rarr;
                    </button>
                </div>
            </div>

            <!-- QUIZ STEP 2: Goal for Transformation -->
            <div class="step" id="step2">
                <h2 class="text-xl font-semibold text-gray-800 mb-4">
                    2. What is your primary <span class="text-blue-600">Goal for Digital Transformation</span> in the next 12 months?
                </h2>
                
                <div class="space-y-4">
                    <label class="radio-option block">
                        <input type="radio" name="q2_goal" value="Efficiency" class="hidden" required>
                        <span class="block p-4 border border-gray-200 rounded-lg cursor-pointer hover:border-blue-400">
                            <span class="font-medium text-gray-700">Operational Efficiency</span>
                            <span class="block text-sm text-gray-500">Streamline workflows and reduce errors.</span>
                        </span>
                    </label>
                    <label class="radio-option block">
                        <input type="radio" name="q2_goal" value="Growth" class="hidden">
                        <span class="block p-4 border border-gray-200 rounded-lg cursor-pointer hover:border-blue-400">
                            <span class="font-medium text-gray-700">Revenue Growth</span>
                            <span class="block text-sm text-gray-500">Expand market share and service offerings.</span>
                        </span>
                    </label>
                    <label class="radio-option block">
                        <input type="radio" name="q2_goal" value="Cost_Reduction" class="hidden">
                        <span class="block p-4 border border-gray-200 rounded-lg cursor-pointer hover:border-blue-400">
                            <span class="font-medium text-gray-700">Cost Reduction</span>
                            <span class="block text-sm text-gray-500">Minimize overheads and optimize spending.</span>
                        </span>
                    </label>
                </div>
                
                <div class="mt-8 flex justify-between items-center">
                    <button type="button" onclick="prevStep(1)" 
                            class="text-gray-600 px-4 py-2 rounded-lg font-semibold hover:bg-gray-100 transition duration-200">
                        &larr; Previous
                    </button>
                    <button type="button" onclick="nextStep(3)" 
                            class="bg-blue-600 text-white px-6 py-2 rounded-lg font-semibold hover:bg-blue-700 transition duration-200 shadow-md">
                        Get Your Report &rarr;
                    </button>
                </div>
            </div>

            <!-- FINAL STEP: Lead Generation Form -->
            <div class="step" id="step3">
                <h2 class="text-xl font-semibold text-gray-800 mb-4 text-center">
                    ✅ Final Step: Get Your Personalized Report
                </h2>
                <p class="text-gray-600 mb-6 text-center">
                    Enter your details below to receive your results PDF and schedule a free consultation.
                </p>
                
                <div class="space-y-4">
                    <div>
                        <label for="name" class="block text-sm font-medium text-gray-700 mb-1">Full Name</label>
                        <input type="text" id="name" name="name" required 
                               class="w-full p-3 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500" 
                               placeholder="John Doe">
                    </div>
                    <div>
                        <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Work Email</label>
                        <input type="email" id="email" name="email" required 
                               class="w-full p-3 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500" 
                               placeholder="john.doe@company.com">
                    </div>
                </div>
                
                <div class="mt-8 flex justify-between items-center">
                    <button type="button" onclick="prevStep(2)" 
                            class="text-gray-600 px-4 py-2 rounded-lg font-semibold hover:bg-gray-100 transition duration-200">
                        &larr; Previous
                    </button>
                    <button type="submit" id="submitBtn" 
                            class="bg-green-600 text-white px-6 py-2 rounded-lg font-semibold hover:bg-green-700 transition duration-200 shadow-lg">
                        Download Report & Schedule
                    </button>
                </div>
                <div id="loadingMessage" class="hidden mt-4 text-center text-blue-600 font-medium">
                    Sending data... Please wait.
                </div>
            </div>

            <!-- THANK YOU STEP (Hidden until successful submission) -->
            <div class="step" id="thankyou">
                <div class="text-center p-6 bg-blue-50 rounded-lg">
                    <div class="text-5xl mb-4">🎉</div>
                    <h2 class="text-2xl font-bold text-gray-800 mb-3">Submission Complete!</h2>
                    <p class="text-gray-600">
                        Your personalized assessment report is being sent to your email. 
                        We will contact you shortly to schedule your free strategy session.
                    </p>
                </div>
            </div>

        </form>
        
    </div>

    <script>
        // --- Form Logic ---
        let currentStep = 1;
        const totalSteps = 3; 

        // Function to update the step display and ensure form validation
        function updateSteps() {
            // Hide all steps
            for (let i = 1; i <= totalSteps; i++) {
                const step = document.getElementById(`step${i}`);
                if (step) {
                    step.classList.remove('active');
                }
            }
            document.getElementById('thankyou').classList.remove('active');

            // Show the current step
            const activeStep = document.getElementById(`step${currentStep}`);
            if (activeStep) {
                activeStep.classList.add('active');
            }
        }

        // Function to navigate to the next step
        function nextStep(stepNumber) {
            const currentStepDiv = document.getElementById(`step${currentStep}`);
            
            // Validation check (only applies to radio steps 1 and 2)
            if (currentStepDiv) {
                const requiredInputs = currentStepDiv.querySelectorAll('input[type="radio"]:required');
                
                if (requiredInputs.length > 0) {
                    const radioGroupName = requiredInputs[0].name;
                    // Check if any radio button in the current group is checked
                    const isChecked = document.querySelector(`input[name="${radioGroupName}"]:checked`);
                    
                    if (!isChecked) {
                        // Use a custom message box instead of alert()
                        showMessageBox("Please select an option to continue.", "error");
                        return; // Stop navigation
                    }
                }
            }
            
            // For the final step (Lead Gen), it's handled by the submit listener
            if (stepNumber <= totalSteps) {
                currentStep = stepNumber;
                updateSteps();
            }
        }

        // Function to navigate to the previous step
        function prevStep(stepNumber) {
            currentStep = stepNumber;
            updateSteps();
        }

        // --- Custom Message Box Function (instead of alert) ---
        function showMessageBox(message, type = 'info') {
            let container = document.getElementById('messageBoxContainer');
            if (!container) {
                container = document.createElement('div');
                container.id = 'messageBoxContainer';
                container.className = 'fixed top-0 left-0 right-0 z-50 p-4 transition-transform duration-300 transform translate-y-0';
                document.body.appendChild(container);
            }

            const box = document.createElement('div');
            let color = 'bg-blue-500';
            if (type === 'error') color = 'bg-red-500';

            box.className = `${color} text-white p-3 rounded-lg shadow-xl text-center mx-auto max-w-sm`;
            box.textContent = message;
            container.innerHTML = ''; // Clear previous messages
            container.appendChild(box);

            setTimeout(() => {
                container.innerHTML = '';
            }, 3000);
        }

        // --- FORM SUBMISSION HANDLER ---
        document.getElementById('prospectQuiz').addEventListener('submit', function(e) {
            e.preventDefault();

            // The URL for your Google Apps Script Web App 
            // !!! REPLACE THIS WITH YOUR DEPLOYED WEB APP URL !!!
            const GAS_URL = "YOUR_DEPLOYED_WEB_APP_URL_HERE"; 
            
            const submitBtn = document.getElementById('submitBtn');
            const loadingMessage = document.getElementById('loadingMessage');
            
            submitBtn.disabled = true;
            loadingMessage.classList.remove('hidden');

            const form = e.target;
            const formData = new FormData(form);

            // Structure the data to match your Google Sheet columns (Timestamp, name, email, q1_maturity, q2_goal)
            const submissionData = {
                name: formData.get('name'),
                email: formData.get('email'),
                q1_maturity: formData.get('q1_maturity'),
                q2_goal: formData.get('q2_goal')
            };

            // Prepare data for Google Apps Script (GAS requires URL-encoded format)
            const urlEncodedData = new URLSearchParams(submissionData).toString();

            // Function for exponential backoff retry logic
            const maxRetries = 3;
            const initialDelay = 1000; // 1 second

            async function submitWithRetry(retryCount = 0) {
                try {
                    const response = await fetch(GAS_URL, {
                        method: 'POST',
                        headers: {
                            'Content-Type': 'application/x-www-form-urlencoded' 
                        },
                        body: urlEncodedData
                    });

                    if (!response.ok) {
                        throw new Error(`HTTP error! status: ${response.status}`);
                    }
                    
                    const result = await response.json(); 

                    if (result.result === 'success') {
                        // Success: Show the thank you screen
                        document.getElementById(`step${currentStep}`).classList.remove('active');
                        document.getElementById('thankyou').classList.add('active');
                        loadingMessage.classList.add('hidden');
                        submitBtn.disabled = false;
                    } else {
                        // GAS returned success=fail
                        throw new Error("GAS reported failure: " + result.message);
                    }

                } catch (error) {
                    if (retryCount < maxRetries) {
                        const delay = initialDelay * Math.pow(2, retryCount);
                        await new Promise(resolve => setTimeout(resolve, delay));
                        // console.log(`Retrying submission... Attempt ${retryCount + 2}`);
                        await submitWithRetry(retryCount + 1);
                    } else {
                        // Final failure: Re-enable button and show error
                        // console.error('Final submission error:', error);
                        submitBtn.disabled = false;
                        loadingMessage.classList.add('hidden');
                        showMessageBox("Submission failed after multiple retries. Check console or try again.", "error");
                    }
                }
            }

            submitWithRetry();
        });

        // Initialize the form to show the first step
        document.addEventListener('DOMContentLoaded', updateSteps);
    </script>
</body>
</html>
