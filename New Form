<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Prospect Information Form</title>
    <style>
        body { font-family: Arial, sans-serif; padding: 20px; max-width: 600px; margin: 0 auto; }
        .form-group { margin-bottom: 20px; }
        label { display: block; margin-bottom: 5px; font-weight: bold; }
        input[type="text"], textarea, select {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box; /* Ensures padding doesn't affect the overall width */
        }
        textarea { resize: vertical; height: 100px; }
        button {
            background-color: #007bff;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>

    <h2>Tell Us About Your Needs</h2>
    <p>Please answer the following five questions so we can best tailor our response to you.</p>

    <form action="/submit-prospect-form" method="POST">

        <div class="form-group">
            <label for="name">Your Name *</label>
            <input type="text" id="name" name="name" required>
        </div>
        <div class="form-group">
            <label for="email">Work Email *</label>
            <input type="email" id="email" name="email" required>
        </div>

        <hr>

        <div class="form-group">
            <label for="challenge">1. What is the **primary challenge or goal** you are hoping to address by exploring solutions like ours? *</label>
            <textarea id="challenge" name="challenge" rows="4" required></textarea>
        </div>

        <div class="form-group">
            <label for="size">2. Which of the following best describes the **size of your team or organization** that will be using/benefiting from this solution? *</label>
            <select id="size" name="organization_size" required>
                <option value="" disabled selected>Select an option</option>
                <option value="1-10">1-10 employees</option>
                <option value="11-50">11-50 employees</option>
                <option value="51-200">51-200 employees</option>
                <option value="201+">201+ employees</option>
            </select>
        </div>

        <div class="form-group">
            <label for="timeline">3. What is your **expected timeline** for implementing a new solution? *</label>
            <select id="timeline" name="timeline" required>
                <option value="" disabled selected>Select an option</option>
                <option value="Within 1 month">Within 1 month (Urgent)</option>
                <option value="1-3 months">1-3 months</option>
                <option value="3-6 months">3-6 months</option>
                <option value="Researching">Just researching right now</option>
            </select>
        </div>

        <div class="form-group">
            <label for="decision_maker">4. Who is the **primary decision-maker** for this type of purchase, and what is their role? (e.g., Jane Doe / VP of Operations) *</label>
            <input type="text" id="decision_maker" name="decision_maker" required>
        </div>

        <div class="form-group">
            <label for="priority">5. What is the **most important factor** to you when evaluating a new vendor (e.g., price, specific features, support, integration)? *</label>
            <textarea id="priority" name="priority" rows="3" required></textarea>
        </div>

        <button type="submit">Submit and Get Started</button>

    </form>

    <p style="margin-top: 20px; font-size: 0.8em; color: #666;">We respect your privacy. The information you provide will only be used to contact you about your interest in our services.</p>

</body>
</html>
