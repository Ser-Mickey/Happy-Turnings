<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday, My Love — Open When...</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Cormorant Garamond (Editorial Serif), Caveat (Handwritten), Plus Jakarta Sans (Clean UI) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@500;600;700&family=Cormorant+Garamond:ital,wght@0,500;0,600;0,700;1,500;1,600&family=Plus+Jakarta+Sans:wght@400;500;600&display=swap" rel="stylesheet">
    <!-- Canvas Confetti for Subtle Celebration Effects -->
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>

    <style>
        /* ==========================================================================
           CUSTOM VARIABLES & BRIGHT WARM-WHITE PALETTE
           ========================================================================== */
        :root {
            --bg-ivory: #FFFDF9;
            --pure-white: #FFFFFF;
            --blush-soft: #FFF1F3;
            --blush-border: #FFE4E8;
            --rose-primary: #E11D48;
            --rose-soft: #FB7185;
            --gold-foil: #D4AF37;
            --gold-light: #F3E5AB;
            --text-dark: #271C1E;
            --text-muted: #6E5A5E;
        }

        body {
            background-color: var(--bg-ivory);
            color: var(--text-dark);
            font-family: 'Plus Jakarta Sans', sans-serif;
            overflow-x: hidden;
            background-image: 
                radial-gradient(circle at 12% 10%, rgba(255, 228, 232, 0.55) 0%, transparent 42%),
                radial-gradient(circle at 88% 85%, rgba(243, 229, 171, 0.3) 0%, transparent 48%);
            min-height: 100vh;
        }

        .font-serif-editorial {
            font-family: 'Cormorant Garamond', serif;
        }

        .font-handwritten {
            font-family: 'Caveat', cursive;
        }

        /* ==========================================================================
           FLOATING AMBIENT PARTICLES CANVAS
           ========================================================================== */
        #ambient-canvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
        }

        /* ==========================================================================
           CLEAN WHITE 3D CSS ENVELOPE STYLING
           ========================================================================== */
        .envelope-wrapper {
            perspective: 1200px;
            cursor: pointer;
            transition: transform 0.35s cubic-bezier(0.22, 1, 0.36, 1);
        }

        .envelope-wrapper:hover {
            transform: translateY(-8px);
        }

        .envelope-wrapper:active {
            transform: translateY(-2px) scale(0.98);
        }

        .envelope-card {
            position: relative;
            width: 100%;
            aspect-ratio: 16 / 10.5;
            background: linear-gradient(145deg, #FFFFFF 0%, #FFF8F9 100%);
            border-radius: 16px;
            box-shadow: 
                0 12px 30px -8px rgba(225, 29, 72, 0.08),
                0 4px 12px -2px rgba(39, 28, 30, 0.04),
                inset 0 0 0 1px rgba(255, 228, 232, 0.9);
            overflow: hidden;
            transition: box-shadow 0.35s ease;
        }

        .envelope-wrapper:hover .envelope-card {
            box-shadow: 
                0 20px 38px -10px rgba(225, 29, 72, 0.14),
                0 8px 18px -4px rgba(212, 175, 55, 0.16),
                inset 0 0 0 1px rgba(212, 175, 55, 0.45);
        }

        /* Inner Letter Peek */
        .letter-peek {
            position: absolute;
            bottom: 8%;
            left: 7%;
            right: 7%;
            height: 75%;
            background: #FFFFFF;
            border-radius: 10px;
            border: 1px solid rgba(212, 175, 55, 0.2);
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
            transition: transform 0.55s cubic-bezier(0.34, 1.56, 0.64, 1);
            z-index: 1;
            display: flex;
            align-items: flex-start;
            justify-content: center;
            padding-top: 14px;
        }

        .envelope-wrapper.opening .letter-peek {
            transform: translateY(-38%);
        }

        /* Envelope Pocket (Left, Right, Bottom Flaps) */
        .envelope-pocket {
            position: absolute;
            inset: 0;
            z-index: 2;
            pointer-events: none;
        }

        /* Left & Right Side Folds */
        .envelope-pocket::before {
            content: '';
            position: absolute;
            inset: 0;
            background: linear-gradient(135deg, #FFF5F7 50%, transparent 50%),
                        linear-gradient(225deg, #FFEDF0 50%, transparent 50%);
            opacity: 0.95;
        }

        /* Bottom Fold Triangle */
        .envelope-bottom {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 62%;
            background: linear-gradient(180deg, #FFFFFF 0%, #FFF1F3 100%);
            clip-path: polygon(0 100%, 50% 18%, 100% 100%);
            z-index: 3;
            box-shadow: 0 -4px 12px rgba(225, 29, 72, 0.04);
        }

        /* Top Flap (Animated Subtle Rose/Pastel Gradient) */
        .envelope-flap {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 58%;
            background: linear-gradient(180deg, #FFE4E8 0%, #FFF5F7 100%);
            clip-path: polygon(0 0, 100% 0, 50% 95%);
            transform-origin: top center;
            transition: transform 0.55s cubic-bezier(0.4, 0, 0.2, 1), z-index 0.2s;
            z-index: 4;
            filter: drop-shadow(0 4px 6px rgba(225, 29, 72, 0.08));
        }

        .envelope-wrapper.opening .envelope-flap {
            transform: rotateX(180deg);
            z-index: 0;
        }

        /* Wax Seal */
        .wax-seal {
            position: absolute;
            top: 47%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 48px;
            height: 48px;
            border-radius: 50%;
            background: radial-gradient(circle at 35% 35%, #F9D5DF, #F1B3C4 70%, #E092A8 100%);
            box-shadow: 
                0 4px 10px rgba(200, 122, 140, 0.35),
                inset 0 2px 4px rgba(255, 245, 248, 0.7),
                inset 0 -2px 4px rgba(175, 95, 115, 0.35);
            z-index: 5;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #FFF5F8;
            transition: transform 0.4s ease, opacity 0.3s ease;
            border: 2px solid rgba(255, 235, 242, 0.65);
        }

        .envelope-wrapper:hover .wax-seal {
            transform: translate(-50%, -50%) scale(1.08);
        }

        .envelope-wrapper.opening .wax-seal {
            opacity: 0;
            transform: translate(-50%, -50%) scale(0.6);
        }

        /* Crisp White Envelope Label Strip */
        .envelope-label {
            position: absolute;
            bottom: 14px;
            left: 16px;
            right: 16px;
            z-index: 4;
            text-align: center;
            background: rgba(255, 255, 255, 0.94);
            backdrop-filter: blur(4px);
            padding: 8px 12px;
            border-radius: 12px;
            border: 1px solid rgba(212, 175, 55, 0.3);
            box-shadow: 0 2px 8px rgba(39, 28, 30, 0.03);
        }

        /* ==========================================================================
           CLEAN WHITE LINED LETTER STATIONERY MODAL
           ========================================================================== */
        .modal-backdrop {
            opacity: 0;
            pointer-events: none;
            transition: opacity 0.35s ease;
        }

        .modal-backdrop.active {
            opacity: 1;
            pointer-events: auto;
        }

        .letter-modal {
            transform: translateY(24px) scale(0.96);
            opacity: 0;
            transition: all 0.4s cubic-bezier(0.22, 1, 0.36, 1);
            background-color: #FFFFFF;
            background-image: linear-gradient(to bottom, transparent 96%, rgba(212, 175, 55, 0.12) 97%);
            background-size: 100% 32px;
        }

        .modal-backdrop.active .letter-modal {
            transform: translateY(0) scale(1);
            opacity: 1;
        }

        /* Polaroid Photo Frame */
        .polaroid-frame {
            background: #FFFFFF;
            padding: 10px 10px 28px 10px;
            box-shadow: 0 8px 24px rgba(39, 28, 30, 0.08);
            border: 1px solid rgba(212, 175, 55, 0.28);
            transform: rotate(-1.5deg);
            transition: transform 0.3s ease;
        }

        .polaroid-frame:hover {
            transform: rotate(0deg) scale(1.01);
        }

        /* Custom Scrollbar for Letter Modal */
        .letter-scroll::-webkit-scrollbar {
            width: 6px;
        }
        .letter-scroll::-webkit-scrollbar-track {
            background: transparent;
        }
        .letter-scroll::-webkit-scrollbar-thumb {
            background: rgba(251, 113, 133, 0.35);
            border-radius: 999px;
        }
    </style>
</head>
<body class="antialiased selection:bg-[#FFE4E8] selection:text-[#271C1E]">

    <!-- Subtle Floating Gold & Rose Particles Canvas -->
    <canvas id="ambient-canvas"></canvas>

    <!-- Main Container -->
    <div class="relative z-10 max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-10 sm:py-16">
        
        <!-- ======================================================================
             HEADER SECTION
             ====================================================================== -->
        <header class="text-center max-w-2xl mx-auto mb-12 sm:mb-16">
            <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-[#F9EBE8] border border-[#EED5D0] text-[#9E4E4C] text-xs font-semibold tracking-widest uppercase mb-4 shadow-sm">
                <svg class="w-3.5 h-3.5 text-[#F4A6B8]" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M12 2L14.4 9.6L22 12L14.4 14.4L12 22L9.6 14.4L2 12L9.6 9.6L12 2Z" />
                </svg>
                <span>A Digital Time Capsule For You</span>
            </div>
            
            <!-- CUSTOMIZE HER NAME / TITLE HERE -->
            <h1 id="main-title" class="font-serif-editorial text-4xl sm:text-5xl lg:text-6xl font-bold text-[#271C1E] tracking-tight mb-4">
                Happy Birthday, My Love
            </h1>

            <p id="main-subtitle" class="text-base sm:text-lg text-[#6E5A5E] leading-relaxed mb-7">
                Because one birthday wish isn't nearly enough. Here are six letters written just for you—open each envelope whenever the moment feels right.
            </p>

            <!-- Action Bar: Celebrate Button & Progress Tracker -->
            <div class="flex flex-wrap items-center justify-center gap-3 sm:gap-4">
                <button id="celebrate-btn" class="inline-flex items-center gap-2 px-6 py-3 rounded-full bg-gradient-to-r from-[#C87A78] to-[#B36260] hover:from-[#B86A68] hover:to-[#9E4E4C] text-white font-medium text-sm shadow-md shadow-[#C87A78]/25 transition-all duration-200 active:scale-95 cursor-pointer">
                    <svg class="w-4 h-4 text-[#FFD6E0]" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 3v4M3 5h4M6 17v4m-2-2h4m5-16l2.286 6.857L21 12l-5.714 2.143L13 21l-2.286-6.857L5 12l5.714-2.143L13 3z"></path>
                    </svg>
                    <span>Celebrate Today</span>
                </button>

                <div class="inline-flex items-center gap-2 px-4 py-2.5 rounded-full bg-white border border-[#D4AF37]/40 text-xs sm:text-sm text-[#6E5A5E] shadow-sm">
                    <span class="w-2 h-2 rounded-full bg-[#D4AF37]"></span>
                    <span id="progress-text">0 of 6 envelopes opened</span>
                </div>
            </div>
        </header>

        <!-- ======================================================================
             RESPONSIVE GRID OF 6 ENVELOPES
             ====================================================================== -->
        <main>
            <div id="envelopes-grid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-7 sm:gap-8 lg:gap-10">
                <!-- Envelopes are dynamically injected here by JavaScript -->
            </div>
        </main>

        <!-- ======================================================================
             FOOTER
             ====================================================================== -->
        <footer class="mt-16 sm:mt-20 text-center text-xs sm:text-sm text-[#6E5A5E]/80">
            <p class="font-serif-editorial italic text-base text-[#E11D48] mb-1">Made with all my heart, just for you.</p>
            <button id="reset-progress-btn" class="underline hover:text-[#271C1E] transition-colors mt-2 cursor-pointer">
                Reset envelope seals
            </button>
        </footer>
    </div>

    <!-- ==========================================================================
         INTERACTIVE WHITE LETTER STATIONERY MODAL
         ========================================================================== -->
    <div id="letter-modal-backdrop" class="modal-backdrop fixed inset-0 z-50 flex items-center justify-center p-4 sm:p-6 bg-[#271C1E]/40 backdrop-blur-sm" aria-hidden="true">
        <div class="letter-modal relative w-full max-w-2xl max-h-[90vh] rounded-2xl shadow-2xl border border-[#D4AF37]/45 flex flex-col overflow-hidden" role="dialog" aria-modal="true">
            
            <!-- Top Decorative Header & Close Button -->
            <div class="flex items-center justify-between px-6 py-4 bg-[#FFFDF9] border-b border-[#FFE4E8]">
                <span id="modal-tag" class="text-xs font-semibold uppercase tracking-widest text-[#E11D48]">
                    Open When...
                </span>
                <button id="close-modal-btn" class="p-2 rounded-full text-[#6E5A5E] hover:text-[#271C1E] hover:bg-[#FFF1F3] transition-colors cursor-pointer" aria-label="Close letter">
                    <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                    </svg>
                </button>
            </div>

            <!-- Scrollable Modal Content -->
            <div class="letter-scroll overflow-y-auto p-6 sm:p-10 space-y-6">
                
                <!-- Secret Passcode Gate (Only shown for Envelope #6 if locked) -->
                <div id="passcode-gate" class="hidden text-center py-8 px-4 space-y-5">
                    <div class="w-16 h-16 mx-auto rounded-full bg-[#FFF1F3] border border-[#D4AF37]/40 flex items-center justify-center text-2xl shadow-inner">
                        🔒
                    </div>
                    <div>
                        <h3 class="font-serif-editorial text-2xl sm:text-3xl font-bold text-[#271C1E] mb-2">
                            A Secret Birthday Surprise
                        </h3>
                        <p id="passcode-hint" class="text-sm text-[#6E5A5E] max-w-md mx-auto">
                            Enter our special passcode to unlock your final birthday letter.
                        </p>
                    </div>
                    
                    <form id="passcode-form" class="max-w-xs mx-auto space-y-3">
                        <input 
                            type="text" 
                            id="passcode-input" 
                            placeholder="Enter passcode..." 
                            autocomplete="off"
                            class="w-full px-4 py-3 text-center rounded-xl border border-[#FFE4E8] bg-[#FFFDF9] focus:outline-none focus:ring-2 focus:ring-[#FB7185] text-[#271C1E] font-medium tracking-wider"
                        />
                        <p id="passcode-error" class="hidden text-xs text-[#E11D48] font-medium">
                            Not quite! Try the hint above or click reveal below.
                        </p>
                        <button type="submit" class="w-full py-3 rounded-xl bg-[#E11D48] hover:bg-[#BE123C] text-white font-medium text-sm shadow-md transition-colors cursor-pointer">
                            Unlock Envelope
                        </button>
                    </form>

                    <div class="pt-2">
                        <button id="instant-reveal-btn" type="button" class="text-xs text-[#6E5A5E] underline hover:text-[#E11D48] cursor-pointer">
                            Can't wait? Tap here to reveal now ✨
                        </button>
                    </div>
                </div>

                <!-- Actual Letter View -->
                <div id="letter-content-view" class="space-y-6">
                    <!-- Date Stamp & Title -->
                    <div class="border-b border-[#D4AF37]/30 pb-4 flex flex-col sm:flex-row sm:items-baseline sm:justify-between gap-2">
                        <h2 id="modal-title" class="font-serif-editorial text-2xl sm:text-3xl font-bold text-[#271C1E]">
                            Open on your birthday morning
                        </h2>
                        <span id="modal-date" class="font-handwritten text-xl text-[#E11D48] shrink-0">
                            November 19
                        </span>
                    </div>

                    <!-- Optional Polaroid Photo Frame -->
                    <div id="modal-photo-container" class="max-w-sm mx-auto my-4">
                        <div class="polaroid-frame rounded-xl">
                            <div class="aspect-[4/3] w-full overflow-hidden rounded-lg bg-[#FFF1F3]">
                                <img 
                                    id="modal-photo" 
                                    src="" 
                                    alt="Our Memory" 
                                    class="w-full h-full object-cover"
                                    onerror="this.src='https://placehold.co/600x450/FFF1F3/E11D48?text=Add+Your+Favorite+Photo+Here'"
                                />
                            </div>
                            <p id="modal-photo-caption" class="font-handwritten text-center text-xl text-[#6E5A5E] mt-2">
                                One of my favorite moments with you
                            </p>
                        </div>
                    </div>

                    <!-- Letter Body -->
                    <div id="modal-body" class="font-serif-editorial text-lg sm:text-xl text-[#271C1E] leading-relaxed space-y-4">
                        <!-- Paragraphs injected here -->
                    </div>

                    <!-- Handwritten Sign-off -->
                    <div class="pt-4 border-t border-[#D4AF37]/25 text-right">
                        <p class="font-serif-editorial italic text-base text-[#6E5A5E]">Forever yours,</p>
                        <p id="modal-signature" class="font-handwritten text-3xl text-[#E11D48] mt-1">
                            Your Favorite Person ❤️
                        </p>
                    </div>
                </div>

            </div>
        </div>
    </div>

    <!-- ==========================================================================
         CUSTOMIZATION & APPLICATION LOGIC
         ========================================================================== -->
    <script>
        /**
         * ========================================================================
         * 1. EASY CUSTOMIZATION SECTION (EDIT EVERYTHING HERE!)
         * ========================================================================
         * Customize her name, your signature, the secret passcode, and each of the
         * 6 letters below. For photos, paste an image URL or relative file path
         * (e.g., "./photos/us.jpg"), or leave the placeholder as-is!
         */
        const CONFIG = {
            mainTitle: "Happy Birthday, My Love",
            mainSubtitle: "Because one birthday wish isn't nearly enough. Here are six letters written just for you—open each envelope whenever the moment feels right.",
            signature: "Yours Always ❤️",
            storageKey: "birthday_open_when_capsule_v2"
        };

        const ENVELOPES_DATA = [
            {
                id: 1,
                label: "Open on your birthday morning",
                sealIcon: "🎂",
                dateStamp: "Birthday Morning",
                photoUrl: "https://placehold.co/600x450/FFF1F3/E11D48?text=Happy+Birthday+Beautiful",
                photoCaption: "Here's to another trip around the sun together ✨",
                paragraphs: [
                    "Good morning, birthday girl! Before the day gets busy with messages, calls, and celebrations, I wanted to be the very first to remind you how deeply loved you are.",
                    "Waking up knowing I get to walk through life beside you is the greatest gift I could ever ask for. You bring warmth, kindness, and a light into every room you enter.",
                    "Take a deep breath today, soak in every bit of joy coming your way, and get ready—because today is all about celebrating the incredible person you are."
                ]
            },
            {
                id: 2,
                label: "Open when you miss me",
                sealIcon: "💌",
                dateStamp: "Whenever We're Apart",
                photoUrl: "https://placehold.co/600x450/FFE4E8/E11D48?text=Thinking+Of+You",
                photoCaption: "No matter the distance, I'm always right there with you",
                paragraphs: [
                    "If you're opening this right now, chances are we're apart and I'm probably missing you just as much as you're missing me.",
                    "Close your eyes for a second and remember the feeling of my hand in yours. Distance and busy schedules are temporary, but what we have is constant.",
                    "Send me a quick text or voice note right now—even if it's just an emoji—so I know you opened this. Counting down the minutes until I see you next."
                ]
            },
            {
                id: 3,
                label: "Open when you need a laugh",
                sealIcon: "😂",
                dateStamp: "Emergency Smile Kit",
                /* Pointing to your local folder pictures. Make sure to copy your chosen image into your project directory */
                photoUrl: "./Printwork LS/your-photo-name.jpg", 
                photoCaption: "Still undefeated at making each other laugh",
                paragraphs: [
                    "Stop whatever serious thing you're doing right now and picture the most ridiculous inside joke we share. Yes, that one.",
                    "One of my favorite things about us is how effortlessly you make me laugh until my stomach hurts—even on days when nothing goes according to plan.",
                    "Consider this your official reminder not to take today too seriously. Put on your favorite upbeat song, do a terrible dance move, and remember I'm always cheering you on."
                ]
            },
            {
                id: 4,
                label: "Open when you had a long day",
                sealIcon: "🌙",
                dateStamp: "Take a Deep Breath",
                photoUrl: "https://placehold.co/600x450/FFE4E8/E11D48?text=Peace+%26+Comfort",
                photoCaption: "You don't have to carry everything on your own",
                paragraphs: [
                    "Hey love. If today felt heavy, exhausting, or overwhelming, I want you to drop your shoulders, unclench your jaw, and take one slow, deep breath.",
                    "You work so hard and care so deeply about everything you do, and I am endlessly proud of you—not just for what you accomplish, but for the grace you carry even on tough days.",
                    "Leave the stress of today outside the door. Tonight, let me take care of you, listen to everything on your mind, or simply sit beside you in quiet comfort."
                ]
            },
            {
                id: 5,
                label: "Open when you want to remember our favorite memory",
                sealIcon: "✨",
                dateStamp: "A Moment Frozen in Time",
                photoUrl: "https://placehold.co/600x450/FFF1F3/E11D48?text=Our+Favorite+Adventure",
                photoCaption: "The exact moment I knew how lucky I was",
                paragraphs: [
                    "Whenever I think back on our favorite memories together, I can't help but smile like an idiot.",
                    "Whether we're out exploring somewhere new or doing absolutely nothing together, you turn ordinary moments into stories I want to keep forever.",
                    "The best part? As much as I treasure every memory we've already made, I'm even more excited for all the adventures still ahead of us."
                ]
            },
            {
                id: 6,
                label: "Open when you are ready for your birthday surprise",
                sealIcon: "🎁",
                dateStamp: "The Grand Finale",
                isLocked: true, // Set to false if you don't want a passcode prompt
                passcode: "LOVE", // Case-insensitive passcode
                passcodeHint: "Hint: Type the 4-letter word 'LOVE' (or tap reveal below!)",
                photoUrl: "https://placehold.co/600x450/FFE4E8/E11D48?text=Your+Birthday+Surprise!",
                photoCaption: "Pack a smile—tonight is all yours",
                paragraphs: [
                    "You unlocked it! Happy Birthday again, my love.",
                    "Here is your official birthday voucher: Tonight, dinner, dessert, and every single plan are completely taken care of—all you have to do is get dressed up and let me spoil you.",
                    "I love you more than code or words could ever capture. Happy Birthday!"
                ]
            }
        ];

        /**
         * ========================================================================
         * 2. STATE MANAGEMENT & INITIALIZATION
         * ========================================================================
         */
        let openedIds = JSON.parse(localStorage.getItem(CONFIG.storageKey)) || [];
        let unlockedSecret = false;
        let currentEnvelope = null;

        document.addEventListener("DOMContentLoaded", () => {
            document.getElementById("main-title").textContent = CONFIG.mainTitle;
            document.getElementById("main-subtitle").textContent = CONFIG.mainSubtitle;
            document.getElementById("modal-signature").textContent = CONFIG.signature;

            renderEnvelopes();
            updateProgress();
            initAmbientParticles();
            triggerGentleConfetti();
        });

        /**
         * ========================================================================
         * 3. RENDER ENVELOPES GRID
         * ========================================================================
         */
        function renderEnvelopes() {
            const grid = document.getElementById("envelopes-grid");
            grid.innerHTML = "";

            ENVELOPES_DATA.forEach((env, index) => {
                const isOpened = openedIds.includes(env.id);

                const wrapper = document.createElement("div");
                wrapper.className = "envelope-wrapper group select-none";
                wrapper.setAttribute("role", "button");
                wrapper.setAttribute("tabindex", "0");
                wrapper.setAttribute("aria-label", env.label);

                wrapper.innerHTML = `
                    <div class="envelope-card">
                        <!-- Subtle Opened Badge -->
                        ${isOpened ? `
                            <div class="absolute top-3 right-3 z-10 inline-flex items-center gap-1 px-2.5 py-1 rounded-full bg-white/90 border border-[#C59B5F]/40 text-[11px] font-semibold text-[#9E4E4C] shadow-sm">
                                <span>✓ Opened</span>
                            </div>
                        ` : `
                            <div class="absolute top-3 left-3 z-10 inline-flex items-center px-2.5 py-0.5 rounded-full bg-white/70 text-[11px] font-medium text-[#6E5D5D]">
                                0${index + 1}
                            </div>
                        `}

                        <!-- Inner Letter Card Peek -->
                        <div class="letter-peek">
                            <span class="font-handwritten text-lg text-[#E11D48] opacity-85">For You...</span>
                        </div>

                        <!-- Side Folds -->
                        <div class="envelope-pocket"></div>

                        <!-- Animated Top Flap -->
                        <div class="envelope-flap"></div>

                        <!-- Gold Wax Seal -->
                        <div class="wax-seal" title="Tap to break seal">
                            <span class="text-lg leading-none">${env.sealIcon}</span>
                        </div>

                        <!-- Bottom Pocket Fold -->
                        <div class="envelope-bottom"></div>

                        <!-- Crisp White Envelope Label -->
                        <div class="envelope-label">
                            <p class="font-serif-editorial font-semibold text-base sm:text-lg text-[#271C1E] leading-snug">
                                ${env.label}
                            </p>
                        </div>
                    </div>
                `;

                const handleOpen = () => openEnvelopeAnimation(wrapper, env);
                wrapper.addEventListener("click", handleOpen);
                wrapper.addEventListener("keydown", (e) => {
                    if (e.key === "Enter" || e.key === " ") {
                        e.preventDefault();
                        handleOpen();
                    }
                });

                grid.appendChild(wrapper);
            });
        }

        /**
         * ========================================================================
         * 4. ENVELOPE OPENING ANIMATION & MODAL DISPLAY
         * ========================================================================
         */
        function openEnvelopeAnimation(wrapperElement, envelopeData) {
            currentEnvelope = envelopeData;
            wrapperElement.classList.add("opening");

            setTimeout(() => {
                showLetterModal(envelopeData);
                wrapperElement.classList.remove("opening");
            }, 420);
        }

        function showLetterModal(env) {
            const backdrop = document.getElementById("letter-modal-backdrop");
            const passcodeGate = document.getElementById("passcode-gate");
            const letterView = document.getElementById("letter-content-view");

            document.getElementById("modal-tag").textContent = `Envelope 0${env.id}`;

            // Check if Envelope has a secret passcode lock
            if (env.isLocked && !unlockedSecret) {
                passcodeGate.classList.remove("hidden");
                letterView.classList.add("hidden");
                document.getElementById("passcode-hint").textContent = env.passcodeHint || "Enter the secret passcode to unlock.";
                document.getElementById("passcode-input").value = "";
                document.getElementById("passcode-error").classList.add("hidden");
            } else {
                passcodeGate.classList.add("hidden");
                letterView.classList.remove("hidden");
                populateLetterContent(env);
                markAsOpened(env.id);
                triggerGentleConfetti();
            }

            backdrop.classList.add("active");
            backdrop.setAttribute("aria-hidden", "false");
            document.body.style.overflow = "hidden";
        }

        function populateLetterContent(env) {
            document.getElementById("modal-title").textContent = env.label;
            document.getElementById("modal-date").textContent = env.dateStamp;

            const photoContainer = document.getElementById("modal-photo-container");
            const photoImg = document.getElementById("modal-photo");
            const photoCaption = document.getElementById("modal-photo-caption");

            if (env.photoUrl) {
                photoContainer.classList.remove("hidden");
                photoImg.src = env.photoUrl;
                photoCaption.textContent = env.photoCaption || "";
            } else {
                photoContainer.classList.add("hidden");
            }

            const bodyContainer = document.getElementById("modal-body");
            bodyContainer.innerHTML = env.paragraphs
                .map(text => `<p>${text}</p>`)
                .join("");
        }

        function closeLetterModal() {
            const backdrop = document.getElementById("letter-modal-backdrop");
            backdrop.classList.remove("active");
            backdrop.setAttribute("aria-hidden", "true");
            document.body.style.overflow = "";
        }

        /**
         * ========================================================================
         * 5. SECRET PASSCODE HANDLERS (ENVELOPE #6)
         * ========================================================================
         */
        document.getElementById("passcode-form").addEventListener("submit", (e) => {
            e.preventDefault();
            if (!currentEnvelope) return;

            const inputVal = document.getElementById("passcode-input").value.trim().toUpperCase();
            const expected = (currentEnvelope.passcode || "").trim().toUpperCase();

            if (inputVal === expected) {
                unlockSecretEnvelope();
            } else {
                document.getElementById("passcode-error").classList.remove("hidden");
            }
        });

        document.getElementById("instant-reveal-btn").addEventListener("click", () => {
            unlockSecretEnvelope();
        });

        function unlockSecretEnvelope() {
            unlockedSecret = true;
            document.getElementById("passcode-gate").classList.add("hidden");
            document.getElementById("letter-content-view").classList.remove("hidden");
            populateLetterContent(currentEnvelope);
            markAsOpened(currentEnvelope.id);
            triggerGentleConfetti();
        }

        /**
         * ========================================================================
         * 6. LOCALSTORAGE READ-STATUS TRACKING
         * ========================================================================
         */
        function markAsOpened(id) {
            if (!openedIds.includes(id)) {
                openedIds.push(id);
                localStorage.setItem(CONFIG.storageKey, JSON.stringify(openedIds));
                renderEnvelopes();
                updateProgress();
            }
        }

        function updateProgress() {
            const progressText = document.getElementById("progress-text");
            progressText.textContent = `${openedIds.length} of ${ENVELOPES_DATA.length} envelopes opened`;
        }

        document.getElementById("reset-progress-btn").addEventListener("click", () => {
            openedIds = [];
            unlockedSecret = false;
            localStorage.removeItem(CONFIG.storageKey);
            renderEnvelopes();
            updateProgress();
        });

        /**
         * ========================================================================
         * 7. MODAL CLOSE LISTENERS & SUBTLE CONFETTI
         * ========================================================================
         */
        document.getElementById("close-modal-btn").addEventListener("click", closeLetterModal);

        document.getElementById("letter-modal-backdrop").addEventListener("click", (e) => {
            if (e.target.id === "letter-modal-backdrop") {
                closeLetterModal();
            }
        });

        document.addEventListener("keydown", (e) => {
            if (e.key === "Escape") {
                closeLetterModal();
            }
        });

        function triggerGentleConfetti() {
            if (typeof confetti !== "function") return;
            confetti({
                particleCount: 55,
                spread: 70,
                origin: { y: 0.65 },
                colors: ["#E11D48", "#FB7185", "#D4AF37", "#FFE4E8", "#F3E5AB"]
            });
        }

        document.getElementById("celebrate-btn").addEventListener("click", () => {
            triggerGentleConfetti();
        });

        /**
         * ========================================================================
         * 8. SUBTLE FLOATING GOLD & BLUSH PARTICLES BACKGROUND
         * ========================================================================
         */
        function initAmbientParticles() {
            const canvas = document.getElementById("ambient-canvas");
            const ctx = canvas.getContext("2d");
            let particles = [];

            function resize() {
                canvas.width = window.innerWidth;
                canvas.height = window.innerHeight;
            }
            window.addEventListener("resize", resize);
            resize();

            const colors = [
                "rgba(251, 113, 133, 0.22)",
                "rgba(212, 175, 55, 0.22)",
                "rgba(255, 228, 232, 0.45)"
            ];

            for (let i = 0; i < 24; i++) {
                particles.push({
                    x: Math.random() * canvas.width,
                    y: Math.random() * canvas.height,
                    radius: Math.random() * 3.5 + 1.5,
                    speedY: Math.random() * 0.35 + 0.15,
                    speedX: (Math.random() - 0.5) * 0.25,
                    color: colors[Math.floor(Math.random() * colors.length)]
                });
            }

            function animate() {
                ctx.clearRect(0, 0, canvas.width, canvas.height);
                particles.forEach(p => {
                    p.y -= p.speedY;
                    p.x += p.speedX;

                    if (p.y < -10) {
                        p.y = canvas.height + 10;
                        p.x = Math.random() * canvas.width;
                    }

                    ctx.beginPath();
                    ctx.arc(p.x, p.y, p.radius, 0, Math.PI * 2);
                    ctx.fillStyle = p.color;
                    ctx.fill();
                });
                requestAnimationFrame(animate);
            }
            animate();
        }
    </script>
</body>
</html>
