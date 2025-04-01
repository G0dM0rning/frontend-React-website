<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>React App</title><script defer="defer" src="/static/js/main.dc9afd55.js"></script><link href="/static/css/main.ead65e1d.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
Home page code 
/* src/styles/HomePage.css */
body {
  font-family: 'Poppins', sans-serif;
  margin: 0;
  padding: 0;
  background: #f8f9fa;
}

/* Navigation Bar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #ff7eb3;
  padding: 15px 50px;
  color: white;
}

.site-title {
  font-size: 24px;
  font-weight: bold;
}

.nav-links {
  display: flex;
  gap: 15px;
}

.nav-button {
  text-decoration: none;
  color: white;
  background: rgba(255, 255, 255, 0.2);
  padding: 8px 16px;
  border-radius: 5px;
  transition: 0.3s;
}

.nav-button:hover {
  background: rgba(255, 255, 255, 0.4);
}

/* Search Bar */
.search-bar {
  display: flex;
  justify-content: center;
  margin: 20px auto;
  width: 80%;
  max-width: 600px;
  position: relative;
}

.search-bar input {
  width: 100%;
  padding: 12px;
  font-size: 16px;
  border: 2px solid #ff7eb3;
  border-radius: 8px;
}

.search-button {
  background: #ff7eb3;
  border: none;
  color: white;
  padding: 12px 20px;
  cursor: pointer;
  border-radius: 8px;
  position: absolute;
  right: 0;
}

.search-button:hover {
  background: #ff5c9a;
}

/* Products Grid */
.products-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  margin: 20px auto;
  width: 80%;
}

/* Product Card */
.product-card {
  background: white;
  padding: 15px;
  border-radius: 10px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  text-align: center;
  transition: transform 0.3s;
}

.product-card:hover {
  transform: translateY(-5px);
}

.product-image {
  width: 100%;
  max-height: 200px;
  object-fit: cover;
  border-radius: 10px;
}

.product-name {
  font-size: 18px;
  margin: 10px 0;
}

.product-brand,
.product-price,
.product-rating {
  font-size: 14px;
  color: #555;
}

.recommend-link {
  display: inline-block;
  margin-top: 10px;
  text-decoration: none;
  background: #ff7eb3;
  color: white;
  padding: 8px 12px;
  border-radius: 5px;
  transition: 0.3s;
}

.recommend-link:hover {
  background: #ff5c9a;
}

/* Responsive Design */
@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    text-align: center;
    padding: 15px;
  }

  .nav-links {
    margin-top: 10px;
  }

  .search-bar {
    width: 90%;
  }

  .products-grid {
    grid-template-columns: 1fr;
  }
}

@media (min-width: 1024px) {
  .products-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}
