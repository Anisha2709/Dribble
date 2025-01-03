# Project Responsive Web Design using Bootstrap
## Date: 24-12-2024

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
<html>

<head>
    <style>
        html {
            scroll-behavior: smooth;
        }

        nav ul {
            list-style: none;
            display: flex;
            background-color: rgb(0, 170, 255);
            padding: 20px;
            font-family: 'Courier New', Courier, monospace;
            margin-top: 1%;
            font-weight: 600;

        }

        nav ul li {
            margin-left: 13%;
            padding: 2px;

        }

        a {
            padding: 1px;
            text-decoration: none;
            color: black;
            font-size: 20px;
        }

        a:hover {
            color: aliceblue;
        }

        .mtitl {
            text-align: center;
            font-family: 'Courier New', Courier, monospace;
            font-size: 60px;
            margin-top: 2%;
            font-weight: bold;
            text-shadow: 2px 3px rgb(0, 170, 255);
        }

        .ab {
            color: rgb(38, 62, 62);
            line-height: 1.6;
            text-align: center;
            font-family: 'Courier New', Courier, monospace;
            margin-top: 2%;
            font-weight: 500;
            margin: 0 15%;
        }

        p {
            text-align: center;
            margin-bottom: 20px;
            font-size: 18px;
            line-height: 1.8;
            font-weight: bold;
        }

        .titl {
            text-shadow: 2px 1px whitesmoke;
            font-size: 40px;
            color: rgb(38, 62, 62);
            margin-top: 2%;
            margin-bottom: 2%;
            margin-left: 2%;
            text-align: left;
            font-family: 'Courier New', Courier, monospace;
            text-decoration: underline;
            font-weight: bold;
        }

        .titl:hover {
            color: whitesmoke;
            text-shadow: 2px 1px black;
            text-decoration: none;
        }

        body {
            background: linear-gradient(to right, rgb(14, 217, 240), rgb(107, 245, 218));
            margin-left: 2%;
        }

        .allbooks {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 60px;
        }

        .book {
            margin-top: 2%;
            font-family: 'Courier New', Courier, monospace;
            font-size: medium;
            font-weight: bold;

        }

        .book img {
            margin-top: 15%;
            width: 200px;
            height: 308px;
            margin-left: 2px;
            transition: transform 0.3s ease-in-out;

        }

        .book img:hover {
            transform: scale(1.1);
        }

        .book .auth {
            font-family: 'Courier New', Courier, monospace;
            font-size: 30px;
            max-width: 220px;
            margin-top: 5%;
            text-align: center;
        }

        .rev {
            margin-left: 2%;
        }

        .rev .comment ul {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(400px, 1fr));
            gap: 20px;
        }

        .rev .comment ul li {
            list-style: none;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            background-color: rgb(187, 255, 255);
            border-radius: 35px;
            padding: 40px;
            height: 50px;
            width: 300px;
            transition: transform 0.3s ease-in-out;
        }

        .rev .comment ul li:hover {
            transform: scale(1.1);
            box-shadow: 2px 3px 8px black;
        }

        footer {
            background-color: rgb(2, 38, 56);
            color: white;
            margin-top: 5%;
            padding: 20px;
            font-family: 'Courier New', Courier, monospace;
        }

        pre {
            font-family: 'Courier New', Courier, monospace;
        }

        .part {
            display: flex;
            justify-content: space-between;
        }

        footer .part ul {
            list-style: none;
            padding: 0;
            margin: 0;
            width: 30%;
        }

        footer .part ul li {
            margin-bottom: 10px;
            font-size: 18px;

        }

        .vertical-line {
            border-right: 2px solid rgb(190, 186, 186);
            padding-right: 10px;
        }
    </style>
</head>

<body>
    <center>
        <nav class="navbar">
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#ba">Books Available</a></li>
                <li><a href="#reviews">Reviews</a></li>
                <li><a href="#footer">Contact Us</a></li>
            </ul>
        </nav>
    </center>
    <div class="mtitl">Nine Lives Library 𓃠</div>
    <section id="about">
        <div class="titl">About 𓃠</div>
        <div class="ab">
            <p>Nestled in the heart of Chennai, <i>Purr & Page</i> is more than just a bookshop—it's a haven
                for book lovers and feline enthusiasts alike. <br> Our cozy shelves are filled with carefully curated
                books, from timeless classics to contemporary gems,
                all waiting to be discovered.But what makes Purr & Page truly special? Our resident shop cats, who are
                always ready to curl up beside
                you as you lose yourself in a story. <br> Whether you're here to browse, sip a cup of tea in our reading
                nook, or simply enjoy the calming
                presence of our whiskered friends,we promise an experience that's as warm and inviting as a sunbeam on a
                lazy afternoon. <br>
                Come for the books, stay for the purrs, and leave with a story (or two) to treasure.Your next adventure
                starts here.</p>
        </div>
    </section>
    <section id="ba">
        <div class="titl">Books Available 𓃠</div>
        <div class="allbooks">
            <div class="book">
                <img src="god of fury.jpg" alt="book img">
                <div class="auth">Rina Kent</div>
            </div>
            <div class="book">
                <img src="sweetest oblivion.jpg" alt="book img">
                <div class="auth">Danielle Lori</div>
            </div>
            <div class="book">
                <img src="Maddest Obsession.jpg" alt="book img">
                <div class="auth">Danielle Lori</div>
            </div>
            <div class="book">
                <img src="ugly love.jpg" alt="book img">
                <div class="auth">Colleen Hoover</div>
            </div>

            <div class="book">
                <img src="things we left behind.jpg" alt="book img">
                <div class="auth">Lucy Score</div>
            </div>
            <div class="book">
                <img src="consider me.jpg" alt="book img">
                <div class="auth">Becka Mack</div>
            </div>
            <div class="book">
                <img src="fall with me.jpg" alt="book img">
                <div class="auth">Becka Mack</div>
            </div>
            <div class="book">
                <img src="sinners condemned.jpg" alt="book img">
                <div class="auth">Somme Sketcher</div>
            </div>
            <div class="book">
                <img src="wretched.jpg" alt="book img">
                <div class="auth">Emily Mcintire</div>
            </div>
            <div class="book">
                <img src="fourth wing.jpg" alt="book img">
                <div class="auth">Rebecca Yarros</div>
            </div>

            <div class="book">
                <img src="hidden truths.jpg" alt="book img">
                <div class="auth">Neva Altaj</div>
            </div>
            <div class="book">
                <img src="stolen touches.jpg" alt="book img">
                <div class="auth">Neva Altaj</div>
            </div>
            <div class="book">
                <img src="darkest sins.jpg" alt="book img">
                <div class="auth">Neva Altaj</div>
            </div>
            <div class="book">
                <img src="yours truly.jpg" alt="book img">
                <div class="auth">Abby Jimenez</div>
            </div>
            <div class="book">
                <img src="king of sloth.jpg" alt="book img">
                <div class="auth">Ana Huang</div>
            </div>
            <div class="book">
                <img src="black ties and white lies.jpg" alt="book img">
                <div class="auth">Kat Singleton</div>
            </div>
            <div class="book">
                <img src="bright lights and Summer nights.jpg" alt="book img">
                <div class="auth">Kat Singleton</div>
            </div>
            <div class="book">
                <img src="bride.jpg" alt="book img">
                <div class="auth">Ali Hazelwood</div>
            </div>
            <div class="book">
                <img src="caught up.jpg" alt="book img">
                <div class="auth">Liz Tomforde</div>
            </div>
            <div class="book">
                <img src="lost heartbeats.jpg" alt="book img">
                <div class="auth">Ella Maise</div>
            </div>
            <div class="book">
                <img src="Marriage for One.jpg" alt="book img">
                <div class="auth">Ella Maise</div>
            </div>
            <div class="book">
                <img src="binding 13.jpg" alt="book img">
                <div class="auth">Chloe Walsh</div>
            </div>
            <div class="book">
                <img src="Redeeming 6.jpg" alt="book img">
                <div class="auth">Chloe Walsh</div>
            </div>

            <div class="book">
                <img src="cruel prince.jpg" alt="book img">
                <div class="auth">Holly Black</div>
            </div>
            <div class="book">
                <img src="wrecked.jpg" alt="book img">
                <div class="auth">Lauren Asher</div>
            </div>
        </div>
    </section>
    <section id="reviews">
        <div class="titl">Reviews 𓃠</div>
        <div class="rev">
            <div class="comment">
                <ul>
                    <li>"An absolute gem of a bookstore – cozy, charming, and filled with character!"</li>
                    <li>"Books have a home here, and so do readers."</li>
                    <li>"Warm lighting, comfy seating, and shelves brimming with treasures"</li>
                    <li>"Came for the books, stayed for the cats."</li>
                    <li>"Customer service here feels like chatting with old friends."</li>
                    <li>"Friendly faces and great bookish conversations – what more could you ask for?"</li>
                </ul>
            </div>
        </div>
    </section>
    <div id="footer"></div>
    <footer>
        <div class="part">
            <ul>
                <li>Contact Us 𓃠</li>
                <br>
                <li>Call us at: 91+ 1234567890</li>
                <li>Email: ninelives@gmail.com</li>
                <li>Visit us at: 123 Street, Avadi, Chennai.</li>
            </ul>
            <div class="vertical-line"></div>
            <ul>
                <li>Open 𓃠</li>
                <br>
                <li>Monday to Saturday: 9 AM - 6 PM</li>
                <li>Sunday: 9 AM - 8 PM</li>
            </ul>
            <div class="vertical-line"></div>
            <ul>
                <li>Follow us on 𓃠</li>
                <br>
                <li>
                    <pre>Facebook  - @NineLivesLibrary </pre>
                </li>
                <li>
                    <pre>Instagram - @NineLivesLibrary </pre>
                </li>
                <li>
                    <pre>Twitter   - @NineLivesLibrary </pre>
                </li>
                <li>
                    <pre>Pinterest - @NineLivesLibrary</pre>
                </li>

            </ul>
        </div>
    </footer>
</body>

</html>
```
## OUTPUT:

![alt text](1.png)

![alt text](2.png)

![alt text](3.png)

![alt text](4.png)

![alt text](5.png)

![alt text](6.png)

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
