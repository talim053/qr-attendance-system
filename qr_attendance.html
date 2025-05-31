<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Look N Hook - Online Bag Shop</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Custom styles for professional look */
        body {
            font-family: "Inter", sans-serif; /* Inter font for a modern look */
            background-color: #f8f8f8; /* Light gray background */
            color: #333;
        }
        /* Ensure all elements have rounded corners */
        .rounded-lg, .rounded-md, .rounded-xl {
            border-radius: 0.5rem; /* Tailwind's default rounded-lg */
        }
        .shadow-md {
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .hover\:shadow-lg:hover {
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
        }
        .btn-primary {
            background-color: #3b82f6; /* Blue for primary actions */
            color: white;
            padding: 0.75rem 1.25rem;
            border-radius: 0.375rem; /* rounded-md */
            transition: background-color 0.3s ease;
        }
        .btn-primary:hover {
            background-color: #2563eb; /* Darker blue on hover */
        }
        .btn-secondary {
            background-color: #6b7280; /* Gray for secondary actions */
            color: white;
            padding: 0.75rem 1.25rem;
            border-radius: 0.375rem; /* rounded-md */
            transition: background-color 0.3s ease;
        }
        .btn-secondary:hover {
            background-color: #4b5563; /* Darker gray on hover */
        }
        /* Styles for the cart modal/sidebar */
        .cart-sidebar {
            position: fixed;
            top: 0;
            right: 0;
            width: 320px;
            height: 100%;
            background-color: white;
            box-shadow: -2px 0 10px rgba(0, 0, 0, 0.1);
            transform: translateX(100%);
            transition: transform 0.3s ease-in-out;
            z-index: 1000;
            display: flex;
            flex-direction: column;
        }
        .cart-sidebar.open {
            transform: translateX(0);
        }
        .cart-header {
            padding: 1rem;
            border-bottom: 1px solid #eee;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .cart-items {
            flex-grow: 1;
            padding: 1rem;
            overflow-y: auto;
        }
        .cart-item {
            display: flex;
            align-items: center;
            margin-bottom: 1rem;
            padding-bottom: 1rem;
            border-bottom: 1px dashed #eee;
            position: relative; /* For positioning the delete button */
        }
        .cart-item:last-child {
            border-bottom: none;
            margin-bottom: 0;
            padding-bottom: 0;
        }
        .cart-item img {
            width: 60px;
            height: 60px;
            object-fit: contain;
            border-radius: 4px;
            margin-right: 0.75rem;
        }
        .cart-item-details {
            flex-grow: 1;
        }
        .cart-item-details h4 {
            font-weight: 600;
            font-size: 0.95rem;
            margin-bottom: 0.25rem;
        }
        .cart-item-details p {
            font-size: 0.85rem;
            color: #666;
        }
        .cart-item-remove {
            background: none;
            border: none;
            color: #ef4444; /* Red color for delete */
            font-size: 1.2rem;
            cursor: pointer;
            padding: 0.2rem;
            margin-left: 0.5rem;
            transition: color 0.2s ease;
        }
        .cart-item-remove:hover {
            color: #dc2626;
        }
        .cart-summary {
            padding: 1rem;
            border-top: 1px solid #eee;
        }
        .cart-summary p {
            display: flex;
            justify-content: space-between;
            font-weight: bold;
            font-size: 1.1rem;
            margin-bottom: 0.5rem;
        }
        .empty-cart-message {
            text-align: center;
            color: #666;
            padding: 2rem;
        }

        /* Styles for Modals (Login/Account/Product Detail) */
        .modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 1001; /* Higher than cart sidebar */
            opacity: 0;
            visibility: hidden;
            transition: opacity 0.3s ease, visibility 0.3s ease;
        }
        .modal.open {
            opacity: 1;
            visibility: visible;
        }
        .modal-content {
            background-color: white;
            padding: 2rem;
            border-radius: 0.75rem; /* rounded-xl */
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            width: 90%;
            max-width: 400px;
            position: relative;
        }
        .modal-close-button {
            position: absolute;
            top: 1rem;
            right: 1rem;
            background: none;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: #666;
            transition: color 0.2s ease;
        }
        .modal-close-button:hover {
            color: #333;
        }
        .modal-input {
            width: 100%;
            padding: 0.75rem;
            margin-bottom: 1rem;
            border: 1px solid #ddd;
            border-radius: 0.375rem;
            font-size: 1rem;
        }
        .modal-button-group {
            display: flex;
            justify-content: space-between;
            gap: 1rem;
            margin-top: 1rem;
        }
        .modal-button-group .btn {
            flex-grow: 1;
        }
        .message-box {
            background-color: #f0fdf4; /* Light green */
            color: #16a34a; /* Dark green */
            padding: 0.75rem;
            border-radius: 0.375rem;
            margin-bottom: 1rem;
            text-align: center;
            border: 1px solid #bbf7d0;
            display: none; /* Hidden by default */
        }
        .message-box.error {
            background-color: #fee2e2; /* Light red */
            color: #dc2626; /* Dark red */
            border-color: #fecaca;
        }
        .message-box.show {
            display: block;
        }

        /* Product Detail Modal Specific Styles */
        #product-detail-modal .modal-content {
            max-width: 1000px; /* Wider for product details, more like Amazon */
            width: 95%;
            padding: 1.5rem;
            display: flex;
            flex-direction: row; /* Arrange content in a row */
            align-items: flex-start; /* Align items to the top */
            text-align: left; /* Align text left within content */
            gap: 2rem; /* Space between columns */
            overflow-y: auto; /* Allow scrolling if content is too long */
            max-height: 95vh; /* Limit height to viewport height */
        }

        @media (max-width: 768px) {
            #product-detail-modal .modal-content {
                flex-direction: column; /* Stack columns on smaller screens */
                align-items: center;
                text-align: center;
                max-height: 90vh; /* Adjust height for mobile */
            }
        }

        #product-detail-modal .product-image-section {
            flex: 1; /* Takes available space */
            display: flex;
            flex-direction: column;
            align-items: center;
            width: 100%; /* Full width on mobile */
            max-width: 450px; /* Max width for image section */
            position: relative; /* For slideshow buttons */
        }

        #product-detail-modal .product-detail-image {
            width: 100%;
            height: auto;
            max-height: 400px; /* Larger image for details */
            object-fit: contain;
            border-radius: 0.5rem;
            margin-bottom: 1rem;
        }
        #product-detail-modal .thumbnail-gallery {
            display: flex;
            flex-wrap: wrap; /* Allow thumbnails to wrap */
            gap: 0.5rem;
            margin-top: 0.5rem;
            justify-content: center; /* Center thumbnails */
            width: 100%;
        }
        #product-detail-modal .thumbnail-gallery img {
            width: 60px; /* Smaller thumbnails */
            height: 60px;
            object-fit: cover;
            border-radius: 0.375rem;
            cursor: pointer;
            border: 2px solid transparent;
            transition: border-color 0.2s ease;
        }
        #product-detail-modal .thumbnail-gallery img.active {
            border-color: #3b82f6; /* Blue border for active thumbnail */
        }

        /* Slideshow navigation buttons */
        .slideshow-nav-button {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            border: none;
            padding: 0.5rem 0.75rem;
            cursor: pointer;
            font-size: 1.5rem;
            border-radius: 0.25rem;
            z-index: 10;
            opacity: 0.7;
            transition: opacity 0.2s ease;
        }
        .slideshow-nav-button:hover {
            opacity: 1;
        }
        .slideshow-nav-button.prev {
            left: 0.5rem;
        }
        .slideshow-nav-button.next {
            right: 0.5rem;
        }


        #product-detail-modal .product-info-section {
            flex: 1.5; /* Takes more space for details */
            display: flex;
            flex-direction: column;
            width: 100%; /* Full width on mobile */
        }

        #product-detail-modal .product-info-section h3 {
            font-size: 2.25rem;
            font-weight: bold;
            color: #1f2937;
            margin-bottom: 0.5rem;
        }
        #product-detail-modal .product-info-section .rating {
            color: #f59e0b; /* Amber for stars */
            margin-bottom: 1rem;
        }
        #product-detail-modal .product-info-section .price {
            font-size: 2.5rem;
            font-weight: bold;
            color: #b91c1c; /* Red for price, common on Amazon */
            margin-top: 1rem;
            margin-bottom: 1.5rem;
        }
        #product-detail-modal .product-info-section p {
            font-size: 1rem;
            color: #4b5563;
            margin-bottom: 0.5rem;
        }
        #product-detail-modal .product-info-section strong {
            color: #1f2937;
        }
        #product-detail-modal .product-info-section .quantity-selector {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            margin-top: 1rem;
            margin-bottom: 1.5rem;
        }
        #product-detail-modal .product-info-section .quantity-selector input {
            width: 60px;
            padding: 0.5rem;
            border: 1px solid #ddd;
            border-radius: 0.375rem;
            text-align: center;
        }
        #product-detail-modal .add-to-cart-detail-btn {
            width: 100%;
            margin-top: 1rem;
        }
        #product-detail-modal .product-description-section,
        #product-detail-modal .product-technical-details-section {
            margin-top: 2rem;
            padding-top: 1.5rem;
            border-top: 1px solid #eee;
        }
        #product-detail-modal .product-description-section h4,
        #product-detail-modal .product-technical-details-section h4 {
            font-size: 1.5rem;
            font-weight: bold;
            color: #1f2937;
            margin-bottom: 1rem;
        }
        #product-detail-modal .product-description-section ul,
        #product-detail-modal .product-technical-details-section ul {
            list-style: disc;
            margin-left: 1.25rem;
            color: #4b5563;
        }
        #product-detail-modal .product-description-section li,
        #product-detail-modal .product-technical-details-section li {
            margin-bottom: 0.5rem;
        }

        /* Header Specific Styles for larger and more attractive look */
        .main-header {
            background: linear-gradient(to right, #4a90e2, #63b3ed); /* Blue gradient */
            padding: 1.5rem 1rem; /* Increased padding */
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15); /* More prominent shadow */
        }
        .main-header .logo-text {
            font-size: 2.5rem; /* Larger font size for logo text */
            font-weight: 700; /* Bolder font */
            color: #ffffff; /* White text for contrast */
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); /* Subtle text shadow */
        }
        .main-header .nav-link {
            color: #e0e7ff; /* Lighter blue for nav links */
            font-weight: 600;
            transition: color 0.3s ease, transform 0.2s ease;
        }
        .main-header .nav-link:hover {
            color: #ffffff; /* White on hover */
            transform: translateY(-2px); /* Slight lift on hover */
        }
        .main-header .search-input {
            background-color: rgba(255, 255, 255, 0.9); /* Slightly transparent white */
            border: none;
            padding: 0.75rem 1rem 0.75rem 2.5rem; /* Adjust padding for icon */
            border-radius: 9999px; /* Pill shape */
            color: #333;
            box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }
        .main-header .search-input:focus {
            outline: none;
            box-shadow: 0 0 0 3px rgba(66, 153, 225, 0.5); /* Blue focus ring */
        }
        .main-header .search-icon {
            color: #666;
            left: 1rem;
        }
        .main-header .icon-button {
            background-color: rgba(255, 255, 255, 0.2); /* Subtle background for icons */
            padding: 0.6rem;
            border-radius: 50%; /* Circular buttons */
            transition: background-color 0.3s ease, transform 0.2s ease;
        }
        .main-header .icon-button:hover {
            background-color: rgba(255, 255, 255, 0.4);
            transform: scale(1.1);
        }
        .main-header .icon-button i {
            color: white; /* White icons */
        }
        .main-header .cart-count {
            background-color: #ef4444; /* Red for cart count */
            border: 2px solid #63b3ed; /* Border matching header gradient */
        }

        /* Section specific styles for About Us and Contact Us */
        .content-section {
            background-color: white;
            border-radius: 0.75rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 2rem;
            margin-bottom: 2rem;
        }
        .content-section h2 {
            font-size: 2.5rem;
            font-weight: bold;
            color: #1f2937;
            margin-bottom: 1.5rem;
            text-align: center;
        }
        .content-section p, .content-section li {
            font-size: 1.1rem;
            line-height: 1.6;
            color: #4b5563;
            margin-bottom: 1rem;
        }
        .content-section ul {
            list-style: disc;
            margin-left: 1.5rem;
            margin-bottom: 1rem;
        }

        /* Contact Form specific styles */
        .contact-form label {
            display: block;
            font-weight: 600;
            margin-bottom: 0.5rem;
            color: #333;
        }
        .contact-form input[type="text"],
        .contact-form input[type="email"],
        .contact-form textarea {
            width: 100%;
            padding: 0.75rem;
            border: 1px solid #ddd;
            border-radius: 0.375rem;
            margin-bottom: 1.5rem;
            font-size: 1rem;
            transition: border-color 0.2s ease, box-shadow 0.2s ease;
        }
        .contact-form input[type="text"]:focus,
        .contact-form input[type="email"]:focus,
        .contact-form textarea:focus {
            outline: none;
            border-color: #3b82f6;
            box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.2);
        }
        .contact-form textarea {
            min-height: 120px;
            resize: vertical;
        }
        .contact-info {
            margin-top: 2rem;
            padding-top: 1.5rem;
            border-top: 1px solid #eee;
        }
        .contact-info h3 {
            font-size: 1.8rem;
            font-weight: bold;
            color: #1f2937;
            margin-bottom: 1rem;
        }
        .contact-info p {
            display: flex;
            align-items: center;
            margin-bottom: 0.75rem;
        }
        .contact-info p i {
            margin-right: 0.75rem;
            color: #3b82f6;
            font-size: 1.2rem;
        }

        /* Hero Section specific styles */
        .hero-section {
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.7)), url('https://placehold.co/1200x400/000000/FFFFFF?text=Premium+Bags'); /* Dark overlay on image */
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 6rem 1rem; /* Increased padding for a larger feel */
            border-radius: 0.75rem;
            margin-bottom: 2rem;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        .hero-section h2 {
            font-size: 3.5rem; /* Very large heading */
            font-weight: extra-bold;
            margin-bottom: 1rem;
            line-height: 1.2;
            text-shadow: 3px 3px 6px rgba(0, 0, 0, 0.4);
        }
        .hero-section p {
            font-size: 1.5rem; /* Larger paragraph text */
            max-width: 800px;
            margin-bottom: 2rem;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }
        .hero-section .btn-primary {
            padding: 1rem 2.5rem; /* Larger button */
            font-size: 1.25rem;
            border-radius: 0.5rem;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .hero-section .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
        }

        /* Account Modal Specific Styles */
        #account-modal .modal-content {
            max-width: 600px; /* Wider for account options */
            padding: 1.5rem;
            display: flex;
            flex-direction: column;
        }
        .account-options-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 1rem;
            margin-top: 1.5rem;
        }
        .account-option-card {
            border: 1px solid #e0e0e0;
            border-radius: 0.5rem;
            padding: 1rem;
            text-align: left;
            cursor: pointer;
            transition: all 0.2s ease;
        }
        .account-option-card:hover {
            background-color: #f0f8ff;
            border-color: #3b82f6;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
        }
        .account-option-card h4 {
            font-weight: 600;
            font-size: 1.1rem;
            margin-bottom: 0.25rem;
            color: #1f2937;
        }
        .account-option-card p {
            font-size: 0.9rem;
            color: #666;
        }
        .account-section {
            display: none; /* Hidden by default */
            margin-top: 1.5rem;
            padding-top: 1.5rem;
            border-top: 1px solid #eee;
        }
        .account-section.active {
            display: block;
        }
        .account-section h3 {
            font-size: 1.8rem;
            font-weight: bold;
            color: #1f2937;
            margin-bottom: 1rem;
        }
        .account-section .back-button {
            background: none;
            border: none;
            color: #3b82f6;
            cursor: pointer;
            font-size: 1rem;
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
        }
        .account-section .back-button i {
            margin-right: 0.5rem;
        }
        /* Active category button styling */
        .category-button.active {
            background-color: #3b82f6;
            color: white;
            box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
        }

        /* Slideshow Banner specific styles */
        .slideshow-banner {
            position: relative;
            width: 100%;
            height: 400px; /* Fixed height for the banner */
            overflow: hidden;
            background-color: #e0e0e0;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 0.75rem;
            margin-bottom: 2rem;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .slideshow-banner img {
            width: 100%;
            height: 100%;
            object-fit: cover; /* Cover the container, cropping if necessary */
            transition: opacity 0.5s ease-in-out;
            position: absolute;
            top: 0;
            left: 0;
            opacity: 0; /* Hidden by default */
        }
        .slideshow-banner img.active {
            opacity: 1; /* Active image is visible */
        }

        .slideshow-content {
            position: absolute;
            bottom: 1.5rem;
            left: 1.5rem;
            right: 1.5rem;
            background-color: rgba(0, 0, 0, 0.6);
            color: white;
            padding: 1rem 1.5rem;
            border-radius: 0.5rem;
            text-align: left;
            max-width: 60%; /* Limit content width */
            backdrop-filter: blur(5px); /* Frosted glass effect */
            -webkit-backdrop-filter: blur(5px); /* For Safari */
        }

        .slideshow-content h3 {
            font-size: 1.8rem;
            font-weight: bold;
            margin-bottom: 0.5rem;
        }

        .slideshow-content p {
            font-size: 1rem;
            line-height: 1.4;
        }

        .slideshow-nav {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            display: flex;
            justify-content: space-between;
            width: 100%;
            padding: 0 1rem;
        }

        .slideshow-nav button {
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            border: none;
            padding: 0.75rem 1rem;
            border-radius: 50%; /* Circular buttons */
            cursor: pointer;
            font-size: 1.5rem;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }

        .slideshow-nav button:hover {
            background-color: rgba(0, 0, 0, 0.7);
            transform: scale(1.1);
        }

        @media (max-width: 768px) {
            .slideshow-banner {
                height: 300px; /* Smaller height on mobile */
            }
            .slideshow-content {
                max-width: 90%; /* Wider content on mobile */
                bottom: 1rem;
                left: 1rem;
                right: 1rem;
                padding: 0.75rem 1rem;
            }
            .slideshow-content h3 {
                font-size: 1.4rem;
            }
            .slideshow-content p {
                font-size: 0.9rem;
            }
            .slideshow-nav button {
                padding: 0.5rem 0.75rem;
                font-size: 1.2rem;
            }
        }

        /* Floating action buttons */
        .floating-buttons {
            position: fixed;
            bottom: 1.5rem;
            right: 1.5rem;
            display: flex;
            flex-direction: column;
            gap: 1rem;
            z-index: 1000;
        }

        .floating-button {
            background-color: #2563eb; /* Blue */
            color: white;
            border-radius: 9999px; /* Fully rounded */
            width: 56px; /* Standard FAB size */
            height: 56px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: background-color 0.3s ease, transform 0.2s ease;
            cursor: pointer;
        }

        .floating-button:hover {
            background-color: #1d4ed8; /* Darker blue */
            transform: translateY(-2px);
        }

        .floating-button.whatsapp {
            background-color: #25d366; /* WhatsApp green */
        }
        .floating-button.whatsapp:hover {
            background-color: #1da851;
        }

        /* Location display in header */
        .location-display {
            color: #e0e7ff;
            font-size: 0.9rem;
            margin: 0 1rem;
            white-space: nowrap; /* Prevent wrapping */
            overflow: hidden;
            text-overflow: ellipsis;
            max-width: 150px; /* Limit width */
        }

        @media (max-width: 768px) {
            .main-header .flex-grow {
                display: none; /* Hide search bar on small screens in header */
            }
            .main-header .logo-text {
                font-size: 2rem; /* Adjust logo size */
            }
            .main-header .nav-link {
                display: none; /* Hide nav links on mobile */
            }
            .main-header .md\:hidden {
                display: block; /* Show hamburger menu */
            }
            .main-header .space-x-6 {
                margin-left: auto; /* Push icons to the right */
            }
            .location-display {
                display: none; /* Hide location on very small screens if space is tight */
            }
        }
    </style>
</head>
<body class="min-h-screen flex flex-col">
    <header class="main-header">
        <div class="container mx-auto px-4 flex items-center justify-between">
            <div class="flex items-center flex-shrink-0">
                <img src="https://m.media-amazon.com/images/S/al-eu-726f4d26-7fdb/19d6a665-af0c-4fc5-9334-bec41431486e._CR0%2C0%2C588%2C548_SX588_.png" alt="Look N Hook Logo" class="h-12 w-12 mr-4 rounded-lg object-contain">
                <h1 class="logo-text">Look N Hook</h1>
            </div>

            <div id="live-location" class="location-display">
                Fetching location...
            </div>

            <div class="flex-grow flex justify-center items-center mx-4">
                <div class="relative w-full">
                    <input type="text" data-lang-key="searchPlaceholder" placeholder="Search for bags, styles, brands..." class="search-input w-full">
                    <i class="fas fa-search absolute top-1/2 -translate-y-1/2 search-icon"></i>
                </div>
            </div>

            <div class="flex items-center flex-shrink-0 space-x-6">
                <nav class="hidden md:flex space-x-8">
                    <a href="#home" class="nav-link" data-lang-key="home">Home</a>
                    <a href="#shop" class="nav-link" data-lang-key="shop">Shop</a>
                    <a href="#about-us" class="nav-link" data-lang-key="aboutUs">About Us</a>
                    <a href="#contact-us" class="nav-link" data-lang-key="contact">Contact</a>
                    <a href="#my-orders" class="nav-link" data-lang-key="myOrders">My Orders</a>
                </nav>
                <button id="cart-button" class="icon-button relative">
                    <i class="fas fa-shopping-cart text-xl"></i>
                    <span id="cart-count" class="absolute -top-1 -right-1 cart-count text-white text-xs rounded-full h-5 w-5 flex items-center justify-center">0</span>
                </button>
                <button id="user-account-button" class="icon-button">
                    <i class="fas fa-user-circle text-xl"></i>
                </button>
            </div>

            <button class="md:hidden text-white text-2xl">
                <i class="fas fa-bars"></i>
            </button>
        </div>
    </header>

    <section id="slideshow-banner" class="slideshow-banner">
        <img id="slideshow-image" src="" alt="Product Slideshow Image" class="active"
             onerror="this.onerror=null;this.src='https://placehold.co/1200x400/e0e0e0/555555?text=Image+Not+Found';">
        <div class="slideshow-content">
            <h3 id="slideshow-item-code"></h3>
            <p id="slideshow-description"></p>
            <p id="slideshow-price" class="text-2xl font-bold mt-2"></p>
        </div>
        <div class="slideshow-nav">
            <button id="slideshow-prev"><i class="fas fa-chevron-left"></i></button>
            <button id="slideshow-next"><i class="fas fa-chevron-right"></i></button>
        </div>
    </section>

    <main class="flex-grow container mx-auto px-4 py-8">
        <section id="home" class="hero-section">
            <h2 data-lang-key="heroHeading">Your Style, Your Companion.<br>Discover Premium Bags.</h2>
            <p data-lang-key="heroSubheading">Explore our curated collection of exquisite bags, crafted for elegance, durability, and your everyday adventures.</p>
            <button class="btn-primary mt-6 text-lg px-8 py-3" onclick="location.href='#shop'" data-lang-key="shopNowButton">Shop Now</button>
        </section>

        <section id="shop" class="content-section">
            <h2 data-lang-key="ourProducts">Our Products</h2>
            <div class="flex flex-wrap justify-center gap-3 mb-8">
                <button class="btn-secondary category-button active" data-category="All" data-lang-key="categoryAll">All</button>
                <button class="btn-secondary category-button" data-category="Hand Bags" data-lang-key="categoryHandBags">Hand Bags</button>
                <button class="btn-secondary category-button" data-category="Tote Bags" data-lang-key="categoryToteBags">Tote Bags</button>
                <button class="btn-secondary category-button" data-category="Cross Body Bags" data-lang-key="categoryCrossBodyBags">Cross Body Bags</button>
                <button class="btn-secondary category-button" data-category="Shoulder Bags" data-lang-key="categoryShoulderBags">Shoulder Bags</button>
                <button class="btn-secondary category-button" data-category="Duffel Bags" data-lang-key="categoryDuffelBags">Duffel Bags</button>
            </div>
            <div id="products-container" class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-8">
                </div>
        </section>

        <section id="about-us" class="content-section">
            <h2 data-lang-key="aboutUsTitle">About Look N Hook</h2>
            <p data-lang-key="aboutUsPara1">At **Look N Hook**, we believe that a bag is more than just an accessory; it's a statement of style, a companion for your journeys, and a reflection of your personality. Founded with a passion for craftsmanship and design, we are dedicated to providing our customers with a diverse range of high-quality bags that blend functionality with contemporary aesthetics.</p>
            <p data-lang-key="aboutUsPara2">Our journey began with a simple vision: to create bags that not only look good but also stand the test of time. We meticulously select premium materials, primarily durable PU leather, and work with skilled artisans to ensure every stitch and detail meets our rigorous standards. From elegant handbags for daily essentials to spacious travel bags for your adventures, each product in our collection is designed with your needs in mind.</p>
            <p data-lang-key="aboutUsPara3">We are committed to:</p>
            <ul>
                <li data-lang-key="aboutUsCommitment1">**Quality Craftsmanship:** Ensuring every bag is built to last, with attention to detail and robust construction.</li>
                <li data-lang-key="aboutUsCommitment2">**Contemporary Design:** Offering trendy and timeless designs that complement various styles and occasions.</li>
                <li data-lang-key="aboutUsCommitment3">**Customer Satisfaction:** Providing an exceptional shopping experience and products that exceed expectations.</li>
                <li data-lang-key="aboutUsCommitment4">**Ethical Sourcing:** Partnering with suppliers who share our values of responsible production.</li>
            </ul>
            <p data-lang-key="aboutUsPara4">Thank you for choosing Look N Hook. We look forward to being a part of your style journey!</p>
        </section>

        <section id="contact-us" class="content-section">
            <h2 data-lang-key="contactUsTitle">Contact Us</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div>
                    <h3 data-lang-key="sendMessageTitle">Send us a Message</h3>
                    <form id="contact-form" class="contact-form">
                        <label for="contact-name" data-lang-key="yourNameLabel">Your Name</label>
                        <input type="text" id="contact-name" data-lang-key="namePlaceholder" placeholder="Enter your name" required>

                        <label for="contact-email" data-lang-key="yourEmailLabel">Your Email</label>
                        <input type="email" id="contact-email" data-lang-key="emailPlaceholder" placeholder="Enter your email" required>

                        <label for="contact-subject" data-lang-key="subjectLabel">Subject</label>
                        <input type="text" id="contact-subject" data-lang-key="subjectPlaceholder" placeholder="Subject of your message">

                        <label for="contact-message" data-lang-key="messageLabel">Message</label>
                        <textarea id="contact-message" data-lang-key="messagePlaceholder" placeholder="Type your message here..." required></textarea>

                        <button type="submit" class="btn-primary w-full" data-lang-key="sendMessageButton">Send Message</button>
                    </form>
                </div>

                <div class="contact-info">
                    <h3 data-lang-key="ourDetailsTitle">Our Details</h3>
                    <p><i class="fas fa-map-marker-alt"></i> <span data-lang-key="address">M21/2 Batla House, Jamia Nagar New Delhi - 110025 India &#x1F1EE;&#x1F1F3;</span></p>
                    <p><i class="fas fa-phone"></i> <span data-lang-key="phone">7210492296</span></p>
                    <p><i class="fas fa-envelope"></i> <span data-lang-key="emailInfo">looknhook2022@gmail.com</span></p>
                    <p><i class="fas fa-clock"></i> <span data-lang-key="hours">Mon - Sat: 9:00 AM - 6:00 PM</span></p>
                    <div class="mt-6">
                        <h4 data-lang-key="followUs">Follow Us:</h4>
                        <div class="flex space-x-4">
                            <a href="https://www.instagram.com/look_n_hook?igsh=YWt1YXEybng5bDR2" target="_blank" class="text-gray-400 hover:text-pink-400 transition duration-300"><i class="fab fa-instagram text-xl"></i></a>
                            <a href="https://www.amazon.in/stores/page/548B5198-C73A-4F1A-8632-60EE04AC442F?ingress=2&visitId=1074026b-d290-444e-880f-ffbb2bd7c3e8&ref_=ast_bln" target="_blank" class="text-gray-400 hover:text-orange-400 transition duration-300"><i class="fab fa-amazon text-xl"></i></a>
                            <a href="#" target="_blank" class="text-gray-400 hover:text-yellow-400 transition duration-300"><i class="fas fa-shopping-bag text-xl"></i></a> </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <div id="cart-sidebar" class="cart-sidebar">
        <div class="cart-header">
            <h3 class="text-xl font-bold" data-lang-key="yourCart">Your Cart</h3>
            <button id="close-cart-button" class="text-gray-600 hover:text-red-500 text-2xl">&times;</button>
        </div>
        <div id="cart-items-container" class="cart-items">
            <p class="empty-cart-message" data-lang-key="emptyCartMessage">Your cart is empty.</p>
        </div>
        <div id="cart-summary" class="cart-summary">
            <p data-lang-key="total">Total: <span id="cart-total">0 RS/-</span></p>
            <button class="btn-primary w-full mt-4" data-lang-key="checkoutButton">Proceed to Checkout</button>
        </div>
    </div>

    <div id="account-modal" class="modal">
        <div class="modal-content">
            <button id="close-account-modal" class="modal-close-button">&times;</button>
            <h3 class="text-2xl font-bold text-gray-800 mb-6 text-center" id="account-modal-title" data-lang-key="yourAccount">Your Account</h3>

            <div id="account-main-options" class="account-options-grid">
                <div class="account-option-card" data-section="your-orders">
                    <h4><i class="fas fa-box mr-2"></i><span data-lang-key="yourOrders">Your Orders</span></h4>
                    <p data-lang-key="trackOrders">Track, return, or buy things again</p>
                </div>
                <div class="account-option-card" data-section="login-security">
                    <h4><i class="fas fa-lock mr-2"></i><span data-lang-key="loginSecurity">Login & Security</span></h4>
                    <p data-lang-key="editLoginInfo">Edit login, name, and mobile number</p>
                </div>
                <div class="account-option-card" data-section="your-addresses">
                    <h4><i class="fas fa-map-marker-alt mr-2"></i><span data-lang-key="yourAddresses">Your Addresses</span></h4>
                    <p data-lang-key="editAddresses">Edit addresses for orders</p>
                </div>
                <div class="account-option-card" data-section="payment-options">
                    <h4><i class="fas fa-credit-card mr-2"></i><span data-lang-key="paymentOptions">Payment Options</span></h4>
                    <p data-lang-key="managePaymentMethods">Manage payment methods</p>
                </div>
            </div>

            <div id="account-your-orders" class="account-section">
                <button class="back-button" data-target="main-options"><i class="fas fa-arrow-left"></i> <span data-lang-key="backToAccount">Back to Your Account</span></button>
                <h3 data-lang-key="yourOrders">Your Orders</h3>
                <p data-lang-key="noOrdersYet">You have no orders yet.</p>
            </div>

            <div id="account-login-security" class="account-section">
                <button class="back-button" data-target="main-options"><i class="fas fa-arrow-left"></i> <span data-lang-key="backToAccount">Back to Your Account</span></button>
                <h3 data-lang-key="loginSecurity">Login & Security</h3>
                <div id="login-message-box" class="message-box"></div>
                <input type="email" id="login-email" data-lang-key="emailPlaceholder" placeholder="Email" class="modal-input" required>
                <input type="password" id="login-password" data-lang-key="passwordPlaceholder" placeholder="Password" class="modal-input" required>
                <div class="modal-button-group">
                    <button id="login-btn" class="btn-primary btn" data-lang-key="loginButton">Login</button>
                    <button id="register-btn" class="btn-secondary btn" data-lang-key="registerButton">Register</button>
                </div>
            </div>

            <div id="account-your-addresses" class="account-section">
                <button class="back-button" data-target="main-options"><i class="fas fa-arrow-left"></i> <span data-lang-key="backToAccount">Back to Your Account</span></button>
                <h3 data-lang-key="yourAddresses">Your Addresses</h3>
                <p data-lang-key="noAddressesYet">No addresses saved. Add a new address to get started.</p>
                <button class="btn-primary w-full mt-4" data-lang-key="addNewAddress">Add New Address</button>
            </div>

            <div id="account-payment-options" class="account-section">
                <button class="back-button" data-target="main-options"><i class="fas fa-arrow-left"></i> <span data-lang-key="backToAccount">Back to Your Account</span></button>
                <h3 data-lang-key="paymentOptions">Payment Options</h3>
                <p data-lang-key="noPaymentMethods">No payment methods saved.</p>
                <button class="btn-primary w-full mt-4" data-lang-key="addPaymentMethod">Add Payment Method</button>
            </div>

        </div>
    </div>

    <div id="product-detail-modal" class="modal">
        <div class="modal-content">
            <button id="close-product-detail-modal" class="modal-close-button">&times;</button>
            
            <div class="product-image-section">
                <img id="product-detail-image" src="" alt="Product Image" class="product-detail-image">
                <button id="prev-image-button" class="slideshow-nav-button prev">&#10094;</button>
                <button id="next-image-button" class="slideshow-nav-button next">&#10095;</button>
                <div id="product-thumbnail-gallery" class="thumbnail-gallery">
                    </div>
            </div>

            <div class="product-info-section">
                <h3 id="product-detail-item-code"></h3>
                <div class="rating">
                    <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="far fa-star"></i> (4.0 out of 5) </div>
                <p><strong data-lang-key="descriptionLabel">Description:</strong> <span id="product-detail-description"></span></p>
                <p><strong data-lang-key="sizeLabel">Size:</strong> <span id="product-detail-size"></span></p>
                <p class="text-green-600 text-lg font-semibold mt-2" data-lang-key="inStock">In Stock</p> <p class="price" id="product-detail-price"></p>

                <div class="quantity-selector">
                    <label for="product-quantity" class="font-semibold" data-lang-key="quantityLabel">Quantity:</label>
                    <input type="number" id="product-quantity" value="1" min="1" class="modal-input">
                </div>

                <button id="add-to-cart-detail-btn" class="btn-primary add-to-cart-detail-btn" data-lang-key="addToCartButton">Add to Cart</button>
                <button class="btn-secondary w-full mt-2" data-lang-key="buyNowButton">Buy Now</button> <div class="product-description-section">
                    <h4 data-lang-key="aboutThisItem">About this item</h4>
                    <ul id="product-about-list">
                        <li data-lang-key="itemFeature1">Made from high-quality PU leather.</li>
                        <li data-lang-key="itemFeature2">Suitable for office and casual use.</li>
                        <li data-lang-key="itemFeature3">Zipper closure and a large pocket.</li>
                        <li data-lang-key="itemFeature4">Made in India.</li>
                    </ul>
                </div>

                <div class="product-technical-details-section">
                    <h4 data-lang-key="technicalDetails">Technical Details</h4>
                    <ul id="product-technical-list">
                        <li><strong data-lang-key="techItemCode">Item Code:</strong> <span id="tech-item-code"></span></li>
                        <li><strong data-lang-key="techMaterial">Material:</strong> <span id="tech-material"></span></li>
                        <li><strong data-lang-key="techSize">Size:</strong> <span id="tech-size"></span></li>
                        <li><strong data-lang-key="techPockets">Number of Pockets:</strong> 1</li>
                        <li><strong data-lang-key="techClosure">Closure:</strong> Zipper</li>
                        <li><strong data-lang-key="techOccasion">Occasion:</strong> Casual, Office</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>

    <footer class="bg-gray-800 text-white py-8 mt-auto">
        <div class="container mx-auto px-4 text-center">
            <div class="flex flex-wrap justify-center space-x-6 mb-4">
                <a href="#" class="hover:text-blue-400 transition duration-300" data-lang-key="privacyPolicy">Privacy Policy</a>
                <a href="#" class="hover:text-blue-400 transition duration-300" data-lang-key="termsConditions">Terms & Conditions</a>
                <a href="#" class="hover:text-blue-400 transition duration-300" data-lang-key="faq">FAQ</a>
                <a href="#" class="hover:text-blue-400 transition duration-300" data-lang-key="shipping">Shipping</a>
            </div>
            <div class="flex justify-center space-x-6 mb-4">
                <a href="https://www.instagram.com/look_n_hook?igsh=YWt1YXEybng5bDR2" target="_blank" class="text-gray-400 hover:text-pink-400 transition duration-300"><i class="fab fa-instagram text-xl"></i></a>
                <a href="https://www.amazon.in/stores/page/548B5198-C73A-4F1A-8632-60EE04AC442F?ingress=2&visitId=1074026b-d290-444e-880f-ffbb2bd7c3e8&ref_=ast_bln" target="_blank" class="text-gray-400 hover:text-orange-400 transition duration-300"><i class="fab fa-amazon text-xl"></i></a>
                <a href="#" target="_blank" class="text-gray-400 hover:text-yellow-400 transition duration-300"><i class="fas fa-shopping-bag text-xl"></i></a>
            </div>
            <p>&copy; 2024 Look N Hook. <span data-lang-key="allRightsReserved">All rights reserved.</span></p>
        </div>
    </footer>

    <div class="floating-buttons">
        <a href="https://wa.me/7210492296" target="_blank" class="floating-button whatsapp" title="Chat on WhatsApp">
            <i class="fab fa-whatsapp"></i>
        </a>
        <a href="tel:7210492296" class="floating-button" title="Call Us">
            <i class="fas fa-phone"></i>
        </a>
    </div>

    <script>
        // Language content object
        const translations = {
            en: {
                searchPlaceholder: "Search for bags, styles, brands...",
                home: "Home",
                shop: "Shop",
                aboutUs: "About Us",
                contact: "Contact",
                myOrders: "My Orders",
                heroHeading: "Your Style, Your Companion.<br>Discover Premium Bags.",
                heroSubheading: "Explore our curated collection of exquisite bags, crafted for elegance, durability, and your everyday adventures.",
                shopNowButton: "Shop Now",
                ourProducts: "Our Products",
                categoryAll: "All",
                categoryHandBags: "Hand Bags",
                categoryToteBags: "Tote Bags",
                categoryCrossBodyBags: "Cross Body Bags",
                categoryShoulderBags: "Shoulder Bags",
                categoryDuffelBags: "Duffel Bags",
                aboutUsTitle: "About Look N Hook",
                aboutUsPara1: "At **Look N Hook**, we believe that a bag is more than just an accessory; it's a statement of style, a companion for your journeys, and a reflection of your personality. Founded with a passion for craftsmanship and design, we are dedicated to providing our customers with a diverse range of high-quality bags that blend functionality with contemporary aesthetics.",
                aboutUsPara2: "Our journey began with a simple vision: to create bags that not only look good but also stand the test of time. We meticulously select premium materials, primarily durable PU leather, and work with skilled artisans to ensure every stitch and detail meets our rigorous standards. From elegant handbags for daily essentials to spacious travel bags for your adventures, each product in our collection is designed with your needs in mind.",
                aboutUsPara3: "We are committed to:",
                aboutUsCommitment1: "**Quality Craftsmanship:** Ensuring every bag is built to last, with attention to detail and robust construction.",
                aboutUsCommitment2: "**Contemporary Design:** Offering trendy and timeless designs that complement various styles and occasions.",
                aboutUsCommitment3: "**Customer Satisfaction:** Providing an exceptional shopping experience and products that exceed expectations.",
                aboutUsCommitment4: "**Ethical Sourcing:** Partnering with suppliers who share our values of responsible production.",
                aboutUsPara4: "Thank you for choosing Look N Hook. We look forward to being a part of your style journey!",
                contactUsTitle: "Contact Us",
                sendMessageTitle: "Send us a Message",
                yourNameLabel: "Your Name",
                namePlaceholder: "Enter your name",
                yourEmailLabel: "Your Email",
                emailPlaceholder: "Enter your email",
                subjectLabel: "Subject",
                subjectPlaceholder: "Subject of your message",
                messageLabel: "Message",
                messagePlaceholder: "Type your message here...",
                sendMessageButton: "Send Message",
                ourDetailsTitle: "Our Details",
                address: "M21/2 Batla House, Jamia Nagar New Delhi - 110025 India \uD83C\uDDEE\uD83C\uDDF3", // Updated address with flag
                phone: "7210492296", // Updated phone number
                emailInfo: "looknhook2022@gmail.com", // Updated email
                hours: "Mon - Sat: 9:00 AM - 6:00 PM",
                followUs: "Follow Us:",
                yourCart: "Your Cart",
                emptyCartMessage: "Your cart is empty.",
                total: "Total:",
                checkoutButton: "Proceed to Checkout",
                yourAccount: "Your Account",
                trackOrders: "Track, return, or buy things again",
                loginSecurity: "Login & Security",
                editLoginInfo: "Edit login, name, and mobile number",
                yourAddresses: "Your Addresses",
                editAddresses: "Edit addresses for orders",
                paymentOptions: "Payment Options",
                managePaymentMethods: "Manage payment methods",
                backToAccount: "Back to Your Account",
                noOrdersYet: "You have no orders yet.",
                noAddressesYet: "No addresses saved. Add a new address to get started.",
                addNewAddress: "Add New Address",
                noPaymentMethods: "No payment methods saved.",
                addPaymentMethod: "Add Payment Method",
                loginSuccessful: "Login successful!",
                invalidCredentials: "Invalid email or password.",
                enterEmailPassword: "Please enter both email and password.",
                registrationSuccessful: "Registration successful! You can now log in.",
                descriptionLabel: "Description:",
                sizeLabel: "Size:",
                inStock: "In Stock",
                quantityLabel: "Quantity:",
                addToCartButton: "Add to Cart",
                buyNowButton: "Buy Now",
                aboutThisItem: "About this item",
                itemFeature1: "Made from high-quality PU leather.",
                itemFeature2: "Suitable for office and casual use.",
                itemFeature3: "Zipper closure and a large pocket.",
                itemFeature4: "Made in India.",
                technicalDetails: "Technical Details",
                techItemCode: "Item Code:",
                techMaterial: "Material:",
                techSize: "Size:",
                techPockets: "Number of Pockets:",
                techClosure: "Closure:",
                techOccasion: "Occasion:",
                allRightsReserved: "All rights reserved."
            }
        };

        let currentLanguage = 'en'; // Default language

        // Function to update text content based on selected language
        function updateContentLanguage() {
            document.querySelectorAll('[data-lang-key]').forEach(element => {
                const key = element.getAttribute('data-lang-key');
                if (translations[currentLanguage] && translations[currentLanguage][key]) {
                    // Handle innerHTML for elements that might contain HTML (like heroHeading)
                    if (key === 'heroHeading' || key.startsWith('aboutUsPara') || key.startsWith('aboutUsCommitment')) {
                        element.innerHTML = translations[currentLanguage][key];
                    } else if (element.tagName === 'INPUT' || element.tagName === 'TEXTAREA') {
                        element.placeholder = translations[currentLanguage][key];
                    } else {
                        element.textContent = translations[currentLanguage][key];
                    }
                }
            });
        }

        // Array of product objects - Updated with categories
        const products = [
            {
                "Item Code": "LHN001/24",
                "Description": "PU",
                "Size": "H9.25XL11.5\"XW4\"",
                "Price": "680 RS/-",
                "Image": [
                    "https://i.ibb.co/fzzyKhv8/PU-SELECTED-BAGS-1.jpg",
                    "https://i.ibb.co/97FfzMv/PU-SELECTED-BAGS-2.jpg",
                    "https://i.ibb.co/bjGGcysM/PU-SELECTED-BAGS-3.jpg"
                ],
                "Category": "Hand Bags"
            },
            {
                "Item Code": "LHN002/24",
                "Description": "PU",
                "Size": "H9.25XL11.5\"XW4\"",
                "Price": "780 RS/-",
                "Image": ["https://i.ibb.co/1kDphSn/PU-SELECTED-BAGS-2.jpg", "https://i.ibb.co/mC2hPBrX/PU-SELECTED-BAGS-7.jpg"],
                "Category": "Tote Bags"
            },
            {
                "Item Code": "LHN03/24",
                "Description": "PU",
                "Size": "H6XL9\"XW3\"",
                "Price": "650 RS/-",
                "Image": ["https://i.ibb.co/bjGGcysM/PU-SELECTED-BAGS-3.jpg", "https://i.ibb.co/ZztBFrct/PU-SELECTED-BAGS-9.jpg"],
                "Category": "Cross Body Bags"
            },
            {
                "Item Code": "LHN04/24",
                "Description": "PU",
                "Size": "H7.5XL8.5\"XW4.5\"",
                "Price": "630 RS/-",
                "Image": ["https://i.ibb.co/nq5NFJDP/PU-SELECTED-BAGS-4.jpg"],
                "Category": "Shoulder Bags"
            },
            {
                "Item Code": "LHN005/24",
                "Description": "PU",
                "Size": "H 4.5XL 7.5\"XW 3\"",
                "Price": "550 RS/-",
                "Image": ["https://i.ibb.co/rY9Z0KQ/PU-SELECTED-BAGS-5.jpg"],
                "Category": "Hand Bags"
            },
            {
                "Item Code": "LHN006/24",
                "Description": "PU",
                "Size": "H8XL11\"XW4\"",
                "Price": "680 RS/-",
                "Image": ["https://i.ibb.co/qYYCpj3K/PU-SELECTED-BAGS-6.jpg"],
                "Category": "Tote Bags"
            },
            {
                "Item Code": "LHN007/24",
                "Description": "PU",
                "Size": "H8.5XL11.5\"XW4.5\"",
                "Price": "680 RS/-",
                "Image": ["https://i.ibb.co/mC2hPBrX/PU-SELECTED-BAGS-7.jpg"],
                "Category": "Cross Body Bags"
            },
            {
                "Item Code": "LHN008/24",
                "Description": "PU",
                "Size": "H8.5XL11.5\"XW4.5\"",
                "Price": "780 RS/-",
                "Image": ["https://i.ibb.co/HDrq8Q60/PU-SELECTED-BAGS-8.jpg"],
                "Category": "Shoulder Bags"
            },
            {
                "Item Code": "LHN009/24",
                "Description": "PU",
                "Size": "H 6.5XL 10.5\"XW 3\"",
                "Price": "650 RS/-",
                "Image": ["https://i.ibb.co/ZztBFrct/PU-SELECTED-BAGS-9.jpg"],
                "Category": "Hand Bags"
            },
            {
                "Item Code": "LHN010/24",
                "Description": "PU",
                "Size": "H 6.5XL 10.5\"XW 3\"",
                "Price": "750 RS/-",
                "Image": ["https://i.ibb.co/Rk6WvRMh/PU-SELECTED-BAGS-10.jpg"],
                "Category": "Tote Bags"
            },
            {
                "Item Code": "LHN011/24",
                "Description": "PU",
                "Size": "H 8.5XL 10.5\"XW 4\"",
                "Price": "680 RS/-",
                "Image": ["https://i.ibb.co/QZ3Nw0g/PU-SELECTED-BAGS-11.jpg"],
                "Category": "Cross Body Bags"
            },
            {
                "Item Code": "LHN012/24",
                "Description": "PU",
                "Size": "H 8.5XL 10.5\"XW 4\"",
                "Price": "780 RS/-",
                "Image": ["https://i.ibb.co/x8PXLwKp/PU-SELECTED-BAGS-12.jpg"],
                "Category": "Shoulder Bags"
            },
            {
                "Item Code": "LHN013/24",
                "Description": "PU",
                "Size": "H 9\"XL 15.5\"XW 6\"",
                "Price": "825 RS/-",
                "Image": ["https://i.ibb.co/ymYGMyqs/PU-SELECTED-BAGS-13.jpg"],
                "Category": "Duffel Bags"
            },
            {
                "Item Code": "LHN014/24",
                "Description": "PU",
                "Size": "H 9\"XL 15.5\"XW 6\"",
                "Price": "925 RS/-",
                "Image": ["https://i.ibb.co/B5kRx7DR/PU-SELECTED-BAGS-14.jpg"],
                "Category": "Duffel Bags"
            },
            {
                "Item Code": "LHN015/24",
                "Description": "PU",
                "Size": "H 9.5\"XL 17.5\"XW 6\"",
                "Price": "925 RS/-",
                "Image": ["https://i.ibb.co/4wLDFMDb/PU-SELECTED-BAGS-15.jpg"],
                "Category": "Hand Bags"
            },
            {
                "Item Code": "LHN016/24",
                "Description": "PU",
                "Size": "H12.5XL15\"XW2\"",
                "Price": "725 RS/-",
                "Image": ["https://i.ibb.co/cXcdktXx/PU-SELECTED-BAGS-16.jpg"],
                "Category": "Tote Bags"
            },
            {
                "Item Code": "LHN017/24",
                "Description": "PU",
                "Size": "H12XL10.7\"XW6\"",
                "Price": "625 RS/-",
                "Image": ["https://i.ibb.co/20qrn1VJ/PU-SELECTED-BAGS-17.jpg"],
                "Category": "Cross Body Bags"
            },
            {
                "Item Code": "LHN018/24",
                "Description": "PU",
                "Size": "H12 XL10.70\"XW6.50\"",
                "Price": "625 RS/-",
                "Image": ["https://i.ibb.co/N2N94LSG/PU-SELECTED-BAGS-18.jpg"],
                "Category": "Shoulder Bags"
            },
            {
                "Item Code": "LHN019/24",
                "Description": "PU",
                "Size": "H 8\"XL 11\"XW 4\"",
                "Price": "650 RS/-",
                "Image": ["https://i.ibb.co/GD1GmgZ/PU-SELECTED-BAGS-19.jpg"],
                "Category": "Duffel Bags"
            }
        ];

        // Get references to DOM elements
        const productsContainer = document.getElementById('products-container');
        const cartSidebar = document.getElementById('cart-sidebar');
        const cartButton = document.getElementById('cart-button');
        const closeCartButton = document.getElementById('close-cart-button');
        const cartItemsContainer = document.getElementById('cart-items-container');
        const cartTotalSpan = document.getElementById('cart-total');
        const cartCountSpan = document.getElementById('cart-count');

        // Account Modal Elements
        const userAccountButton = document.getElementById('user-account-button');
        const accountModal = document.getElementById('account-modal');
        const closeAccountModalButton = document.getElementById('close-account-modal');
        const accountMainOptions = document.getElementById('account-main-options');
        const accountSections = document.querySelectorAll('.account-section');
        const accountModalTitle = document.getElementById('account-modal-title');

        // Login/Register elements within Account Modal
        const loginEmailInput = document.getElementById('login-email');
        const loginPasswordInput = document.getElementById('login-password');
        const loginBtn = document.getElementById('login-btn');
        const registerBtn = document.getElementById('register-btn');
        const loginMessageBox = document.getElementById('login-message-box'); // Reused for account modal messages

        // Product Detail Modal Elements
        const productDetailModal = document.getElementById('product-detail-modal');
        const closeProductDetailModalButton = document.getElementById('close-product-detail-modal');
        const productDetailImage = document.getElementById('product-detail-image');
        const productThumbnailGallery = document.getElementById('product-thumbnail-gallery');
        const productDetailItemCode = document.getElementById('product-detail-item-code');
        const productDetailDescription = document.getElementById('product-detail-description');
        const productDetailSize = document.getElementById('product-detail-size');
        const productDetailPrice = document.getElementById('product-detail-price');
        const addToCartDetailBtn = document.getElementById('add-to-cart-detail-btn');
        const productQuantityInput = document.getElementById('product-quantity');
        const productAboutList = document.getElementById('product-about-list');
        const productTechnicalList = document.getElementById('product-technical-list');
        const techItemCode = document.getElementById('tech-item-code');
        const techMaterial = document.getElementById('tech-material');
        const techSize = document.getElementById('tech-size');

        // Slideshow navigation elements for product details
        const prevImageButton = document.getElementById('prev-image-button');
        const nextImageButton = document.getElementById('next-image-button');

        // Global variables for current product images and index (for product detail modal)
        let currentProductImages = [];
        let currentImageIndex = 0;

        // Slideshow banner elements
        const slideshowBanner = document.getElementById('slideshow-banner');
        const slideshowImage = document.getElementById('slideshow-image');
        const slideshowItemCode = document.getElementById('slideshow-item-code');
        const slideshowDescription = document.getElementById('slideshow-description');
        const slideshowPrice = document.getElementById('slideshow-price');
        const slideshowPrevBtn = document.getElementById('slideshow-prev');
        const slideshowNextBtn = document.getElementById('slideshow-next');

        let currentSlideIndex = 0; // Current index for the banner slideshow
        let slideshowInterval; // Variable to hold the interval for autoplay

        // Initialize an empty cart array
        let cart = [];

        // Live Location Element
        const liveLocationDisplay = document.getElementById('live-location');
        const contactForm = document.getElementById('contact-form');

        // Function to display a specific slide in the banner slideshow
        function showBannerSlide(index) {
            // Ensure index is within bounds
            currentSlideIndex = (index + products.length) % products.length;
            const product = products[currentSlideIndex];

            // Update image and text content
            slideshowImage.src = Array.isArray(product.Image) ? product.Image[0] : product.Image;
            slideshowItemCode.textContent = product['Item Code'];
            slideshowDescription.textContent = product.Description;
            slideshowPrice.textContent = product.Price;

            // Restart autoplay timer
            resetSlideshowAutoplay();
        }

        // Function to go to the next slide in the banner slideshow
        function nextBannerSlide() {
            showBannerSlide(currentSlideIndex + 1);
        }

        // Function to go to the previous slide in the banner slideshow
        function prevBannerSlide() {
            showBannerSlide(currentSlideIndex - 1);
        }

        // Function to reset the autoplay timer
        function resetSlideshowAutoplay() {
            clearInterval(slideshowInterval); // Clear existing interval
            slideshowInterval = setInterval(nextBannerSlide, 5000); // Set new interval for 5 seconds
        }

        // Event listeners for banner slideshow navigation
        slideshowPrevBtn.addEventListener('click', prevBannerSlide);
        slideshowNextBtn.addEventListener('click', nextBannerSlide);


        // Function to render products on the page, with category filtering
        function renderProducts(category = 'All') {
            productsContainer.innerHTML = ''; // Clear existing products
            const filteredProducts = category === 'All' ? products : products.filter(p => p.Category === category);

            if (filteredProducts.length === 0) {
                productsContainer.innerHTML = `<p class="text-center text-gray-600 text-xl col-span-full" data-lang-key="noProductsInCategory">No products available in this category.</p>`;
            } else {
                filteredProducts.forEach(product => {
                    const imageSrc = Array.isArray(product.Image) ? product.Image[0] : product.Image;

                    const productCard = document.createElement('div');
                    productCard.classList.add('bg-white', 'rounded-xl', 'shadow-md', 'p-6', 'text-center', 'flex', 'flex-col', 'justify-between', 'transform', 'transition', 'duration-300', 'hover:scale-105', 'hover:shadow-lg', 'cursor-pointer');

                    productCard.innerHTML = `
                        <img src="${imageSrc}" alt="${product['Item Code']} - ${product.Description}"
                             class="max-w-full h-48 object-contain mb-4 rounded-lg mx-auto"
                             onerror="this.onerror=null;this.src='https://placehold.co/400x400/e0e0e0/555555?text=Image+Not+Found';">
                        <h3 class="text-xl font-semibold text-gray-800 mb-2">${product['Item Code']}</h3>
                        <p class="text-gray-600 mb-1" data-lang-key="descriptionLabel"><strong>Description:</strong> ${product.Description}</p>
                        <p class="text-600 mb-3" data-lang-key="sizeLabel"><strong>Size:</strong> ${product.Size}</p>
                        <p class="text-2xl font-bold text-blue-600 mb-4">${product.Price}</p>
                        <button class="btn-primary w-full add-to-cart-btn" data-item-code="${product['Item Code']}" data-lang-key="addToCartButton">Add to Cart</button>
                    `;
                    productsContainer.appendChild(productCard);

                    productCard.addEventListener('click', (event) => {
                        if (!event.target.classList.contains('add-to-cart-btn')) {
                            openProductDetailsModal(product);
                        }
                    });
                });
            }

            // Update active state for category buttons
            document.querySelectorAll('.category-button').forEach(button => {
                if (button.dataset.category === category) {
                    button.classList.add('active');
                } else {
                    button.classList.remove('active');
                }
            });

            // Attach event listeners to "Add to Cart" buttons after rendering
            document.querySelectorAll('.add-to-cart-btn').forEach(button => {
                button.addEventListener('click', addToCart);
            });
            updateContentLanguage(); // Apply language to newly rendered product cards
        }

        // Event listeners for category buttons
        document.querySelectorAll('.category-button').forEach(button => {
            button.addEventListener('click', () => {
                const category = button.dataset.category;
                renderProducts(category);
            });
        });


        // Function to add item to cart
        function addToCart(event) {
            const itemCode = event.target.dataset.itemCode;
            const quantity = parseInt(productQuantityInput.value) || 1;
            const productToAdd = products.find(p => p['Item Code'] === itemCode);

            if (productToAdd) {
                const existingItem = cart.find(item => item['Item Code'] === itemCode);
                if (existingItem) {
                    existingItem.quantity += quantity;
                } else {
                    const imageForCart = Array.isArray(productToAdd.Image) ? productToAdd.Image[0] : productToAdd.Image;
                    cart.push({ ...productToAdd, Image: imageForCart, quantity: quantity });
                }
                updateCartUI();
                openCartSidebar();
            }
        }

        // Function to remove item from cart
        function removeFromCart(event) {
            const itemCodeToRemove = event.target.dataset.itemCode;
            cart = cart.filter(item => item['Item Code'] !== itemCodeToRemove);
            updateCartUI();
        }

        // Function to update the cart UI
        function updateCartUI() {
            cartItemsContainer.innerHTML = '';
            let total = 0;

            if (cart.length === 0) {
                cartItemsContainer.innerHTML = `<p class="empty-cart-message" data-lang-key="emptyCartMessage">Your cart is empty.</p>`;
            } else {
                cart.forEach(item => {
                    const itemPrice = parseFloat(item.Price.replace(' RS/-', ''));
                    total += itemPrice * item.quantity;

                    const cartItemDiv = document.createElement('div');
                    cartItemDiv.classList.add('cart-item');
                    cartItemDiv.innerHTML = `
                        <img src="${item.Image}" alt="${item['Item Code']}" onerror="this.onerror=null;this.src='https://placehold.co/60x60/cccccc/333333?text=Bag';">
                        <div class="cart-item-details">
                            <h4>${item['Item Code']}</h4>
                            <p>${item.Price} x ${item.quantity}</p>
                        </div>
                        <button class="cart-item-remove" data-item-code="${item['Item Code']}">
                            <i class="fas fa-trash-alt"></i>
                        </button>
                    `;
                    cartItemsContainer.appendChild(cartItemDiv);
                });
                document.querySelectorAll('.cart-item-remove').forEach(button => {
                    button.addEventListener('click', removeFromCart);
                });
            }

            cartTotalSpan.textContent = `${total} RS/-`;
            cartCountSpan.textContent = cart.reduce((sum, item) => sum + item.quantity, 0);
            updateContentLanguage(); // Apply language to cart UI
        }

        // Function to open the cart sidebar
        function openCartSidebar() {
            cartSidebar.classList.add('open');
        }

        // Function to close the cart sidebar
        function closeCartSidebar() {
            cartSidebar.classList.remove('open');
        }

        // Function to show message in login/account modal
        function showAccountMessage(message, isError = false) {
            loginMessageBox.textContent = message;
            loginMessageBox.classList.remove('error', 'show');
            if (isError) {
                loginMessageBox.classList.add('error');
            }
            loginMessageBox.classList.add('show');
            setTimeout(() => {
                loginMessageBox.classList.remove('show');
            }, 3000);
        }

        // Function to handle login
        function handleLogin() {
            const email = loginEmailInput.value;
            const password = loginPasswordInput.value;

            if (email === "" || password === "") {
                showAccountMessage(translations[currentLanguage].enterEmailPassword, true);
                return;
            }

            if (email === "test@example.com" && password === "password123") {
                showAccountMessage(translations[currentLanguage].loginSuccessful);
            } else {
                showAccountMessage(translations[currentLanguage].invalidCredentials, true);
            }
        }

        // Function to handle registration
        function handleRegister() {
            const email = loginEmailInput.value;
            const password = loginPasswordInput.value;

            if (email === "" || password === "") {
                showAccountMessage(translations[currentLanguage].enterEmailPassword, true);
                return;
            }

            showAccountMessage(translations[currentLanguage].registrationSuccessful);
            loginEmailInput.value = '';
            loginPasswordInput.value = '';
        }

        // Function to update the main product image and active thumbnail
        function updateMainImage(index) {
            if (currentProductImages.length === 0) return;

            currentImageIndex = (index + currentProductImages.length) % currentProductImages.length;
            productDetailImage.src = currentProductImages[currentImageIndex];

            document.querySelectorAll('#product-thumbnail-gallery img').forEach((thumb, idx) => {
                if (idx === currentImageIndex) {
                    thumb.classList.add('active');
                } else {
                    thumb.classList.remove('active');
                }
            });
        }

        // Function to open product details modal
        function openProductDetailsModal(product) {
            productDetailItemCode.textContent = product['Item Code'];
            productDetailDescription.textContent = product.Description;
            productDetailSize.textContent = product.Size;
            productDetailPrice.textContent = product.Price;
            
            addToCartDetailBtn.dataset.itemCode = product['Item Code'];
            productQuantityInput.value = 1;

            techItemCode.textContent = product['Item Code'];
            techMaterial.textContent = product.Description;
            techSize.textContent = product.Size;

            productThumbnailGallery.innerHTML = '';

            currentProductImages = Array.isArray(product.Image) ? product.Image : [product.Image];
            currentImageIndex = 0;

            currentProductImages.forEach((imgUrl, index) => {
                const thumbnail = document.createElement('img');
                thumbnail.src = imgUrl;
                thumbnail.alt = `Thumbnail ${index + 1}`;
                thumbnail.classList.add('rounded-md', 'cursor-pointer', 'border-2', 'border-transparent', 'transition', 'duration-200');
                thumbnail.addEventListener('click', () => updateMainImage(index));
                productThumbnailGallery.appendChild(thumbnail);
            });

            updateMainImage(currentImageIndex);

            productDetailModal.classList.add('open');
            updateContentLanguage(); // Ensure product modal text is updated
        }

        // Function to close product details modal
        function closeProductDetailsModal() {
            productDetailModal.classList.remove('open');
        }

        // Event listeners for cart button and close button
        cartButton.addEventListener('click', openCartSidebar);
        closeCartButton.addEventListener('click', closeCartSidebar);

        // Event listeners for Account Modal
        userAccountButton.addEventListener('click', () => {
            accountModal.classList.add('open');
            showAccountSection('main-options'); // Show main options when modal opens
            loginMessageBox.classList.remove('show'); // Hide any previous messages
        });
        closeAccountModalButton.addEventListener('click', () => {
            accountModal.classList.remove('open');
        });

        // Handle clicks on account option cards
        document.querySelectorAll('.account-option-card').forEach(card => {
            card.addEventListener('click', (event) => {
                const section = event.currentTarget.dataset.section;
                showAccountSection(section);
            });
        });

        // Handle clicks on back buttons in account sections
        document.querySelectorAll('.account-section .back-button').forEach(button => {
            button.addEventListener('click', (event) => {
                const targetSection = event.currentTarget.dataset.target;
                showAccountSection(targetSection);
            });
        });

        // Function to show a specific account section
        function showAccountSection(sectionId) {
            accountSections.forEach(section => {
                section.classList.remove('active');
            });
            accountMainOptions.classList.add('hidden'); // Hide main options when a sub-section is active

            if (sectionId === 'main-options') {
                accountMainOptions.classList.remove('hidden'); // Show main options
                accountModalTitle.textContent = translations[currentLanguage].yourAccount;
            } else {
                document.getElementById(`account-${sectionId}`).classList.add('active');
                // Update modal title based on the active section
                if (sectionId === 'your-orders') accountModalTitle.textContent = translations[currentLanguage].yourOrders;
                if (sectionId === 'login-security') accountModalTitle.textContent = translations[currentLanguage].loginSecurity;
                if (sectionId === 'your-addresses') accountModalTitle.textContent = translations[currentLanguage].yourAddresses;
                if (sectionId === 'payment-options') accountModalTitle.textContent = translations[currentLanguage].paymentOptions;
            }
            updateContentLanguage(); // Re-apply language after changing section
        }


        loginBtn.addEventListener('click', handleLogin);
        registerBtn.addEventListener('click', handleRegister);

        // Event listener for product detail modal close button
        closeProductDetailModalButton.addEventListener('click', closeProductDetailsModal);

        // Event listeners for slideshow navigation buttons
        prevImageButton.addEventListener('click', () => updateMainImage(currentImageIndex - 1));
        nextImageButton.addEventListener('click', () => updateMainImage(currentImageIndex + 1));

        // Event listener for "Add to Cart" button inside product detail modal
        addToCartDetailBtn.addEventListener('click', (event) => {
            const itemCode = event.target.dataset.itemCode;
            const quantity = parseInt(productQuantityInput.value) || 1;
            const productToAdd = products.find(p => p['Item Code'] === itemCode);
            if (productToAdd) {
                const imageForCart = Array.isArray(productToAdd.Image) ? productToAdd.Image[0] : productToAdd.Image;
                const existingItem = cart.find(item => item['Item Code'] === itemCode);
                if (existingItem) {
                    existingItem.quantity += quantity;
                } else {
                    cart.push({ ...productToAdd, Image: imageForCart, quantity: quantity });
                }
                updateCartUI();
                openCartSidebar();
                closeProductDetailsModal();
            }
        });

        // WhatsApp integration for contact form
        contactForm.addEventListener('submit', function(event) {
            event.preventDefault(); // Prevent default form submission

            const name = document.getElementById('contact-name').value;
            const email = document.getElementById('contact-email').value;
            const subject = document.getElementById('contact-subject').value;
            const message = document.getElementById('contact-message').value;

            const phoneNumber = "7210492296"; // Your WhatsApp number
            const whatsappMessage = `Hello Look N Hook,\n\nName: ${name}\nEmail: ${email}\nSubject: ${subject}\n\nMessage: ${message}`;
            const whatsappUrl = `https://wa.me/${phoneNumber}?text=${encodeURIComponent(whatsappMessage)}`;

            window.open(whatsappUrl, '_blank'); // Open WhatsApp in a new tab/window
        });

        // Function to get user's live location
        function getLiveLocation() {
            if (navigator.geolocation) {
                navigator.geolocation.getCurrentPosition(
                    async (position) => {
                        const lat = position.coords.latitude;
                        const lon = position.coords.longitude;
                        
                        try {
                            // Using OpenStreetMap Nominatim for reverse geocoding
                            const response = await fetch(`https://nominatim.openstreetmap.org/reverse?format=json&lat=${lat}&lon=${lon}&zoom=10`);
                            const data = await response.json();

                            if (data.address) {
                                const city = data.address.city || data.address.town || data.address.village || '';
                                const state = data.address.state || data.address.province || '';
                                if (city && state) {
                                    liveLocationDisplay.textContent = `${city}, ${state}`;
                                } else if (city) {
                                    liveLocationDisplay.textContent = city;
                                } else if (state) {
                                    liveLocationDisplay.textContent = state;
                                } else {
                                    liveLocationDisplay.textContent = "Location found (details limited)";
                                }
                            } else {
                                liveLocationDisplay.textContent = "Location details unavailable.";
                            }
                        } catch (error) {
                            console.error("Error fetching location details:", error);
                            liveLocationDisplay.textContent = "Error fetching location details.";
                        }
                    },
                    (error) => {
                        console.error("Geolocation error:", error);
                        switch(error.code) {
                            case error.PERMISSION_DENIED:
                                liveLocationDisplay.textContent = "Location access denied.";
                                break;
                            case error.POSITION_UNAVAILABLE:
                                liveLocationDisplay.textContent = "Location unavailable.";
                                break;
                            case error.TIMEOUT:
                                liveLocationDisplay.textContent = "Location request timed out.";
                                break;
                            default:
                                liveLocationDisplay.textContent = "Location error.";
                                break;
                        }
                    }
                );
            } else {
                liveLocationDisplay.textContent = "Geolocation not supported.";
            }
        }


        // Initial render of products and cart UI
        renderProducts(); // Render all products initially
        updateCartUI(); // Initialize cart UI (will show empty cart message)
        showBannerSlide(0); // Show the first slide of the banner slideshow
        updateContentLanguage(); // Apply initial language to all static elements
        getLiveLocation(); // Fetch and display live location
    </script>
</body>
</html>
