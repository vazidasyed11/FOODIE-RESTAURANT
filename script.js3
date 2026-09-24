// =========================
// FOODIE RESTAURANT JAVASCRIPT
// =========================


// =========================
// RESERVATION FORM
// =========================

const form = document.querySelector(".form");

form.addEventListener("submit", function (event) {

    event.preventDefault();

    const name = document.getElementById("name").value;
    const email = document.getElementById("email").value;
    const date = document.getElementById("date").value;
    const people = document.getElementById("people").value;
    const message = document.getElementById("message").value;

    if (name === "" || email === "" || date === "") {
        alert("Please fill in all required fields.");
        return;
    }

    alert(
        "Table booked successfully! 🍽️\n\n" +
        "Name: " + name +
        "\nEmail: " + email +
        "\nDate: " + date +
        "\nGuests: " + people
    );

    // Clear form after booking
    form.reset();
});


// =========================
// NAVBAR ACTIVE LINK
// =========================

const navLinks = document.querySelectorAll("nav ul li a");

navLinks.forEach(function (link) {

    link.addEventListener("click", function () {

        navLinks.forEach(function (item) {
            item.classList.remove("active");
        });

        this.classList.add("active");
    });

});


// =========================
// SET MINIMUM RESERVATION DATE
// =========================

const dateInput = document.getElementById("date");

const today = new Date();

const year = today.getFullYear();

const month = String(today.getMonth() + 1).padStart(2, "0");

const day = String(today.getDate()).padStart(2, "0");

const currentDate = `${year}-${month}-${day}`;

dateInput.setAttribute("min", currentDate);


// =========================
// WELCOME MESSAGE
// =========================

window.addEventListener("load", function () {

    console.log("Welcome to Foodie Restaurant! 🍕");

});


// =========================
// SMOOTH SCROLLING
// =========================

navLinks.forEach(function (link) {

    link.addEventListener("click", function (event) {

        const targetId = this.getAttribute("href");

        const targetSection = document.querySelector(targetId);

        if (targetSection) {

            event.preventDefault();

            targetSection.scrollIntoView({
                behavior: "smooth"
            });

        }

    });

});


// =========================
// MENU CARD CLICK EFFECT
// =========================

const foodCards = document.querySelectorAll(".food-card");

foodCards.forEach(function (card) {

    card.addEventListener("click", function () {

        const foodName = this.querySelector("h3").textContent;

        const price = this.querySelector(".price").textContent;

        alert(
            "🍽️ " + foodName +
            "\nPrice: " + price +
            "\n\nThank you for choosing Foodie!"
        );

    });

});


// =========================
// CATEGORY CLICK
// =========================

const categories = document.querySelectorAll(".category");

categories.forEach(function (category) {

    category.addEventListener("click", function () {

        const categoryName = this.querySelector("h3").textContent;

        alert(
            "You selected " +
            categoryName +
            " 🍴"
        );

    });

});