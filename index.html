<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Secure Crypto Verification</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body { background-color: #0f172a; color: white; font-family: 'Inter', sans-serif; }
        .glass-card { background: rgba(30, 41, 59, 0.7); backdrop-filter: blur(10px); border: 1px solid rgba(255, 255, 255, 0.1); border-radius: 1rem; }
        .step { display: none; }
        .step.active { display: block; animation: fadeIn 0.5s ease-out; }
        @keyframes fadeIn { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }
        .spinner { border: 4px solid rgba(255, 255, 255, 0.1); border-left-color: #3b82f6; border-radius: 50%; width: 40px; height: 40px; animation: spin 1s linear infinite; }
        @keyframes spin { to { transform: rotate(360deg); } }
        .scan-line { position: absolute; width: 100%; height: 2px; background: #3b82f6; box-shadow: 0 0 15px #3b82f6; animation: scan 2s linear infinite; }
        @keyframes scan { 0% { top: 0; } 100% { top: 100%; } }
    </style>
</head>
<body class="min-h-screen flex items-center justify-center p-4">

    <div id="app" class="max-w-md w-full glass-card p-8 shadow-2xl">
        <!-- Header -->
        <div class="text-center mb-8">
            <div class="inline-block p-3 bg-blue-500/10 rounded-full mb-4">
                <i class="fas fa-shield-halved text-blue-500 text-2xl"></i>
            </div>
            <h1 class="text-xl font-bold tracking-tight">System Verification</h1>
        </div>

        <!-- Step 1: Wallet Confirmation -->
        <div id="step-1" class="step active">
            <div class="bg-green-500/10 border border-green-500/20 p-4 rounded-lg mb-6">
                <p class="text-sm text-green-400 mb-1">Incoming Payment Detected</p>
                <h2 class="text-2xl font-bold">$35,000.00 USDT</h2>
            </div>
            <p class="text-slate-400 text-sm mb-4">Please confirm you are the owner of the following address to accept these funds:</p>
            <div class="bg-black/20 p-3 rounded font-mono text-xs break-all border border-white/10 mb-6">
                TDDW3JnTQietyVdY2w56dioFURLHaoP1Uy
            </div>
            <button onclick="nextStep(2)" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 rounded-lg transition duration-200">
                Yes, I am the owner
            </button>
        </div>

        <!-- Step 2: Rules & Regulations -->
        <div id="step-2" class="step">
            <h3 class="font-bold mb-4">USDT Withdrawal Regulations</h3>
            <ul class="text-sm text-slate-300 space-y-3 mb-6">
                <li><i class="fas fa-check text-blue-500 mr-2"></i> Funds must be settled in a TRC-20 compatible wallet.</li>
                <li><i class="fas fa-check text-blue-500 mr-2"></i> Verification of identity is required for high-value transfers.</li>
                <li><i class="fas fa-check text-blue-500 mr-2"></i> Network fees may apply for standard processing.</li>
                <li><i class="fas fa-check text-blue-500 mr-2"></i> Reversal is not possible once the transaction is initiated.</li>
            </ul>
            <label class="flex items-center space-x-3 cursor-pointer mb-6">
                <input type="checkbox" id="accept-rules" class="form-checkbox h-5 w-5 text-blue-600 rounded">
                <span class="text-sm text-slate-400">I understand and accept all regulations</span>
            </label>
            <button onclick="handleRules()" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 rounded-lg transition">
                Continue
            </button>
        </div>

        <!-- Step 3: Initial Processing (15 Seconds) -->
        <div id="step-3" class="step text-center">
            <div class="flex justify-center mb-6">
                <div class="spinner"></div>
            </div>
            <p class="text-lg font-medium mb-2">Analyzing Network...</p>
            <p class="text-sm text-slate-400">Processing incoming $35,000 USDT transfer to your wallet. Please wait...</p>
            <div class="mt-8 bg-blue-500/5 h-1 w-full rounded-full overflow-hidden">
                <div id="progress-bar-1" class="bg-blue-500 h-full w-0 transition-all duration-1000"></div>
            </div>
        </div>

        <!-- Step 4: Face Verification -->
        <div id="step-4" class="step text-center">
            <div class="relative w-48 h-48 mx-auto bg-black/40 rounded-full border-2 border-blue-500/30 flex items-center justify-center overflow-hidden mb-6">
                <i class="fas fa-user text-6xl text-slate-600"></i>
                <div id="scanner" class="hidden">
                    <div class="scan-line"></div>
                </div>
            </div>
            <h3 class="text-lg font-bold mb-2">Biometric Face Verification</h3>
            <p class="text-sm text-slate-400 mb-6">Final security step required to process the transfer.</p>
            <button id="verify-btn" onclick="startScanning()" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 rounded-lg transition">
                Verify My Face
            </button>
        </div>

        <!-- Step 5: Final Loading -->
        <div id="step-5" class="step text-center">
            <div class="flex justify-center mb-6">
                <div class="spinner border-t-blue-400"></div>
            </div>
            <h3 class="text-xl font-bold mb-2">Processing Verification</h3>
            <p class="text-sm text-slate-400">Confirming biometric data with network nodes. This may take a moment...</p>
        </div>

        <!-- Step 6: Verification Error & License Fee -->
        <div id="step-6" class="step">
            <div class="bg-red-500/10 border border-red-500/20 p-4 rounded-lg mb-6 flex items-start space-x-3">
                <i class="fas fa-circle-exclamation text-red-500 mt-1"></i>
                <div>
                    <h3 class="font-bold text-red-500">Verification Error</h3>
                    <p class="text-xs text-red-400">Standard verification failed due to high transaction volume.</p>
                </div>
            </div>
            <p class="text-sm text-slate-300 mb-4">A **Full License Verification** is required to release the $35,000 USDT to your wallet.</p>
            <div class="bg-blue-500/10 p-4 rounded-lg mb-6">
                <div class="flex justify-between items-center mb-2">
                    <span class="text-xs text-blue-400">License Fee</span>
                    <span class="font-bold text-lg">32 TRX</span>
                </div>
                <p class="text-[10px] text-blue-300/60">This fee is required for instant network release and KYC validation.</p>
            </div>
            <button onclick="nextStep(7)" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 rounded-lg transition">
                I have paid, release my funds
            </button>
        </div>

        <!-- Step 7: Awaiting Confirmation -->
        <div id="step-7" class="step text-center">
            <div class="inline-block p-4 bg-yellow-500/10 rounded-full mb-6">
                <i class="fas fa-clock text-yellow-500 text-3xl animate-pulse"></i>
            </div>
            <h3 class="text-xl font-bold mb-2 text-yellow-500">Awaiting Confirmation</h3>
            <p class="text-sm text-slate-300 mb-6">Your payment of **32 TRX** is pending confirmation. To speed up the release of your **$35,000 USDT**, please send a screenshot of the payment to support.</p>
            <div class="p-4 border border-white/5 bg-white/5 rounded-lg text-xs text-slate-400 italic">
                The system will process the release once the license verification fee is confirmed on the blockchain.
            </div>
        </div>
    </div>

    <script>
        let currentStep = 1;

        function nextStep(step) {
            document.querySelectorAll('.step').forEach(el => el.classList.remove('active'));
            document.getElementById(`step-${step}`).classList.add('active');
            currentStep = step;
        }

        function handleRules() {
            if (document.getElementById('accept-rules').checked) {
                nextStep(3);
                startTimer(15000, 4);
            } else {
                alert('Please accept the regulations to continue.');
            }
        }

        function startTimer(duration, next) {
            let start = Date.now();
            let bar = document.getElementById('progress-bar-1');
            
            let timer = setInterval(() => {
                let diff = Date.now() - start;
                let percent = (diff / duration) * 100;
                if (bar) bar.style.width = percent + '%';
                
                if (diff >= duration) {
                    clearInterval(timer);
                    nextStep(next);
                }
            }, 100);
        }

        function startScanning() {
            const btn = document.getElementById('verify-btn');
            const scanner = document.getElementById('scanner');
            btn.disabled = true;
            btn.innerText = "Scanning Face...";
            scanner.classList.remove('hidden');

            setTimeout(() => {
                nextStep(5);
                setTimeout(() => {
                    nextStep(6);
                }, 4000); // Small processing pause
            }, 8000); // 8 second scan
        }
    </script>
</body>
</html>
