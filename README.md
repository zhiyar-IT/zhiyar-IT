<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>mn u to cafe</title>
    <style>
        /* Global Styles */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
            line-height: 1.6;
            scroll-behavior: smooth;
        }

        h1, h2, h3 {
            margin: 0;
            font-weight: normal;
        }

        p {
            margin: 10px 0;
        }

        /* Header */
        header {
            background-color: #8d6e63;
            color: #fff;
            padding: 40px 0;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            animation: fadeInDown 1s ease-in-out;
        }

        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
            font-family: 'Montserrat', sans-serif;
        }

        header p {
            font-size: 1.5em;
        }

        /* Navigation */
        nav {
            background-color: #333;
            overflow: hidden;
            text-align: center;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            animation: fadeInDown 1s ease-in-out;
        }

        nav a {
            display: inline-block;
            color: #fff;
            padding: 16px 25px;
            text-decoration: none;
            font-size: 1.1em;
            transition: background-color 0.3s ease, color 0.3s ease, transform 0.3s ease;
        }

        nav a:hover {
            background-color: #555;
            color: #fff;
            transform: scale(1.05);
        }

        /* Main Content */
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 50px auto;
            padding: 30px;
            background-color: #fff;
            border-radius: 12px;
            box-shadow: 0 6px 18px rgba(0, 0, 0, 0.1);
            animation: fadeInUp 1s ease-in-out;
        }

        h2 {
            font-size: 2.5em;
            text-align: center;
            margin-bottom: 40px;
            color: #333;
        }

        /* Menu Section */
        .menu-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            margin-bottom: 20px;
            background-color: #f9f9f9;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            animation: fadeInUp 1s ease-in-out;
        }

        .menu-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        .menu-item h3 {
            font-size: 1.8em;
            color: #444;
            transition: color 0.3s ease;
        }

        .menu-item p {
            color: #777;
            font-size: 1.1em;
        }

        .menu-item:hover h3 {
            color: #8d6e63;
        }

        .menu-item ul {
            list-style: none;
            padding-left: 0;
        }

        .menu-item ul li {
            margin-bottom: 8px;
            font-size: 1.1em;
        }

        .menu-item span {
            font-size: 1.5em;
            font-weight: bold;
            color: #8d6e63;
            transition: color 0.3s ease;
        }

        .menu-item:hover span {
            color: #4a2c1c; /* Darker brown when hovered */
        }

        /* Footer */
        footer {
            background-color: #333;
            color: #fff;
            padding: 30px 0;
            text-align: center;
            font-size: 1.1em;
            transition: background-color 0.3s ease;
            animation: fadeInUp 1s ease-in-out;
        }

        footer p {
            margin: 0;
        }

        footer:hover {
            background-color: #444;
        }

        /* Button Hover Effect (for possible future use) */
        .button {
            padding: 10px 20px;
            background-color: #8d6e63;
            color: white;
            font-size: 1.2em;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: transform 0.3s ease, background-color 0.3s ease;
        }

        .button:hover {
            background-color: #6b4d3d;
            transform: scale(1.1);
        }

        /* Home Section */
        #home {
            background-image: url('https://example.com/coffee-background.jpg'); /* Replace with your own image */
            background-size: cover;
            background-position: center;
            padding: 100px 0;
            color: #fff;
            text-align: center;
            animation: fadeIn 1s ease-in-out;
        }

        #home h2 {
            font-size: 3em;
            margin-bottom: 20px;
            font-family: 'Montserrat', sans-serif;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        #home p {
            font-size: 1.4em;
            margin-bottom: 30px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        .home-button {
            padding: 15px 30px;
            font-size: 1.2em;
            background-color: #8d6e63;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }

        .home-button:hover {
            background-color: #6b4d3d;
            transform: scale(1.1);
        }

        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes fadeInDown {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            nav a {
                font-size: 1em;
                padding: 14px 20px;
            }

            .menu-item {
                flex-direction: column;
                align-items: flex-start;
            }

            .menu-item span {
                font-size: 1.3em;
                margin-top: 10px;
            }

            .container {
                width: 95%;
                padding: 20px;
            }

            header h1 {
                font-size: 2.2em;
            }

            h2 {
                font-size: 2em;
            }
        }

        @media (max-width: 480px) {
            header h1 {
                font-size: 2em;
            }

            .menu-item h3 {
                font-size: 1.4em;
            }

            .menu-item span {
                font-size: 1.2em;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>بەخێربێی بۆ کافتریای من و تۆ</h1>
        <p>شوێنێک تایبەت بۆ یاری و خواردن و خواردنەوەکان</p>
    </header>

    <nav>
        <a href="#home">Home</a>
        <a href="#menu">Menu</a>
        <a href="#about">دەربارەی ئێمە</a>
        
    </nav>

    <!-- Home Section -->
    <div id="home">
        <h2>Discover Your Favorite Coffee</h2>
        <p> At mn u to Cafe, we offer the finest selection of coffee blends and a cozy atmosphere perfect for relaxing and socializing. Enjoy every sip!</p>
        <a href="#menu">
            <button class="home-button">Explore Our Menu</button>
        </a>
    </div>

    <div class="container" id="menu">
        <h2>مینۆ تایبەتەکەمان بۆ ئێوە</h2>

        <!-- Coffee section -->
        <div class="menu-item">
            <div>

                <h3>شەربەتەکان</h3>
                <img src="https://www.itl.cat/pngfile/big/159-1592544_fresh-juice-images-hd.jpg"  height="70"  alt="Juices">
                <p>availeble juices</p
                <ul>
                    <li>لیمۆ</li>
                    <li>پڕتەقال</li>
                    <li>هەنار</li>
                    <li>شیرمۆز</li>
                 
                </ul>
            </div>
            <span>١٠٠٠ دینار</span>
        </div>

        <div class="menu-item">
            <div>
                <h3> خواردنەکان</h3>
                
                <ul>
                    <li>فینگەر</li>
                    <li>بۆرگەر</li>
                 
                </ul>
            </div>
            <span>١٥٠٠ دینار</span>
        </div>
        <!-- Available Shishas section -->
        <div class="menu-item">
            <div>
                <h3>نێرگەلەکان</h3>
                <p>تامی تایبەتی خۆت هەلبژێرە              </p>
                <ul>
                    <li>بنیشت و فراولە</li>
                    <li>دوو سێو</li>
                    <li>بنیشت گندۆرە</li>
                    <li>ئينگلیزی</li>
                    <li>من و تۆ ٧</li>
                    <li>کینگ</li>
                    <li>لیمۆ</li>
                    <li>بەغدادی</li>
                    <li>بنیشت سادە</li>
                     <li>کاسترۆ</li>
                     <li>ڤی ئاي پی</li>
                     <li>تيکتۆک</li>


                </ul>
            </div>
            <span>٥٠٠٠ دینار</span>
        </div>

        <!-- Drinks section -->
        <div class="menu-item">
            <div>
                <h3>خواردنەوەکان</h3>
                <p>خواردنەوە گازیەکان و تێکەلەی مەکسیکی
                </p>
                <ul>                
                    <li>ئاو </li>
                    <li>سمارت <b>(1500 IQD) </b></li>
                    <li>تایگەر <b>(1500 IQD) </b></li>
                    <li>پلينگ <b>(1500 IQD) </b></li>
                    <li>وایت</li>
                    <li>جاگوار</li>

                    <li>مەکسیکی تایگەر <b>(2000 IQD)</b>></li>
                    <li>تێکەلەی مەکسیکی لەگەل ،تایگەر ،سمارت،پلینگ،وایت،هتد….
                        . (2000 IQD)</li>
                </ul>
            </div>
            <span>+1000 IQD</span>
        </div>
        <div class="menu-item">
            <div>
                <h3>خواردنەوە گەرمەکان</h3>
                
                <ul>
                    <li>چای <b>(Free)</b></li>                   
                    <li>چۆکولاتە <b>(500 IQD) </b></li>
                    <li>قاوەی مەحموود <b>(500 IQD) </b></li>
                    <li>کاپاچینۆ <b>(500 IQD) </b></li>
                    <li>شیر    <b>(500 IQD) </b>      </li>  
                    <li>نیسکافە   <b>(500 IQD) </b>  </li>
                    <li>قاوە سادە    <b>(500 IQD) </b>  </li>

                    
                </ul>
            </div>
            <span>+500 IQD</span>
        </div>

        <!-- Services section -->
        <div class="menu-item">
            <div>
                <h3>چیپس</h3>
                <ul>
                    <li>لیمۆ </li>                   
                    <li>تەماتە </li>
                    <li>تیژ</li>
                    <li>سرکە</li>
                    <li>پۆفاک</li>
                    

                    
                </ul>
            </div>
            
            <span>٢٥٠ دینار</span>
        </div>

        <!-- Board Games section -->
        <div class="menu-item">
            <div>
                <h3>یاریەکانمان</h3>
                
                <ul>
                    <li>دۆمینە</li>
                    <li>ئۆکێي</li>
                    <li>شەترەنج</li>
                    <li>تاولە</li>
                    <li>کۆنکان</li>
                </ul>
            </div>
            <span>گشتی خۆراییە</span>
        </div>

        <!-- Tea and Board Games -->
        <div class="menu-item">
            <div>
                <h3>چای لەگەل یاری</h3>
                <p>خۆرایی</p>
            </div>
            <span>Free Services</span>
        </div>
    </div>
  
    
    <footer>
        <p>&copy; 2025 mn u to cafe. All rights reserved.</p>
    </footer>

</body>
</html>
