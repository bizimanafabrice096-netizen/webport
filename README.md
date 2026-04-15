/* General Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Body with Aqua Gradient + Background Image */
body {
  font-family: Arial, sans-serif;
  background: linear-gradient(to bottom right, aqua, #e0ffff),
              url("bizi.jpeg") no-repeat top left fixed;
  background-size: cover;
  color: #333;
  line-height: 1.6;
}

/* Overlay effect for readability */
body::before {
  content: "";
  position: fixed;
  top: 0; left: 0;
  width: 100%; height: 100%;
  background: rgba(0, 255, 255, 0.4);
  z-index: -1;
}

/* Decorative circle shape */
body::after {
  content: "";
  position: fixed;
  bottom: -50px; right: -50px;
  width: 200px; height: 200px;
  background: rgba(0, 102, 102, 0.3);
  border-radius: 50%;
  z-index: -1;
}

/* Navigation */
.navbar {
  background: #006666;
  padding: 10px;
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 1000;
}
.navbar ul {
  display: flex;
  justify-content: center;
  list-style: none;
}
.navbar ul li {
  margin: 0 15px;
}
.navbar ul li a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}
.navbar ul li a:hover {
  text-decoration: underline;
}

/* Sections */
section {
  padding: 80px 50px;
  text-align: center;
  border-bottom: 2px solid #ccc;
  background: rgba(255, 255, 255, 0.85);
  margin: 20px;
  border-radius: 10px;
}

/* Home Section Layout */
.home-container {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 30px;
}

/* Profile Photo Styling */
.profile-photo {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  padding: 5px;
  border: 3px solid #006666;
  object-fit: cover;
}

/* Text beside photo */
.home-text {
  max-width: 500px;
  text-align: left;
}

/* Flexbox for Projects */
.flex-container {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin-top: 20px;
  flex-wrap: wrap;
}
.card {
  background: white;
  padding: 20px;
  border-radius: 8px;
  width: 200px;
  box-shadow: 2px 2px 8px rgba(0,0,0,0.2);
}
