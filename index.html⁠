<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Community Recognition Portal</title>
    <style>
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --accent-color: #22c55e;
            --accent-hover: #16a34a;
            --text-primary: #f8fafc;
            --text-secondary: #94a3b8;
            --border-color: #334155;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-primary);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
        }

        .container {
            background-color: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            width: 100%;
            max-width: 600px;
            padding: 32px;
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.5);
        }

        .step {
            display: none;
        }

        .step.active {
            display: block;
        }

        .badge {
            display: inline-block;
            background-color: rgba(34, 197, 94, 0.15);
            color: var(--accent-color);
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-bottom: 16px;
            text-transform: uppercase;
            letter-spacing: 0.05em;
        }

        h1 {
            font-size: 1.75rem;
            margin-bottom: 16px;
            color: var(--text-primary);
        }

        p {
            color: var(--text-secondary);
            line-height: 1.6;
            margin-bottom: 24px;
            font-size: 0.95rem;
        }

        .form-group {
            margin-bottom: 20px;
        }

        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            font-size: 0.9rem;
            color: var(--text-primary);
        }

        input[type="text"], textarea, select {
            width: 100%;
            padding: 12px;
            background-color: var(--bg-color);
            border: 1px solid var(--border-color);
            border-radius: 6px;
            color: var(--text-primary);
            font-size: 0.95rem;
            outline: none;
            transition: border-color 0.2s;
        }

        input[type="text"]:focus, textarea:focus, select:focus {
            border-color: var(--accent-color);
        }

        textarea {
            resize: vertical;
            min-height: 80px;
        }

        .toggle-container {
            display: flex;
            align-items: center;
            justify-content: space-between;
            background-color: var(--bg-color);
            padding: 16px;
            border-radius: 8px;
            border: 1px solid var(--border-color);
            margin-bottom: 24px;
        }

        .switch {
            position: relative;
            display: inline-block;
            width: 50px;
            height: 26px;
        }

        .switch input {
            opacity: 0;
            width: 0;
            height: 0;
        }

        .slider {
            position: absolute;
            cursor: pointer;
            top: 0; left: 0; right: 0; bottom: 0;
            background-color: var(--border-color);
            transition: .3s;
            border-radius: 26px;
        }

        .slider:before {
            position: absolute;
            content: "";
            height: 18px;
            width: 18px;
            left: 4px;
            bottom: 4px;
            background-color: white;
            transition: .3s;
            border-radius: 50%;
        }

        input:checked + .slider {
            background-color: var(--accent-color);
        }

        input:checked + .slider:before {
            transform: translateX(24px);
        }

        .btn {
            width: 100%;
            padding: 14px;
            background-color: var(--accent-color);
            color: #000;
            font-weight: 700;
            border: none;
            border-radius: 6px;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.2s, opacity 0.2s;
        }

        .btn:disabled {
            background-color: var(--border-color);
            color: var(--text-secondary);
            cursor: not-allowed;
            opacity: 0.6;
        }

        .btn:hover:not(:disabled) {
            background-color: var(--accent-hover);
        }

        .progress-box {
            display: none;
            margin-top: 20px;
        }

        .progress-bar-bg {
            width: 100%;
            height: 12px;
            background-color: var(--bg-color);
            border-radius: 6px;
            overflow: hidden;
            margin-bottom: 8px;
            border: 1px solid var(--border-color);
        }

        .progress-bar-fill {
            height: 100%;
            width: 0%;
            background-color: var(--accent-color);
            transition: width 0.1s linear;
        }

        .progress-text {
            text-align: center;
            font-size: 0.85rem;
            color: var(--text-secondary);
        }
    </style>
</head>
<body>

<div class="container">
    <!-- STEP 1: CONGRATULATIONS & ACCEPTANCE -->
    <div id="step-1" class="step active">
        <span class="badge">Official Notice</span>
        <h1>Congratulations!</h1>
        <p><strong>COMMUNITY RECOGNITION</strong><br><br>
        Your ongoing engagement across our official social channels, specifically on X (formerly Twitter), has been noted by our executive tracking team. We acknowledge and appreciate your positive presence and contributions within the online community.</p>
        
        <div class="toggle-container">
            <span>Accept Terms & Proceed</span>
            <label class="switch">
                <input type="checkbox" id="accept-toggle-1">
                <span class="slider"></span>
            </label>
        </div>

        <button id="next-btn-1" class="btn" disabled>Next</button>
    </div>

    <!-- STEP 2: QUESTIONNAIRE -->
    <div id="step-2" class="step">
        <span class="badge">Step 2 of 3</span>
        <h1>Community Feedback</h1>
        <p>Please answer the following questions to verify your community engagement history.</p>

        <div class="form-group">
            <label for="duration">How long have you been a fan / community member?</label>
            <select id="duration" class="survey-input">
                <option value="" disabled selected>Select duration</option>
                <option value="less-6m">Less than 6 months</option>
                <option value="6m-1y">6 months to 1 year</option>
                <option value="1y-2y">1 to 2 years</option>
                <option value="2y-plus">2+ years</option>
            </select>
        </div>

        <div class="form-group">
            <label for="project">Which of our projects caught your attention or inspired you the most?</label>
            <textarea id="project" class="survey-input" placeholder="Share your thoughts..."></textarea>
        </div>

        <div class="form-group">
            <label for="additional">What feature or update would you like to see next?</label>
            <input type="text" id="additional" class="survey-input" placeholder="Your suggestion...">
        </div>

        <div class="toggle-container">
            <span>I confirm my answers are accurate</span>
            <label class="switch">
                <input type="checkbox" id="accept-toggle-2">
                <span class="slider"></span>
            </label>
        </div>

        <button id="next-btn-2" class="btn" disabled>Next</button>
    </div>

    <!-- STEP 3: CLAIM PACKAGE -->
    <div id="step-3" class="step">
        <span class="badge">Final Step</span>
        <h1>Claim Your Package</h1>
        <p>Click below to contact our support team and receive your direct access link.</p>

        <button id="claim-btn" class="btn">Contact Support Team to Claim Package</button>

        <div id="progress-box" class="progress-box">
            <div class="progress-bar-bg">
                <div id="progress-fill" class="progress-bar-fill"></div>
            </div>
            <div id="progress-text" class="progress-text">Connecting... 0%</div>
        </div>
    </div>
</div>

<script>
    // Configurable Target URL
    const TARGET_TEAMS_LINK = "https://teams.live.com/l/invite/FEAcgWNsPMyx32lrA?v=g1";

    // Step 1 Elements
    const toggle1 = document.getElementById('accept-toggle-1');
    const nextBtn1 = document.getElementById('next-btn-1');

    // Step 2 Elements
    const toggle2 = document.getElementById('accept-toggle-2');
    const nextBtn2 = document.getElementById('next-btn-2');
    const surveyInputs = document.querySelectorAll('.survey-input');

    // Step 3 Elements
    const claimBtn = document.getElementById('claim-btn');
    const progressBox = document.getElementById('progress-box');
    const progressFill = document.getElementById('progress-fill');
    const progressText = document.getElementById('progress-text');

    // Toggle 1 state change
    toggle1.addEventListener('change', function() {
        nextBtn1.disabled = !this.checked;
    });

    nextBtn1.addEventListener('click', function() {
        document.getElementById('step-1').classList.remove('active');
        document.getElementById('step-2').classList.add('active');
    });

    // Validate Step 2 inputs and toggle
    function validateStep2() {
        let allFilled = true;
        surveyInputs.forEach(input => {
            if (!input.value.trim()) allFilled = false;
        });
        nextBtn2.disabled = !(allFilled && toggle2.checked);
    }

    surveyInputs.forEach(input => input.addEventListener('input', validateStep2));
    surveyInputs.forEach(input => input.addEventListener('change', validateStep2));
    toggle2.addEventListener('change', validateStep2);

    nextBtn2.addEventListener('click', function() {
        document.getElementById('step-2').classList.remove('active');
        document.getElementById('step-3').classList.add('active');
    });

    // Handle Claim Button and Progress Bar
    claimBtn.addEventListener('click', function() {
        claimBtn.disabled = true;
        progressBox.style.display = 'block';

        let progress = 0;
        const interval = setInterval(() => {
            progress += 2;
            progressFill.style.width = progress + '%';
            progressText.innerText = 'Redirecting to support chat... ' + progress + '%';

            if (progress >= 100) {
                clearInterval(interval);
                window.location.href = TARGET_TEAMS_LINK;
            }
        }, 30);
    });
</script>
</body>
</html>
