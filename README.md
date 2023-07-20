# HealthMitra-Project
<!DOCTYPE html>
<html lang="en">
<head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Healthmitra</title>
    <style>
        .question-btn {
            font-weight: bold;
            float: left;
            cursor: pointer;
            margin-bottom: 2px;
            width: 30%;
            background-color: #ccc;
            color: #333;
        }
    
        .answer {
            display: none;
            position: absolute;
            width: 60%;
            right: 10%;
            background-color: burlywood;
            font-size: medium;
            margin-bottom: 10px;
        }
    
        @media (max-width: 768px) {
            .column {
                flex-direction: row;
                margin-left: 0;
            }
        }
    </style>
</head>
<body>
    <button class="question-btn" onclick="toggleAnswer('answer0')">Script</button>
    <div class="answer" id="answer0">
        <p><h3>Start :</h3>Hello Sir/Madam,.. Good Morning
            Sir you had enquired for a health plan. What type of health plan you are looking for</p>
        <p><h3>Intro :</h3>Sir/Maam I am (name of the agent) from HealthMitra. this call is regarding Health plan,
            <p>Can I take a few moments for you to help yourself or someone needy having heavy health
                expenses.</p>
            <p>This health plan helps to get discounts on doctor fee and other medical expenses and can
                reduce overall medical expenses by 30-50%</p>
            <p>Are you looking health plan for yourself and your family?</p>
            <p><h3>If yes :</h3>Sir Before I tell you the plan and benefits I would like to known for whom you want to take the
                plan /Self/Family/Couple</p>
            <p><h3>Information request from customer :</h3>
            <ul type="square">
                <li>Age of the customer.</li>
                <li>Numbers of family member.</li>
                <li>PED (Pre Existing Disease) Confirm.</li>
                <li>House hold income.</li>
                <li>Any existing health policy.</li>
                <li>last year OPD expenses. (Out Patient Dept)</li>
            </ul>
        </p>
    </div>
    <button class="question-btn" onclick="toggleAnswer('response1')">Benifits of HealthMitra</button>
    <div class="answer" id="response1">
        <ul type="square">
            <li>We have plans in which we are covering your OPD expenses from day 1 that means
                your
                medicine bills, doctor fee, and lab test
                We have discounts on lab tests and medicines which are generally 5 to 10% more than other
                discounting companies. </li>
            <li>Waiting Period:We don’t have any waiting period. Immediately after you buy the plan from us, you
                get an E-card
                which you can use it immediately.</li>
            <li>No Capping: Sir/Maam, There is no capping on how much of total discount you get.</li>
            <li>No Exclusions: No exclusion. One can use this discount for pre-existing diseases too.</li>
        </ul>
    </div>
    <button class="question-btn" onclick="toggleAnswer('answer15')">Product type</button>
    <div class="answer" id="answer15">
        <p>Sir plz come over on the website so i can assist you how you can avail our services
            through the website.</p>
        <p>Select the plan click on buy now option and fill your details and select your
            payment mode</p>
    </div>
    <button class="question-btn" onclick="toggleAnswer('answer16')">After payment</button>
    <div class="answer" id="answer16">
        <p>Sir/Madam once your payment part is done you will receive a mail from Healthmitra in which your
            login id will be there once you login
            you have to upload your documents (Aadhar card and Pancard).</p>
        <p>After that, your plan will activate automatically.</p>
    </div>
    <div class="column">
        <div>
            <div class="faq-container">
                <button class="question-btn" onclick="toggleAnswer('answer1')">Where can I
                    get HealthMitra
                    Services like Lab tests and
                    medicines?
                </button>
                <div class="answer" id="answer1"> You can avail services
                    via ANY in-network
                    partner on the
                    HealthMitra mobile app. HealthMitra has a presence in
                    over
                    300 cities with a network of over 1000+ labs, hospitals,
                    Eyecare, Dental, pharmacy partners and more.
                </div>
                <br><br>

                <!-- Rest of the buttons and answers are not shown for brevity -->

                <script>
                    function toggleAnswer(answerId) {
                        const answerElement = document.getElementById(answerId);
                        if (answerElement.style.display === 'none') {
                            answerElement.style.display = 'block';
                        } else {
                            answerElement.style.display = 'none';
                        }
                    }
                </script>
            </div>
        </div>
    </div>
</body>
</html>
