<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Find My Pets</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            background: #f4f4f4;
            text-align: center;
            padding: 20px;
        }

        .card {
            background: white;
            max-width: 420px;
            margin: auto;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 3px 15px rgba(0,0,0,0.1);
        }

        input, select {
            width: 90%;
            padding: 12px;
            margin: 7px 0;
            border: 1px solid #ccc;
            border-radius: 8px;
            box-sizing: border-box;
            background: white;
        }

        button {
            padding: 12px 20px;
            margin: 8px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            background: #222;
            color: white;
        }

        #profile {
            display: none;
            margin-top: 20px;
            padding: 20px;
            background: #eee;
            border-radius: 10px;
        }

        #qrcode {
            margin: 20px auto;
            width: 180px;
        }

        .found {
            display: none;
        }
    </style>
</head>

<body>

<div class="card">

    <h1>🐾 Find My Pets</h1>
    <p>Keep your pet safe and easy to identify.</p>

    <div id="register">

        <h2>Register Your Pet</h2>

        <select id="petType">
            <option value="">Select Pet Type</option>
            <option value="Cat">🐱 Cat</option>
            <option value="Dog">🐶 Dog</option>
            <option value="Rabbit">🐰 Rabbit</option>
            <option value="Bird">🐦 Bird</option>
            <option value="Other">🐾 Other Pet</option>
        </select>

        <input type="text" id="petName" placeholder="Pet Name">

        <input type="text" id="ownerName" placeholder="Owner Name">

        <input type="text" id="phone" placeholder="Phone Number">

        <input type="text" id="petColor" placeholder="Pet Color">

        <input type="text" id="petBreed" placeholder="Breed">

        <br>

        <button onclick="saveProfile()">💾 Register Pet</button>

        <div id="profile">

            <h2>🐾 Pet Information</h2>

            <p id="showType"></p>
            <p id="showPet"></p>
            <p id="showOwner"></p>
            <p id="showPhone"></p>
            <p id="showColor"></p>
            <p id="showBreed"></p>

            <button onclick="callOwner()">📞 Call Owner</button>

            <button onclick="whatsappOwner()">💬 WhatsApp Owner</button>

            <h3>📱 Scan This QR Code</h3>

            <div id="qrcode"></div>

        </div>

    </div>


    <div id="found" class="found">

        <h2>🐾 Pet Found!</h2>

        <p id="foundType"></p>
        <p id="foundPet"></p>
        <p id="foundColor"></p>
        <p id="foundBreed"></p>

        <p>
            Please contact the owner to return this pet safely.
        </p>

        <button id="foundCall">
            📞 Call Owner
        </button>

        <button id="foundWhatsApp">
            💬 WhatsApp Owner
        </button>

    </div>

</div>


<script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>


<script>

function saveProfile() {

    let type = document.getElementById("petType").value;
    let pet = document.getElementById("petName").value.trim();
    let owner = document.getElementById("ownerName").value.trim();
    let phone = document.getElementById("phone").value.trim();
    let color = document.getElementById("petColor").value.trim();
    let breed = document.getElementById("petBreed").value.trim();


    if (type === "" || pet === "" || owner === "" || phone === "") {

        alert("Please select Pet Type and enter Pet Name, Owner Name and Phone Number.");

        return;
    }


    document.getElementById("showType").innerHTML =
        "🐾 Pet Type: " + type;

    document.getElementById("showPet").innerHTML =
        "🐾 Pet Name: " + pet;

    document.getElementById("showOwner").innerHTML =
        "👤 Owner: " + owner;

    document.getElementById("showPhone").innerHTML =
        "📞 Phone: " + phone;

    document.getElementById("showColor").innerHTML =
        "🎨 Color: " + (color || "Not provided");

    document.getElementById("showBreed").innerHTML =
        "🐾 Breed: " + (breed || "Not provided");


    document.getElementById("profile").style.display = "block";


    let baseURL =
        window.location.origin + window.location.pathname;


    let qrData =
        baseURL +
        "?type=" + encodeURIComponent(type) +
        "&pet=" + encodeURIComponent(pet) +
        "&owner=" + encodeURIComponent(owner) +
        "&phone=" + encodeURIComponent(phone) +
        "&color=" + encodeURIComponent(color) +
        "&breed=" + encodeURIComponent(breed);


    document.getElementById("qrcode").innerHTML = "";


    new QRCode(document.getElementById("qrcode"), {

        text: qrData,

        width: 180,

        height: 180

    });

}


function callOwner() {

    let phone =
        document.getElementById("phone").value;

    window.location.href =
        "tel:" + phone;

}


function whatsappOwner() {

    let phone =
        document.getElementById("phone").value;

    phone =
        phone.replace(/\D/g, "");


    if (phone.startsWith("0")) {

        phone =
            "92" + phone.substring(1);

    }


    window.open(
        "https://wa.me/" + phone,
        "_blank"
    );

}


function showFoundPet() {

    let params =
        new URLSearchParams(window.location.search);


    let pet =
        params.get("pet");


    if (!pet) {

        return;

    }


    let type =
        params.get("type");

    let owner =
        params.get("owner");

    let phone =
        params.get("phone");

    let color =
        params.get("color");

    let breed =
        params.get("breed");


    document.getElementById("register").style.display =
        "none";


    document.getElementById("found").style.display =
        "block";


    document.getElementById("foundType").innerHTML =
        "🐾 Pet Type: " + (type || "Pet");


    document.getElementById("foundPet").innerHTML =
        "🐾 Pet Name: " + pet;


    document.getElementById("foundColor").innerHTML =
        "🎨 Color: " + (color || "Not provided");


    document.getElementById("foundBreed").innerHTML =
        "🐾 Breed: " + (breed || "Not provided");


    document.getElementById("foundCall").onclick =
        function() {

            window.location.href =
                "tel:" + phone;

        };


    document.getElementById("foundWhatsApp").onclick =
        function() {

            let whatsappNumber =
                phone.replace(/\D/g, "");


            if (whatsappNumber.startsWith("0")) {

                whatsappNumber =
                    "92" + whatsappNumber.substring(1);

            }


            window.open(
                "https://wa.me/" + whatsappNumber,
                "_blank"
            );

        };

}


showFoundPet();

</script>

</body>
</html>
