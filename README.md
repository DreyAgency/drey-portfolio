/* Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 1.6;
  background: #f4f4f4;
  color: #333;
  padding-bottom: 100px;
}

/* Navigation */
nav {
  background: #111;
  color: white;
  padding: 10px 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: sticky;
  top: 0;
  z-index: 10;
}

nav .logo {
  font-size: 1.5rem;
  font-weight: bold;
}

nav ul {
  display: flex;
  gap: 20px;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: 500;
}

nav a:hover {
  text-decoration: underline;
}

/* Header */
header {
  background: #1a73e8;
  color: white;
  padding: 40px 20px;
  text-align: center;
}

/* Sections */
section {
  padding: 40px 20px;
  max-width: 900px;
  margin: auto;
}

/* Testimonials */
.testimonials video {
  width: 100%;
  border-radius: 10px;
}

.video-container {
  margin-bottom: 30px;
}

/* Services */
#services .service-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
  margin-top: 20px;
  animation: fadeIn 2s ease-in-out;
}

.service-item {
  background: #fff;
  padding: 20px;
  border-left: 5px solid #1a73e8;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  border-radius: 10px;
  transition: transform 0.3s ease;
}

.service-item:hover {
  transform: translateY(-5px);
}

/* Scroll Button */
#scrollTopBtn {
  position: fixed;
  bottom: 30px;
  right: 30px;
  background: #1a73e8;
  color: white;
  border: none;
  padding: 10px 14px;
  border-radius: 50%;
  font-size: 20px;
  cursor: pointer;
  display: none;
  box-shadow: 0 0 10px rgba(0,0,0,0.2);
}

#scrollTopBtn:hover {
  background: #004aad;
}

/* Footer */
footer {
  text-align: center;
  padding: 20px;
  background: #111;
  color: white;
  position: relative;
}

/* Animations */
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Responsive */
@media (max-width: 768px) {
  nav ul {
    flex-direction: column;
    gap: 10px;
  }

  header h1 {
    font-size: 1.8rem;
  }
}
