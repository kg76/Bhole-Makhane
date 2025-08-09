<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FreshPress - Campus Laundry Service</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f9fafb;
        }
        
        .hero-gradient {
            background: linear-gradient(135deg, #60a5fa 0%, #3b82f6 100%);
        }
        
        .pricing-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        
        .service-card:hover {
            transform: scale(1.02);
        }
    </style>
</head>
<body>
    <!-- Navbar -->
    <nav class="bg-white shadow-md">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16">
                <div class="flex items-center">
                    <div class="flex-shrink-0 flex items-center">
                        <img src="https://placehold.co/50x50" alt="FreshPress Logo - Blue shirt with water drop icon" class="h-8 w-auto">
                        <span class="ml-2 text-xl font-bold text-blue-600">FreshPress</span>
                    </div>
                </div>
                <div class="flex items-center">
                    <button class="bg-blue-600 text-white px-4 py-2 rounded-md hover:bg-blue-700">
                        <i class="fas fa-sign-in-alt mr-2"></i>Login/Signup
                    </button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <div class="hero-gradient text-white py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center">
                <div>
                    <h1 class="text-4xl font-bold mb-4">Stress-free Laundry for Students</h1>
                    <p class="text-xl mb-6">Pickup & delivery laundry service at your PG/Hostel. Just ₹1500 for 6 months!</p>
                    <div class="flex space-x-4">
                        <button class="bg-white text-blue-600 px-6 py-3 rounded-lg font-semibold hover:bg-gray-100 transition">
                            <i class="fas fa-download mr-2"></i>Download App
                        </button>
                        <button class="border-2 border-white text-white px-6 py-3 rounded-lg font-semibold hover:bg-white hover:text-blue-600 transition">
                            <i class="fas fa-play-circle mr-2"></i>See How It Works
                        </button>
                    </div>
                </div>
                <div>
                    <img src="https://placehold.co/600x400" alt="Happy college student holding clean laundry bag, smartphone showing FreshPress app" class="rounded-lg shadow-xl">
                </div>
            </div>
        </div>
    </div>

    <!-- Booking Section -->
    <div class="bg-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-2xl font-bold text-center mb-2">Book a Laundry Pickup</h2>
            <p class="text-gray-600 text-center mb-8">Just 3 simple steps and we'll handle your laundry</p>
            
            <div class="bg-gray-50 rounded-xl p-6 max-w-3xl mx-auto">
                <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mb-6">
                    <div class="border-2 border-dashed border-gray-300 rounded-lg p-4 text-center">
                        <i class="fas fa-calendar-alt text-blue-600 text-2xl mb-2"></i>
                        <h3 class="font-medium">1. Schedule</h3>
                        <p class="text-sm text-gray-600">Choose pickup time</p>
                    </div>
                    <div class="border-2 border-dashed border-gray-300 rounded-lg p-4 text-center">
                        <i class="fas fa-tshirt text-blue-600 text-2xl mb-2"></i>
                        <h3 class="font-medium">2. Prepare</h3>
                        <p class="text-sm text-gray-600">Pack your clothes</p>
                    </div>
                    <div class="border-2 border-dashed border-gray-300 rounded-lg p-4 text-center">
                        <i class="fas fa-truck text-blue-600 text-2xl mb-2"></i>
                        <h3 class="font-medium">3. Track</h3>
                        <p class="text-sm text-gray-600">Follow delivery</p>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-sm p-6">
                    <form>
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2" for="location">Your Hostel/PG Name</label>
                            <select id="location" class="w-full px-4 py-2 border rounded-lg focus:ring-blue-500 focus:border-blue-500">
                                <option value="">Select your hostel/PG</option>
                                <option value="h1">ABC Girls Hostel</option>
                                <option value="h2">XYZ Boys PG</option>
                                <option value="h3">University Campus Hostel</option>
                            </select>
                        </div>
                        
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                            <div class="mb-4">
                                <label class="block text-gray-700 mb-2" for="date">Pickup Date</label>
                                <input type="date" id="date" class="w-full px-4 py-2 border rounded-lg focus:ring-blue-500 focus:border-blue-500">
                            </div>
                            <div class="mb-4">
                                <label class="block text-gray-700 mb-2" for="time">Pickup Time</label>
                                <select id="time" class="w-full px-4 py-2 border rounded-lg focus:ring-blue-500 focus:border-blue-500">
                                    <option value="">Select time slot</option>
                                    <option value="9-11">9 AM - 11 AM</option>
                                    <option value="11-1">11 AM - 1 PM</option>
                                    <option value="4-6">4 PM - 6 PM</option>
                                </select>
                            </div>
                        </div>
                        
                        <div class="mb-4">
                            <button type="button" class="text-blue-600 text-sm flex items-center" onclick="toggleSpecialInstructions()">
                                <i class="fas fa-plus-circle mr-1"></i> Add Special Instructions
                            </button>
                            <textarea id="specialInstructions" class="hidden mt-2 w-full px-4 py-2 border rounded-lg focus:ring-blue-500 focus:border-blue-500" rows="2" placeholder="Any specific washing instructions?"></textarea>
                        </div>
                        
                        <button type="submit" class="w-full bg-blue-600 text-white py-3 rounded-lg font-medium hover:bg-blue-700 transition">
                            Schedule Pickup (₹25 per kg)
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </div>

    <!-- Pricing Plans -->
    <div class="bg-gray-50 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-2xl font-bold text-center mb-2">Affordable Subscription Plans</h2>
            <p class="text-gray-600 text-center mb-8">Choose the plan that fits your washing needs</p>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Basic Plan -->
                <div class="pricing-card bg-white rounded-xl shadow-md p-6 transition duration-300">
                    <div class="text-center mb-4">
                        <h3 class="text-lg font-semibold text-gray-800">Basic Plan</h3>
                        <div class="mt-2">
                            <span class="text-4xl font-bold text-blue-600">₹1500</span>
                            <span class="text-gray-500">/6 months</span>
                        </div>
                        <p class="text-gray-500 mt-2">Ideal for occasional washers</p>
                    </div>
                    <ul class="space-y-3 mb-6">
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>10 washes/month (60 total)</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>5 kg per wash</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Standard detergents</span>
                        </li>
                        <li class="flex items-start text-gray-400">
                            <i class="fas fa-times mt-1 mr-2"></i>
                            <span>No ironing included</span>
                        </li>
                    </ul>
                    <button class="w-full bg-blue-100 text-blue-600 py-2 rounded-lg font-medium hover:bg-blue-200 transition">
                        Select Plan
                    </button>
                </div>
                
                <!-- Premium Plan (Recommended) -->
                <div class="pricing-card bg-white rounded-xl shadow-lg p-6 border-2 border-blue-500 relative transition duration-300">
                    <div class="absolute top-0 right-0 bg-blue-600 text-white text-xs font-bold px-2 py-1 rounded-bl-lg rounded-tr-lg">
                        MOST POPULAR
                    </div>
                    <div class="text-center mb-4">
                        <h3 class="text-lg font-semibold text-gray-800">Premium Plan</h3>
                        <div class="mt-2">
                            <span class="text-4xl font-bold text-blue-600">₹2500</span>
                            <span class="text-gray-500">/6 months</span>
                        </div>
                        <p class="text-gray-500 mt-2">Best for regular washers</p>
                    </div>
                    <ul class="space-y-3 mb-6">
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>20 washes/month (120 total)</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>7 kg per wash</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Premium detergents</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Basic ironing included</span>
                        </li>
                    </ul>
                    <button class="w-full bg-blue-600 text-white py-2 rounded-lg font-medium hover:bg-blue-700 transition">
                        Select Plan
                    </button>
                </div>
                
                <!-- Unlimited Plan -->
                <div class="pricing-card bg-white rounded-xl shadow-md p-6 transition duration-300">
                    <div class="text-center mb-4">
                        <h3 class="text-lg font-semibold text-gray-800">Unlimited Plan</h3>
                        <div class="mt-2">
                            <span class="text-4xl font-bold text-blue-600">₹3500</span>
                            <span class="text-gray-500">/6 months</span>
                        </div>
                        <p class="text-gray-500 mt-2">For heavy laundry needs</p>
                    </div>
                    <ul class="space-y-3 mb-6">
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Unlimited washes</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>10 kg per wash</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Premium+ detergents</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Full ironing service</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Monthly dry cleaning (2 items)</span>
                        </li>
                    </ul>
                    <button class="w-full bg-blue-100 text-blue-600 py-2 rounded-lg font-medium hover:bg-blue-200 transition">
                        Select Plan
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- How It Works -->
    <div class="py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-2xl font-bold text-center mb-2">How FreshPress Works</h2>
            <p class="text-gray-600 text-center mb-8">Simple 4-step process for clean clothes</p>
            
            <div class="grid grid-cols-1 md:grid-cols-4 gap-6">
                <div class="service-card bg-white p-6 rounded-lg shadow-sm text-center transition">
                    <div class="bg-blue-100 rounded-full w-16 h-16 flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-mobile-alt text-blue-600 text-2xl"></i>
                    </div>
                    <h3 class="font-medium mb-2">1. Book Via App</h3>
                    <p class="text-gray-600 text-sm">Select pickup time and location</p>
                </div>
                
                <div class="service-card bg-white p-6 rounded-lg shadow-sm text-center transition">
                    <div class="bg-blue-100 rounded-full w-16 h-16 flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-bell text-blue-600 text-2xl"></i>
                    </div>
                    <h3 class="font-medium mb-2">2. We Pickup</h3>
                    <p class="text-gray-600 text-sm">Executive comes at scheduled time</p>
                </div>
                
                <div class="service-card bg-white p-6 rounded-lg shadow-sm text-center transition">
                    <div class="bg-blue-100 rounded-full w-16 h-16 flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-water text-blue-600 text-2xl"></i>
                    </div>
                    <h3 class="font-medium mb-2">3. Professional Wash</h3>
                    <p class="text-gray-600 text-sm">Hygienic cleaning with quality detergents</p>
                </div>
                
                <div class="service-card bg-white p-6 rounded-lg shadow-sm text-center transition">
                    <div class="bg-blue-100 rounded-full w-16 h-16 flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-home text-blue-600 text-2xl"></i>
                    </div>
                    <h3 class="font-medium mb-2">4. Delivery Back</h3>
                    <p class="text-gray-600 text-sm">Clean clothes delivered within 24 hours</p>
                </div>
            </div>
            
            <div class="mt-12 bg-blue-50 rounded-xl p-8 text-center">
                <div class="max-w-3xl mx-auto">
                    <h3 class="text-xl font-semibold mb-4">Why Choose FreshPress?</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-left">
                        <div class="flex items-start">
                            <i class="fas fa-check-circle text-blue-600 mt-1 mr-3"></i>
                            <div>
                                <h4 class="font-medium">College Student Focused</h4>
                                <p class="text-gray-600 text-sm">Our pickup points cover all major hostels and PGs</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <i class="fas fa-check-circle text-blue-600 mt-1 mr-3"></i>
                            <div>
                                <h4 class="font-medium">Budget Pricing</h4>
                                <p class="text-gray-600 text-sm">50% cheaper than local laundry shops</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <i class="fas fa-check-circle text-blue-600 mt-1 mr-3"></i>
                            <div>
                                <h4 class="font-medium">No Hidden Charges</h4>
                                <p class="text-gray-600 text-sm">Pay once, unlimited washes in your plan</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <i class="fas fa-check-circle text-blue-600 mt-1 mr-3"></i>
                            <div>
                                <h4 class="font-medium">24/7 Support</h4>
                                <p class="text-gray-600 text-sm">WhatsApp, phone and in-app chat support</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Tracking Section -->
    <div class="bg-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-2xl font-bold text-center mb-8">Real-time Order Tracking</h2>
            
            <div class="bg-gray-50 rounded-xl p-6 max-w-3xl mx-auto">
                <div class="flex items-center mb-6">
                    <div class="bg-blue-600 text-white rounded-full w-10 h-10 flex items-center justify-center mr-4">
                        <i class="fas fa-shopping-bag"></i>
                    </div>
                    <div>
                        <h3 class="font-medium">Order #FP12345</h3>
                        <p class="text-gray-600 text-sm">Scheduled for pickup today at 5 PM</p>
                    </div>
                </div>
                
                <div class="relative pl-12">
                    <!-- Timeline -->
                    <div class="absolute left-6 h-full w-0.5 bg-gray-300 top-4"></div>
                    
                    <!-- Step 1 - Completed -->
                    <div class="mb-8 relative">
                        <div class="absolute left-0 -ml-7 w-6 h-6 rounded-full bg-green-500 flex items-center justify-center">
                            <i class="fas fa-check text-white text-xs"></i>
                        </div>
                        <div class="pl-4">
                            <h4 class="font-medium text-green-600">Order Confirmed</h4>
                            <p class="text-gray-600 text-sm">Today, 10:15 AM</p>
                        </div>
                    </div>
                    
                    <!-- Step 2 - Active -->
                    <div class="mb-8 relative">
                        <div class="absolute left-0 -ml-7 w-6 h-6 rounded-full bg-blue-600 flex items-center justify-center">
                            <i class="fas fa-sync-alt text-white text-xs animate-spin"></i>
                        </div>
                        <div class="pl-4">
                            <h4 class="font-medium">Pickup Executive Assigned</h4>
                            <p class="text-gray-600 text-sm">Rahul Kumar is on his way</p>
                            <div class="mt-2 flex items-center">
                                <i class="fas fa-motorcycle text-blue-500 mr-2"></i>
                                <span class="text-sm font-medium">ETA: 15 minutes</span>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Step 3 - Pending -->
                    <div class="mb-8 relative">
                        <div class="absolute left-0 -ml-7 w-6 h-6 rounded-full bg-gray-300 border-4 border-gray-100"></div>
                        <div class="pl-4">
                            <h4 class="font-medium text-gray-400">Washing in Progress</h4>
                            <p class="text-gray-400 text-sm">Will begin after pickup</p>
                        </div>
                    </div>
                    
                    <!-- Step 4 - Pending -->
                    <div class="relative">
                        <div class="absolute left-0 -ml-7 w-6 h-6 rounded-full bg-gray-300 border-4 border-gray-100"></div>
                        <div class="pl-4">
                            <h4 class="font-medium text-gray-400">Delivery Scheduled</h4>
                            <p class="text-gray-400 text-sm">Tomorrow by 2 PM</p>
                        </div>
                    </div>
                </div>
                
                <div class="mt-6 pt-6 border-t border-gray-200">
                    <button class="w-full bg-blue-600 text-white py-3 rounded-lg font-medium hover:bg-blue-700 transition flex items-center justify-center">
                        <i class="fas fa-comment-alt mr-2"></i> Chat with Support
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- FAQ Section -->
    <div class="bg-gray-50 py-12">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-2xl font-bold text-center mb-8">Frequently Asked Questions</h2>
            
            <div class="space-y-4">
                <div class="bg-white rounded-lg shadow-sm overflow-hidden">
                    <button class="faq-toggle w-full flex justify-between items-center p-4 text-left" onclick="toggleFAQ(this)">
                        <h3 class="font-medium">How does the ₹1500 for 6 months plan work?</h3>
                        <i class="fas fa-chevron-down transition-transform"></i>
                    </button>
                    <div class="faq-content hidden px-4 pb-4">
                        <p class="text-gray-600">Our ₹1500 plan gives you 10 washes per month (60 washes total) for 6 months. Each wash can be up to 5kg of clothes. This works out to just ₹25 per wash - much cheaper than local laundry services. Perfect for students who do laundry once or twice a week.</p>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-sm overflow-hidden">
                    <button class="faq-toggle w-full flex justify-between items-center p-4 text-left" onclick="toggleFAQ(this)">
                        <h3 class="font-medium">What if my clothes get damaged or lost?</h3>
                        <i class="fas fa-chevron-down transition-transform"></i>
                    </button>
                    <div class="faq-content hidden px-4 pb-4">
                        <p class="text-gray-600">FreshPress provides 100% coverage for any lost or damaged items. We photograph all garments at pickup and maintain strict quality control. In the rare case of damage, we'll either reimburse you for the garment or replace it with a new one of similar value.</p>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-sm overflow-hidden">
                    <button class="faq-toggle w-full flex justify-between items-center p-4 text-left" onclick="toggleFAQ(this)">
                        <h3 class="font-medium">Can I share my subscription with my roommate?</h3>
                        <i class="fas fa-chevron-down transition-transform"></i>
                    </button>
                    <div class="faq-content hidden px-4 pb-4">
                        <p class="text-gray-600">Yes! Our Family Plans allow you to share washes with up to 3 roommates. Just notify our support team and we'll link your accounts. You can even split the subscription cost among yourselves.</p>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-sm overflow-hidden">
                    <button class="faq-toggle w-full flex justify-between items-center p-4 text-left" onclick="toggleFAQ(this)">
                        <h3 class="font-medium">What detergent do you use? I have sensitive skin.</h3>
                        <i class="fas fa-chevron-down transition-transform"></i>
                    </button>
                    <div class="faq-content hidden px-4 pb-4">
                        <p class="text-gray-600">We use dermatologically-tested, hypoallergenic detergents that are gentle on skin. You can also choose from several options in the app, including organic or fragrance-free variants. Just leave a note with your preference when scheduling pickup.</p>
                    </div>
                </div>
            </div>
            
            <div class="mt-8 text-center">
                <button class="text-blue-600 font-medium flex items-center justify-center mx-auto">
                    <i class="fas fa-question-circle mr-2"></i> More Questions? Chat with us
                </button>
            </div>
        </div>
    </div>

    <!-- Testimonials -->
    <div class="py-12 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-2xl font-bold text-center mb-8">What Students Say</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-gray-50 rounded-xl p-6">
                    <div class="flex items-center mb-4">
                        <img src="https://placehold.co/50x50" alt="Smiling college student - Priya from Delhi University" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-medium">Priya K.</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600">"As a medical student, I never had time for laundry. FreshPress saved me 4 hours every week! Their 6-month plan is perfect for college schedules."</p>
                </div>
                
                <div class="bg-gray-50 rounded-xl p-6">
                    <div class="flex items-center mb-4">
                        <img src="https://placehold.co/50x50" alt="Happy student Rohan from IIT Bombay hostel" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-medium">Rohan M.</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600">"Hostel laundry machines were always broken. With FreshPress, I get clean clothes delivered to my hostel gate. Worth every rupee!"</p>
                </div>
                
                <div class="bg-gray-50 rounded-xl p-6">
                    <div class="flex items-center mb-4">
                        <img src="https://placehold.co/50x50" alt="Ananya, PG resident in Bangalore using FreshPress" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-medium">Ananya S.</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star-half-alt"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600">"PG life was stressful with no washing machines. FreshPress executives pickup with a smile and return clothes neatly folded. Life saver!"</p>
                </div>
            </div>
        </div>
    </div>

    <!-- CTA Section -->
    <div class="hero-gradient text-white py-12">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-3xl font-bold mb-4">Ready to say goodbye to laundry hassles?</h2>
            <p class="text-xl mb-8">Download the FreshPress app and get your first wash free!</p>
            <div class="flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-6">
                <button class="bg-white text-blue-600 px-6 py-3 rounded-lg font-semibold hover:bg-gray-100 transition flex items-center justify-center">
                    <i class="fab fa-google-play text-2xl mr-3"></i>
                    <div class="text-left">
                        <div class="text-xs">GET IT ON</div>
                        <div class="text-lg">Google Play</div>
                    </div>
                </button>
                <button class="bg-black text-white px-6 py-3 rounded-lg font-semibold hover:bg-gray-800 transition flex items-center justify-center">
                    <i class="fab fa-apple text-2xl mr-3"></i>
                    <div class="text-left">
                        <div class="text-xs">Download on the</div>
                        <div class="text-lg">App Store</div>
                    </div>
                </button>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <div class="flex items-center mb-4">
                        <img src="https://placehold.co/40x40" alt="FreshPress Logo" class="h-8 mr-2">
                        <span class="text-xl font-bold">FreshPress</span>
                    </div>
                    <p class="text-gray-400 mb-4">India's most trusted laundry service for students.</p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                    </div>
                </div>
                
                <div>
                    <h3 class="text-lg font-semibold mb-4">Services</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Wash & Fold</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Ironing</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Dry Cleaning</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Subscription Plans</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Emergency Wash</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-lg font-semibold mb-4">Company</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">About Us</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Careers</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Blog</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Press</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Contact</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-lg font-semibold mb-4">Support</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Help Center</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Terms of Service</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Privacy Policy</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Refund Policy</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-8 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 text-sm mb-4 md:mb-0">© 2023 FreshPress Technologies Pvt Ltd. All rights reserved.</p>
                <div class="flex space-x-6">
                    <img src="https://placehold.co/120x40" alt="Payment Methods - Accepts UPI, Credit Cards, Net Banking" class="h-10">
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Toggle FAQ items
        function toggleFAQ(button) {
            const content = button.nextElementSibling;
            const icon = button.querySelector('i');
            
            content.classList.toggle('hidden');
            icon.classList.toggle('rotate-180');
        }
        
        // Toggle special instructions textarea
        function toggleSpecialInstructions() {
            const textarea = document.getElementById('specialInstructions');
            textarea.classList.toggle('hidden');
        }
        
        // Simple booking form validation
        document.querySelector('form').addEventListener('submit', function(e) {
            const location = document.getElementById('location').value;
            const date = document.getElementById('date').value;
            const time = document.getElementById('time').value;
            
            if (!location || !date || !time) {
                e.preventDefault();
                alert('Please fill in all required fields before submitting.');
            }
        });
        
        // Animation for pricing cards on scroll
        document.addEventListener('DOMContentLoaded', function() {
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('animate-fadeInUp');
                    }
                });
            }, { threshold: 0.1 });
            
            document.querySelectorAll('.pricing-card, .service-card').forEach(card => {
                observer.observe(card);
                card.style.opacity = '0';
                card.classList.add('transition-all', 'duration-500', 'ease-in-out');
            });
            
            // Inject CSS for animations
            const style = document.createElement('style');
            style.textContent = `
                @keyframes fadeInUp {
                    from { opacity: 0; transform: translateY(20px); }
                    to { opacity: 1; transform: translateY(0); }
                }
                .animate-fadeInUp {
                    animation: fadeInUp 0.6s forwards;
                    opacity: 1 !important;
                }
            `;
            document.head.appendChild(style);
        });
    </script>
</body>
</html>
