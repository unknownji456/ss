
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Materials</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
        }

        .row {
            display: flex;
            width: 80%;
            margin-bottom: 15px;
        }

        section {
            flex: 2; /* Section takes 2/3 of space */
            padding: 20px;
            border: 2px solid black;
            border-radius: 5px;
            cursor: pointer;
            background-color: lightblue;
        }

        .empty-space {
            flex: 1; /* Space for images */
            display: flex;
            align-items: center;
            justify-content: center;
            border: 2px dashed gray;
            margin-left: 10px;
            padding: 10px;
        }

        .empty-space img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
        }

        .details {
            display: none;
            margin-top: 10px;
            padding: 10px;
            background: white;
            border: 1px solid black;
            border-radius: 5px;
        }
    </style>
</head>
<body>

    <h2>TANDOORI HUT MENU</h2>

    <div class="row">
        <section onclick="toggleDetails('section1')">
            <h2>INDIAN CUISINE(VEG.)</h2>
            <div id="section1" class="details">
                <p>Plastic is a synthetic material made from polymers.</p>
            </div>
        </section>
        <div class="empty-space">
            <img src="https://upload.wikimedia.org/wikipedia/commons/4/4c/Plastic_bottles.jpg" alt="Plastic">
        </div>
    </div>

    <div class="row">
        <section onclick="toggleDetails('section2')">
            <h2>COMBO+BEVERAGE HOT+SHAKES</h2>
            <div id="section2" class="details">
                <p>Iron is a strong, durable metal commonly used in construction.</p>
            </div>
        </section>
        <div class="empty-space">
            <img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/Iron_ore_pellets.jpg" alt="Iron">
        </div>
    </div>

    <div class="row">
        <section onclick="toggleDetails('section3')">
            <h2>FAST FOOD</h2>
            <div id="section3" class="details">
                <p>Metals are solid materials that conduct electricity and heat.</p>
            </div>
        </section>
        <div class="empty-space">
            <img src="https://upload.wikimedia.org/wikipedia/commons/9/91/Aluminium.jpg" alt="Metal">
        </div>
    </div>

    <div class="row">
        <section onclick="toggleDetails('section4')">
            <h2>Wood</h2>
            <div id="section4" class="details">
                <p>Wood is a natural material used in furniture and construction.</p>
            </div>
        </section>
        <div class="empty-space">
            <img src="https://upload.wikimedia.org/wikipedia/commons/3/3e/Wooden_planks.jpg" alt="Wood">
        </div>
    </div>

    <div class="row">
        <section onclick="toggleDetails('section5')">
            <h2>Glass</h2>
            <div id="section5" class="details">
                <p>Glass is a transparent material used in windows and bottles.</p>
            </div>
        </section>
        <div class="empty-space">
            <img src="https://upload.wikimedia.org/wikipedia/commons/2/2f/Glass_Bottles.jpg" alt="Glass">
        </div>
    </div>

    <div class="row">
        <section onclick="toggleDetails('section6')">
            <h2>Concrete</h2>
            <div id="section6" class="details">
                <p>Concrete is a composite material used for construction.</p>
            </div>
        </section>
        <div class="empty-space">
            <img src="https://upload.wikimedia.org/wikipedia/commons/a/aa/Concrete_blocks.jpg" alt="Concrete">
        </div>
    </div>

    <div class="row">
        <section onclick="toggleDetails('section7')">
            <h2>Ceramic</h2>
            <div id="section7" class="details">
                <p>Ceramic materials are used in pottery and tiles.</p>
            </div>
        </section>
        <div class="empty-space">
            <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Ceramic_pottery.jpg" alt="Ceramic">
        </div>
    </div>

    <div class="row">
        <section onclick="toggleDetails('section8')">
            <h2>Rubber</h2>
            <div id="section8" class="details">
                <p>Rubber is a flexible material used in tires and seals.</p>
            </div>
        </section>
        <div class="empty-space">
            <img src="https://upload.wikimedia.org/wikipedia/commons/d/d2/Rubber_tree.jpg" alt="Rubber">
        </div>
    </div>

    <div class="row">
        <section onclick="toggleDetails('section9')">
            <h2>Paper</h2>
            <div id="section9" class="details">
                <p>Paper is made from wood pulp and is used for writing and printing.</p>
            </div>
        </section>
        <div class="empty-space">
            <img src="https://upload.wikimedia.org/wikipedia/commons/9/9a/Paper_stack.jpg" alt="Paper">
        </div>
    </div>

    <div class="row">
        <section onclick="toggleDetails('section10')">
            <h2>Fabric</h2>
            <div id="section10" class="details">
                <p>Fabric is used in clothing and upholstery.</p>
            </div>
        </section>
        <div class="empty-space">
            <img src="https://upload.wikimedia.org/wikipedia/commons/5/51/Fabric_textiles.jpg" alt="Fabric">
        </div>
    </div>

    <script>
        function toggleDetails(id) {
            var details = document.getElementById(id);
            if (details.style.display === "none" || details.style.display === "") {
                details.style.display = "block";
            } else {
                details.style.display = "none";
            }
        }
    </script>

</body>
</html>
