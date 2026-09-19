# Html-<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gurukula Hub</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        .tab-content { display: none; }
        .tab-content.active { display: block; }
    </style>
</head>
<body class="bg-gray-50 text-gray-800 font-sans">

    <!-- Navigation Header -->
    <header class="bg-indigo-700 text-shadow shadow-md sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 py-4 flex justify-between items-center">
            <h1 class="text-2xl font-bold text-white tracking-wide">Gurukula Hub</h1>
            <nav class="hidden md:flex space-x-6">
                <button onclick="switchTab('home')" class="text-white hover:text-indigo-200 transition font-medium">Home</button>
                <button onclick="switchTab('coaching')" class="text-white hover:text-indigo-200 transition font-medium">Coaching</button>
                <button onclick="switchTab('pg-hostel')" class="text-white hover:text-indigo-200 transition font-medium">PG & Hostel</button>
                <button onclick="switchTab('rent')" class="text-white hover:text-indigo-200 transition font-medium">Rent Room</button>
                <button onclick="switchTab('ride')" class="text-white hover:text-indigo-200 transition font-medium">Ride Berry</button>
                <button onclick="switchTab('mess')" class="text-white hover:text-indigo-200 transition font-medium">Mess</button>
                <button onclick="switchTab('stationery')" class="text-white hover:text-indigo-200 transition font-medium">Stationery</button>
            </nav>
            <div class="md:hidden">
                <button id="menu-btn" class="text-white focus:outline-none" onclick="toggleMobileMenu()">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path>
                    </svg>
                </button>
            </div>
        </div>
        <!-- Mobile Navigation Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-indigo-800 px-4 pt-2 pb-4 space-y-2">
            <button onclick="switchTab('home'); toggleMobileMenu();" class="block text-white hover:text-indigo-200 py-1">Home</button>
            <button onclick="switchTab('coaching'); toggleMobileMenu();" class="block text-white hover:text-indigo-200 py-1">Coaching</button>
            <button onclick="switchTab('pg-hostel'); toggleMobileMenu();" class="block text-white hover:text-indigo-200 py-1">PG & Hostel</button>
            <button onclick="switchTab('rent'); toggleMobileMenu();" class="block text-white hover:text-indigo-200 py-1">Rent Room</button>
            <button onclick="switchTab('ride'); toggleMobileMenu();" class="block text-white hover:text-indigo-200 py-1">Ride Berry</button>
            <button onclick="switchTab('mess'); toggleMobileMenu();" class="block text-white hover:text-indigo-200 py-1">Mess</button>
            <button onclick="switchTab('stationery'); toggleMobileMenu();" class="block text-white hover:text-indigo-200 py-1">Stationery</button>
        </div>
    </header>

    <!-- Main Container -->
    <main class="max-w-7xl mx-auto px-4 py-8">

        <!-- HOME TAB -->
        <section id="home" class="tab-content active space-y-8">
            <div class="bg-gradient-to-r from-indigo-600 to-blue-500 rounded-2xl p-8 md:p-12 text-white text-center shadow-lg">
                <h2 class="text-3xl md:text-5xl font-extrabold mb-4">Welcome to Gurukula Hub</h2>
                <p class="text-lg md:text-xl text-indigo-100 max-w-2xl mx-auto mb-6">Your ultimate student and residential ecosystem. Find coaching, housing, rides, food, and study supplies all in one place.</p>
                <button onclick="switchTab('coaching')" class="bg-white text-indigo-700 font-semibold px-6 py-3 rounded-lg shadow hover:bg-indigo-50 transition">Explore Services</button>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                <div onclick="switchTab('coaching')" class="bg-white p-6 rounded-xl shadow hover:shadow-md cursor-pointer transition border border-gray-100">
                    <h3 class="text-xl font-bold text-indigo-600 mb-2">Coaching Hub</h3>
                    <p class="text-gray-600">Discover top-rated coaching centers, institutes, and expert tutors near you.</p>
                </div>
                <div onclick="switchTab('pg-hostel')" class="bg-white p-6 rounded-xl shadow hover:shadow-md cursor-pointer transition border border-gray-100">
                    <h3 class="text-xl font-bold text-indigo-600 mb-2">PG & Hostel</h3>
                    <p class="text-gray-600">Secure safe, comfortable, and affordable paying guest and hostel options.</p>
                </div>
                <div onclick="switchTab('rent')" class="bg-white p-6 rounded-xl shadow hover:shadow-md cursor-pointer transition border border-gray-100">
                    <h3 class="text-xl font-bold text-indigo-600 mb-2">Rent Room</h3>
                    <p class="text-gray-600">Find private rental rooms and flats tailored to your budget and location.</p>
                </div>
                <div onclick="switchTab('ride')" class="bg-white p-6 rounded-xl shadow hover:shadow-md cursor-pointer transition border border-gray-100">
                    <h3 class="text-xl font-bold text-indigo-600 mb-2">Ride Berry</h3>
                    <p class="text-gray-600">Share rides, carpool, or find daily commuting options effortlessly.</p>
                </div>
                <div onclick="switchTab('mess')" class="bg-white p-6 rounded-xl shadow hover:shadow-md cursor-pointer transition border border-gray-100">
                    <h3 class="text-xl font-bold text-indigo-600 mb-2">Mess</h3>
                    <p class="text-gray-600">Healthy and delicious tiffin services and mess facilities for students.</p>
                </div>
                <div onclick="switchTab('stationery')" class="bg-white p-6 rounded-xl shadow hover:shadow-md cursor-pointer transition border border-gray-100">
                    <h3 class="text-xl font-bold text-indigo-600 mb-2">Stationery Hub</h3>
                    <p class="text-gray-600">Books, notebooks, notes, and all educational stationery delivered fast.</p>
                </div>
            </div>
        </section>

        <!-- COACHING TAB -->
        <section id="coaching" class="tab-content space-y-6">
            <div class="flex justify-between items-center border-b pb-4">
                <h2 class="text-2xl font-bold text-indigo-700">Coaching Hub</h2>
                <span class="text-sm text-gray-500">Top Institutes & Tutors</span>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div class="bg-white rounded-xl shadow p-6 border border-gray-100">
                    <h3 class="font-bold text-lg text-gray-800 mb-1">Apex Science Academy</h3>
                    <p class="text-sm text-indigo-600 font-medium mb-3">Physics, Chemistry, Mathematics</p>
                    <p class="text-gray-600 text-sm mb-4">Specialized coaching for entrance exams with experienced faculty and proven results.</p>
                    <button onclick="openModal('Apex Science Academy')" class="w-full bg-indigo-600 text-white py-2 rounded-lg hover:bg-indigo-700 transition">Enquire Now</button>
                </div>
                <div class="bg-white rounded-xl shadow p-6 border border-gray-100">
                    <h3 class="font-bold text-lg text-gray-800 mb-1">Global Language & Skills</h3>
                    <p class="text-sm text-indigo-600 font-medium mb-3">Spoken English & Computer Basics</p>
                    <p class="text-gray-600 text-sm mb-4">Enhance your personality, communication skills, and technical knowledge.</p>
                    <button onclick="openModal('Global Language & Skills')" class="w-full bg-indigo-600 text-white py-2 rounded-lg hover:bg-indigo-700 transition">Enquire Now</button>
                </div>
            </div>
        </section>

        <!-- PG & HOSTEL TAB -->
        <section id="pg-hostel" class="tab-content space-y-6">
            <div class="flex justify-between items-center border-b pb-4">
                <h2 class="text-2xl font-bold text-indigo-700">PG & Hostel Accommodations</h2>
                <span class="text-sm text-gray-500">Safe & Secure Stays</span>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div class="bg-white rounded-xl shadow p-6 border border-gray-100">
                    <h3 class="font-bold text-lg text-gray-800 mb-1">Comfort Boys PG</h3>
                    <p class="text-sm text-indigo-600 font-medium mb-3">₹5,500 / month (Includes Wi-Fi & Food)</p>
                    <p class="text-gray-600 text-sm mb-4">Furnished rooms, 24/7 water, security, and high-speed internet near university areas.</p>
                    <button onclick="openModal('Comfort Boys PG')" class="w-full bg-indigo-600 text-white py-2 rounded-lg hover:bg-indigo-700 transition">Book Visit</button>
                </div>
                <div class="bg-white rounded-xl shadow p-6 border border-gray-100">
                    <h3 class="font-bold text-lg text-gray-800 mb-1">Grace Girls Hostel</h3>
                    <p class="text-sm text-indigo-600 font-medium mb-3">₹6,000 / month (Mess included)</p>
                    <p class="text-gray-600 text-sm mb-4">Safe environment with CCTV surveillance, warden, study room, and attached bathrooms.</p>
                    <button onclick="openModal('Grace Girls Hostel')" class="w-full bg-indigo-600 text-white py-2 rounded-lg hover:bg-indigo-700 transition">Book Visit</button>
                </div>
            </div>
        </section>

        <!-- RENT ROOM TAB -->
        <section id="rent" class="tab-content space-y-6">
            <div class="flex justify-between items-center border-b pb-4">
                <h2 class="text-2xl font-bold text-indigo-700">Rent Room</h2>
                <span class="text-sm text-gray-500">Independent Living Spaces</span>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div class="bg-white rounded-xl shadow p-6 border border-gray-100">
                    <h3 class="font-bold text-lg text-gray-800 mb-1">1RK Independent Studio</h3>
                    <p class="text-sm text-indigo-600 font-medium mb-3">₹4,500 / month</p>
                    <p class="text-gray-600 text-sm mb-4">Semi-furnished room with a separate kitchenette and washroom. Electricity separate.</p>
                    <button onclick="openModal('1RK Independent Studio')" class="w-full bg-indigo-600 text-white py-2 rounded-lg hover:bg-indigo-700 transition">Contact Owner</button>
                </div>
            </div>
        </section>

        <!-- RIDE BERRY TAB -->
        <section id="ride" class="tab-content space-y-6">
            <div class="flex justify-between items-center border-b pb-4">
                <h2 class="text-2xl font-bold text-indigo-700">Ride Berry</h2>
                <span class="text-sm text-gray-500">Commute & Carpooling</span>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div class="bg-white rounded-xl shadow p-6 border border-gray-100">
                    <h3 class="font-bold text-lg text-gray-800 mb-1">Daily Campus Pool</h3>
                    <p class="text-sm text-indigo-600 font-medium mb-3">Route: City Center to University Gate</p>
                    <p class="text-gray-600 text-sm mb-4">Share bike/auto rides with fellow students safely and economically every morning.</p>
                    <button onclick="openModal('Daily Campus Pool')" class="w-full bg-indigo-600 text-white py-2 rounded-lg hover:bg-indigo-700 transition">Join Ride</button>
                </div>
            </div>
        </section>

        <!-- MESS TAB -->
        <section id="mess" class="tab-content space-y-6">
            <div class="flex justify-between items-center border-b pb-4">
                <h2 class="text-2xl font-bold text-indigo-700">Mess & Tiffin Services</h2>
                <span class="text-sm text-gray-500">Ghar Ka Khana</span>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div class="bg-white rounded-xl shadow p-6 border border-gray-100">
                    <h3 class="font-bold text-lg text-gray-800 mb-1">Annapurna Tiffin Service</h3>
                    <p class="text-sm text-indigo-600 font-medium mb-3">₹2,800 / month (Lunch & Dinner)</p>
                    <p class="text-gray-600 text-sm mb-4">Hygenic, nutritious, and homely vegetarian meals delivered right to your room or hostel.</p>
                    <button onclick="openModal('Annapurna Tiffin Service')" class="w-full bg-indigo-600 text-white py-2 rounded-lg hover:bg-indigo-700 transition">Subscribe</button>
                </div>
            </div>
        </section>

        <!-- STATIONERY HUB TAB -->
        <section id="stationery" class="tab-content space-y-6">
            <div class="flex justify-between items-center border-b pb-4">
                <h2 class="text-2xl font-bold text-indigo-700">Stationery Hub</h2>
                <span class="text-sm text-gray-500">Books & Study Supplies</span>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div class="bg-white rounded-xl shadow p-6 border border-gray-100">
                    <h3 class="font-bold text-lg text-gray-800 mb-1">Vidya Stationery & Prints</h3>
                    <p class="text-sm text-indigo-600 font-medium mb-3">Notebooks, Pens, Photocopy & Spiral Binding</p>
                    <p class="text-gray-600 text-sm mb-4">All academic essentials and fast printing services available at student-friendly rates.</p>
                    <button onclick="openModal('Vidya Stationery & Prints')" class="w-full bg-indigo-600 text-white py-2 rounded-lg hover:bg-indigo-700 transition">Order Supplies</button>
                </div>
            </div>
        </section>

    </main>

    <!-- Modal Popup -->
    <div id="enquiry-modal" class="fixed inset-0 bg-black bg-opacity-50 hidden flex items-center justify-center p-4 z-50">
        <div class="bg-white rounded-xl max-w-md w-full p-6 relative">
            <button onclick="closeModal()" class="absolute top-4 right-4 text-gray-400 hover:text-gray-600 font-bold text-lg">&times;</button>
            <h3 id="modal-title" class="text-xl font-bold text-indigo-700 mb-2">Enquire</h3>
            <p class="text-sm text-gray-600 mb-4">Fill out your details below and we will get back to you shortly.</p>
            <form onsubmit="handleFormSubmit(event)" class="space-y-4">
                <div>
                    <label class="block text-sm font-medium text-gray-700 mb-1">Your Name</label>
                    <input type="text" required class="w-full border border-gray-300 rounded-lg px-3 py-2 focus:ring-indigo-500 focus:border-indigo-500">
                </div>
                <div>
                    <label class="block text-sm font-medium text-gray-700 mb-1">Phone Number</label>
                    <input type="tel" required class="w-full border border-gray-300 rounded-lg px-3 py-2 focus:ring-indigo-500 focus:border-indigo-500">
                </div>
                <button type="submit" class="w-full bg-indigo-600 text-white py-2 rounded-lg hover:bg-indigo-700 transition">Submit Request</button>
            </form>
        </div>
    </div>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white text-center py-6 mt-12">
        <p class="text-sm text-gray-400">&copy; Gurukula Hub. All rights reserved.</p>
    </footer>

    <!-- JavaScript functionality -->
    <script>
        function switchTab(tabId) {
            const tabs = document.querySelectorAll('.tab-content');
            tabs.forEach(tab => tab.classList.remove('active'));
            document.getElementById(tabId).classList.add('active');
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        function toggleMobileMenu() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        }

        function openModal(serviceName) {
            document.getElementById('modal-title').innerText = 'Enquire about ' + serviceName;
            document.getElementById('enquiry-modal').classList.remove('hidden');
        }

        function closeModal() {
            document.getElementById('enquiry-modal').classList.add('hidden');
        }

        function handleFormSubmit(event) {
            event.preventDefault();
            alert('Thank you! Your request has been submitted successfully.');
            closeModal();
        }
    </script>
</body>
</html>
