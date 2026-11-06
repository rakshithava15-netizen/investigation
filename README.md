# investigation
A very confidential birthday project
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Birthday Wishlist Bureau</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:ital,wght@0,500;0,600;0,700;1,500&display=swap');

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    background: #f9edf0;
    color: #49343c;
    font-family: 'DM Sans', sans-serif;
    min-height: 100vh;
    padding: 25px 15px;
}

.container {
    max-width: 720px;
    margin: auto;
    background: #fffaf8;
    border: 1px solid #ead4da;
    border-radius: 22px;
    padding: 35px;
    box-shadow: 0 10px 35px rgba(111, 67, 82, 0.09);
}

.small-heading {
    color: #b47b8c;
    text-transform: uppercase;
    letter-spacing: 3px;
    font-size: 11px;
    font-weight: 700;
    text-align: center;
    margin-bottom: 15px;
}

h1, h2 {
    font-family: 'Playfair Display', serif;
    text-align: center;
    color: #754b5b;
}

h1 {
    font-size: clamp(32px, 7vw, 47px);
    line-height: 1.2;
    margin-bottom: 15px;
}

h2 {
    font-size: 29px;
    margin-bottom: 12px;
}

.subtitle {
    text-align: center;
    color: #90747d;
    line-height: 1.7;
    font-size: 14px;
    margin-bottom: 25px;
}

.decor {
    text-align: center;
    font-size: 25px;
    margin: 20px 0;
}

button {
    font-family: 'DM Sans', sans-serif;
    cursor: pointer;
    border: none;
    transition: 0.2s ease;
}

.primary-btn {
    display: block;
    margin: 25px auto 0;
    padding: 14px 28px;
    border-radius: 30px;
    background: #a96f83;
    color: white;
    font-weight: 700;
    font-size: 14px;
}

.primary-btn:hover {
    background: #895366;
    transform: translateY(-2px);
}

.secondary-btn {
    padding: 12px 22px;
    border-radius: 25px;
    background: #f2e4e8;
    color: #895366;
    font-weight: 600;
}

.secondary-btn:hover {
    background: #ead2da;
}

.progress-info {
    display: flex;
    justify-content: space-between;
    font-size: 11px;
    color: #a47b88;
    margin-bottom: 8px;
    font-weight: 600;
}

.progress-bar {
    height: 6px;
    background: #f0e1e5;
    border-radius: 20px;
    overflow: hidden;
    margin-bottom: 30px;
}

.progress-fill {
    height: 100%;
    width: 0%;
    background: #b77e91;
    transition: width 0.3s ease;
}

.chapter-label {
    text-align: center;
    color: #b17b8b;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-size: 11px;
    font-weight: 700;
    margin-bottom: 12px;
}

.question {
    margin: 25px 0;
}

.question-title {
    font-weight: 700;
    font-size: 15px;
    margin-bottom: 12px;
    line-height: 1.5;
}

.options {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 9px;
}

.option {
    background: #fff4f5;
    border: 1px solid #efdce1;
    border-radius: 12px;
    padding: 12px;
    color: #755663;
    font-size: 13px;
    text-align: left;
}

.option:hover {
    border-color: #bd8799;
    background: #f9e9ed;
}

.option.selected {
    background: #a96f83;
    color: white;
    border-color: #a96f83;
}

input[type="text"], textarea {
    width: 100%;
    border: 1px solid #e8d2d9;
    background: #fff7f7;
    border-radius: 12px;
    padding: 13px;
    font-family: 'DM Sans', sans-serif;
    font-size: 13px;
    color: #49343c;
    outline: none;
    resize: vertical;
}

input:focus, textarea:focus {
    border-color: #b77e91;
}

.hint {
    font-size: 11px;
    color: #a88a94;
    margin-top: 7px;
}

.navigation {
    display: flex;
    justify-content: space-between;
    gap: 12px;
    margin-top: 30px;
}

.navigation button {
    flex: 1;
}

.hidden {
    display: none !important;
}

.report {
    background: #fff4f5;
    border: 1px dashed #d6a9b7;
    padding: 22px;
    border-radius: 15px;
    margin-top: 20px;
}

.report-section {
    margin: 20px 0;
    border-bottom: 1px solid #ead7dd;
    padding-bottom: 15px;
}

.report-section h3 {
    font-family: 'Playfair Display', serif;
    color: #895366;
    font-size: 19px;
    margin-bottom: 10px;
}

.report-section p {
    font-size: 13px;
    line-height: 1.7;
    margin: 7px 0;
}

.report-section strong {
    color: #895366;
}

.footer-note {
    text-align: center;
    font-size: 11px;
    color: #ad8c96;
    margin-top: 25px;
    line-height: 1.6;
}

@media(max-width: 520px) {
    .container {
        padding: 25px 18px;
    }

    .options {
        grid-template-columns: 1fr;
    }

    h1 {
        font-size: 34px;
    }
}
</style>
</head>

<body>

<div class="container">

    <!-- WELCOME PAGE -->
    <section id="welcome">

        <div class="small-heading">An Official Birthday Investigation</div>

        <div class="decor">୨୧ ♡ ୨୧</div>

        <h1>The Birthday<br>Wishlist Bureau</h1>

        <p class="subtitle">
            Attention, birthday girl!<br>
            Your cooperation is required for a very important investigation.
            <br><br>
            We need to discover what you actually want for your birthday.
            No vague answers. No suspicious behaviour. Be honest.
        </p>

        <div class="decor">🎀 🕯️ 💌</div>

        <p class="subtitle">
            Estimated completion time: 5–7 minutes.<br>
            Confidentiality level: Extremely dramatic.
        </p>

        <button class="primary-btn" onclick="startQuiz()">
            Begin Investigation →
        </button>

        <p class="footer-note">
            The Birthday Wishlist Bureau · Established for birthday-related matters
        </p>

    </section>


    <!-- QUIZ PAGE -->
    <section id="quiz" class="hidden">

        <div class="progress-info">
            <span id="chapterProgress">Chapter 1</span>
            <span id="questionProgress">0% completed</span>
        </div>

        <div class="progress-bar">
            <div class="progress-fill" id="progressFill"></div>
        </div>

        <div id="quizContent"></div>

        <div class="navigation">
            <button class="secondary-btn" onclick="previous()">← Back</button>
            <button class="primary-btn" id="nextButton" onclick="next()">
                Next →
            </button>
        </div>

    </section>


    <!-- FINAL REPORT -->
    <section id="result" class="hidden">

        <div class="small-heading">Investigation Completed</div>

        <div class="decor">💌 ✧ 🎀</div>

        <h1>The Final Wishlist</h1>

        <p class="subtitle">
            The evidence has been collected. The birthday department
            may now begin its preparations.
        </p>

        <div class="report" id="report"></div>

        <button class="primary-btn" onclick="copyReport()">
            Copy My Wishlist
        </button>

        <p class="footer-note">
            Please send this report to the investigator.<br>
            Your answers are not automatically sent anywhere.
        </p>

    </section>

</div>


<script>

const sections = [

{
    title: "01 · General Interrogation",
    questions: [

        {
            q: "What kind of birthday gift usually makes you happiest?",
            a: [
                "Something useful",
                "Something pretty",
                "Something sentimental",
                "Something expensive",
                "Something unexpected",
                "Something I've wanted for ages"
            ]
        },

        {
            q: "Which category are you most interested in right now?",
            a: [
                "Fashion & clothing",
                "Jewellery & accessories",
                "Skincare & beauty",
                "Books & stationery",
                "Technology",
                "Room decor",
                "Bags & footwear",
                "Something else entirely"
            ]
        },

        {
            q: "Pick up to THREE categories you'd genuinely love.",
            a: [
                "Clothes",
                "Jewellery",
                "Makeup",
                "Skincare",
                "Perfume",
                "Books",
                "Bags",
                "Shoes",
                "Accessories",
                "Personalised gifts",
                "Room decor",
                "Other"
            ],
            multi: true,
            max: 3
        },

        {
            q: "Is there anything you've been wanting lately?",
            type: "text",
            hint: "It can be something small or something you've been eyeing for months."
        }

    ]
},

{
    title: "02 · Identify the Gift",
    questions: [

        {
            q: "Would you prefer something practical or something just for enjoyment?",
            a: [
                "Practical, definitely",
                "Just for enjoyment",
                "A little bit of both",
                "Depends on the gift"
            ]
        },

        {
            q: "What sort of gift would you get most excited to unwrap?",
            a: [
                "A beautiful accessory",
                "A fashion item",
                "A beauty product",
                "A personalised gift",
                "A surprise box",
                "Something completely unexpected"
            ]
        },

        {
            q: "Would you rather receive one specific thing you've asked for or a surprise?",
            a: [
                "Exactly what I asked for",
                "A complete surprise",
                "A surprise within my preferences",
                "Either is fine"
            ]
        },

        {
            q: "Name a specific item you would love to own.",
            type: "text",
            hint: "Be as specific as possible!"
        }

    ]
},

{
    title: "03 · The Aesthetic Department",
    questions: [

        {
            q: "Which aesthetic feels most like you?",
            a: [
                "Soft and feminine",
                "Vintage and romantic",
                "Minimal and classy",
                "Dark and mysterious",
                "Cute and playful",
                "Bold and glamorous",
                "Earthy and autumnal"
            ]
        },

        {
            q: "Which colours would you prefer in a gift?",
            a: [
                "Pink & blush",
                "Black & grey",
                "Brown & beige",
                "Maroon & burgundy",
                "White & cream",
                "Pastels",
                "Dark colours",
                "No preference"
            ]
        },

        {
            q: "What kind of design do you usually like?",
            a: [
                "Simple and minimal",
                "Floral and delicate",
                "Vintage-inspired",
                "Bold and statement-making",
                "Cute and detailed",
                "Elegant and timeless"
            ]
        },

        {
            q: "Are there any colours or styles you absolutely dislike?",
            type: "text",
            hint: "Tell me what to avoid."
        }

    ]
},

{
    title: "04 · Tiny Details",
    questions: [

        {
            q: "If it's jewellery, what do you usually prefer?",
            a: [
                "Gold",
                "Silver",
                "Rose gold",
                "Antique jewellery",
                "Oxidised jewellery",
                "I don't really wear jewellery"
            ]
        },

        {
            q: "If it's a bag, what kind would you like?",
            a: [
                "Shoulder bag",
                "Tote bag",
                "Sling bag",
                "Handbag",
                "Backpack",
                "Mini bag",
                "Not interested in bags"
            ]
        },

        {
            q: "If it's clothing, what would you actually wear?",
            a: [
                "Tops",
                "Dresses",
                "Traditional wear",
                "Shirts",
                "Casual wear",
                "Something formal",
                "Not interested in clothing"
            ]
        },

        {
            q: "Do you have any preferences regarding size, material or fit?",
            type: "text",
            hint: "Mention sizes or materials if relevant."
        }

    ]
},

{
    title: "05 · Sentimental Evidence",
    questions: [

        {
            q: "Would you like a personalised gift?",
            a: [
                "Yes, absolutely!",
                "Maybe, if it's tasteful",
                "No, I'd prefer something normal",
                "Depends on the personalisation"
            ]
        },

        {
            q: "Which of these would you find meaningful?",
            a: [
                "A handwritten letter",
                "A photo album",
                "A customised accessory",
                "A memory box",
                "Something handmade",
                "A gift connected to an inside joke",
                "None of these"
            ]
        },

        {
            q: "Is there a memory, character, place or thing you are especially attached to?",
            type: "text",
            hint: "Anything that could inspire a thoughtful gift."
        }

    ]
},

{
    title: "06 · The Gift Logistics",
    questions: [

        {
            q: "What would make you actually use or appreciate a gift?",
            a: [
                "Something I need",
                "Something I've always wanted",
                "Something beautiful",
                "Something unique",
                "Something I can keep forever"
            ]
        },

        {
            q: "Would you prefer a branded product or something unique and uncommon?",
            a: [
                "A well-known brand",
                "Something handmade",
                "Something uncommon",
                "No preference"
            ]
        },

        {
            q: "Are there any brands you particularly love?",
            type: "text",
            hint: "Clothing, jewellery, beauty, anything."
        },

        {
            q: "Is there a particular product you've seen online and wanted?",
            type: "text",
            hint: "Give me the exact product if possible."
        }

    ]
},

{
    title: "07 · Final Confession",
    questions: [

        {
            q: "Is there anything you definitely DON'T want as a gift?",
            type: "text",
            hint: "This is important. Save the investigator from making a mistake."
        },

        {
            q: "If you could receive absolutely anything within reason, what would it be?",
            type: "text",
            hint: "No need to be shy. This is your final confession."
        },

        {
            q: "Anything else the Birthday Wishlist Bureau should know?",
            type: "text",
            hint: "Additional details, links, hints or secret wishes..."
        }

    ]
}

];


let currentSection = 0;
let answers = {};


function startQuiz() {
    document.getElementById("welcome").classList.add("hidden");
    document.getElementById("quiz").classList.remove("hidden");
    render();
}


function render() {

    const section = sections[currentSection];

    document.getElementById("chapterProgress").innerText =
        `Chapter ${currentSection + 1} of ${sections.length}`;

    let totalQuestions = sections.reduce(
        (sum, s) => sum + s.questions.length, 0
    );

    let completedQuestions = 0;

    for (let i = 0; i < currentSection; i++) {
        completedQuestions += sections[i].questions.length;
    }

    let percentage = Math.round(
        (completedQuestions / totalQuestions) * 100
    );

    document.getElementById("questionProgress").innerText =
        percentage + "% completed";

    document.getElementById("progressFill").style.width =
        percentage + "%";


    let html = `
        <div class="chapter-label">${section.title}</div>
        <h2>${section.title.split("·")[1]}</h2>
        <p class="subtitle">Answer honestly. The investigator is watching. ♡</p>
    `;


    section.questions.forEach((question, index) => {

        let key = currentSection + "-" + index;
        let saved = answers[key];

        html += `
            <div class="question">
                <div class="question-title">
                    ${index + 1}. ${question.q}
                </div>
        `;


        if (question.type === "text") {

            html += `
                <textarea
                    rows="3"
                    placeholder="${question.hint || "Your answer..."}"
                    oninput="saveText('${key}', this.value)"
                >${saved || ""}</textarea>
            `;

        } else {

            html += `<div class="options">`;

            question.a.forEach(option => {

                let selected = question.multi
                    ? (saved || []).includes(option)
                    : saved === option;

                html += `
                    <button
                        class="option ${selected ? "selected" : ""}"
                        onclick="selectOption('${key}', '${option.replace(/'/g, "\\'")}', ${question.multi ? "true" : "false"}, ${question.max || 0})"
                    >
                        ${option}
                    </button>
                `;

            });

            html += `</div>`;

            if (question.multi) {
                html += `<p class="hint">Choose up to ${question.max} options.</p>`;
            }

        }

        html += `</div>`;

    });


    document.getElementById("quizContent").innerHTML = html;


    document.getElementById("nextButton").innerText =
        currentSection === sections.length - 1
            ? "Finish Investigation ✧"
            : "Next →";

}


function saveText(key, value) {
    answers[key] = value;
}


function selectOption(key, option, multi, max) {

    if (multi) {

        let selected = answers[key] || [];

        if (selected.includes(option)) {
            selected = selected.filter(item => item !== option);
        } else {

            if (selected.length >= max) {
                alert(`You can choose only ${max} options!`);
                return;
            }

            selected.push(option);
        }

        answers[key] = selected;

    } else {

        answers[key] = option;

    }

    render();
}


function next() {

    if (currentSection < sections.length - 1) {

        currentSection++;
        render();

    } else {

        finish();

    }

}


function previous() {

    if (currentSection > 0) {

        currentSection--;
        render();

    } else {

        document.getElementById("quiz").classList.add("hidden");
        document.getElementById("welcome").classList.remove("hidden");

    }

}


function finish() {

    document.getElementById("quiz").classList.add("hidden");
    document.getElementById("result").classList.remove("hidden");

    document.getElementById("progressFill").style.width = "100%";


    let reportHTML = `
        <div style="text-align:center; margin-bottom:20px;">
            <h2 style="font-size:24px;">The Official Birthday Wishlist</h2>
            <p style="font-size:12px; color:#a47b88;">
                Classified information · Handle with care
            </p>
        </div>
    `;


    sections.forEach((section, sectionIndex) => {

        reportHTML += `
            <div class="report-section">
                <h3>${section.title}</h3>
        `;


        section.questions.forEach((question, index) => {

            let key = sectionIndex + "-" + index;
            let answer = answers[key];

            if (answer && answer.length !== 0) {

                if (Array.isArray(answer)) {
                    answer = answer.join(", ");
                }

                reportHTML += `
                    <p>
                        <strong>${question.q}</strong><br>
                        ${answer}
                    </p>
                `;

            }

        });


        reportHTML += `</div>`;

    });


    reportHTML += `
        <p style="text-align:center; font-size:13px; color:#895366;">
            ✧ Investigation successfully completed. ✧
        </p>
    `;


    document.getElementById("report").innerHTML = reportHTML;

}


function copyReport() {

    let text = "THE OFFICIAL BIRTHDAY WISHLIST\n\n";

    sections.forEach((section, sectionIndex) => {

        text += section.title + "\n";

        section.questions.forEach((question, index) => {

            let key = sectionIndex + "-" + index;
            let answer = answers[key];

            if (answer && answer.length !== 0) {

                if (Array.isArray(answer)) {
                    answer = answer.join(", ");
                }

                text += question.q + "\n";
                text += answer + "\n\n";

            }

        });

        text += "\n";

    });


    navigator.clipboard.writeText(text)
        .then(() => alert("Wishlist copied! Send it to your investigator. 💌"))
        .catch(() => alert("Please select and copy the wishlist manually."));

}

</script>

</body>
</html>
