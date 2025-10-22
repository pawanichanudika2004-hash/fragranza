<!DOCTYPE html>
<html>
<html lang="en">
<head>
	<meta charset="utf-8"/>
	<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
	<title>FRAGRANSA-A pure scent</title>
	<style>
		body{
			margin: o;
			font-family: 'Segoe UI', sans-serif;
			background-color: gray;
			color: #333;
		}

		header{
			display: flex;
			justify-content: space-between;
			align-items: center;
			padding: 15px 30px;
			background-color: #fff;
			border-bottom: 1px solid #ddd;
			position: sticky;
			top: 0;
			z-index: 1000;
		}

		header img{
			height: 50px;
		}

		nav a{
			margin: 0 15px;
			text-decoration: none;
			color: #555;
			font-weight: 500;
		}

		nav a:hover{
			color: #c89b6d;
		}

		.hero{
			background: url()no-repeat center center/cover;
			height: 90vh;
			display: flex;
			align-items: center;
			justify-content: center;
			color: white;
			text-align: center;
		}

		.hero h1{
			font-size: 3rem;
			background-color: rgba(0, 0, 0, 0.5);
			padding: 20px;
			border-radius: 10px;
		}

		.section{
			padding: 50px 20px;
			text-align: center;
		}

		.products{
			display: grid;
			grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
			gap: 30px;
			padding: 20px;
		}

		.product{
			background-color: #fff;
			border-radius: 10px;
			box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
			padding: 20px;
			transition: transform 0.3s;
		}

		.product:hover{
			transform: scale(1.05);
		}

		.product img{
			width: 100%;
			border-radius: 10px;
		}

		footer{
			background-color: #333;
			color: #fff;
			text-align: center;
			padding: 20px;
		}

		@media(orientation: portrait){
			.hero h1{
				font-size: 2rem;
			}
		}

	</style>
</head>
<body>

<header>
	<img src="A Perfume banner.jpeg" alt="Business logo" class="logo">
	<nav>
		<a href="#">Home</a>
		<a href="#products">Products</a>
		<a href="contact">Contact</a>
		<a href="#"id="cart">
		Cart(<span id="cart-count">0</span>)
	</a>
	</nav>
</header>

<div class="hero">
	<h1>Discover Your Signature Scent</h1>
</div>

<section class="section" id="products">
	<h2>Our Perfume Collection</h2>
	<div class="products">
		<div class="product">
			<img src="plumeria.jpeg" alt="Perfume 1"/>
			<h3>Plumeria</h3>
			<p>Offering you the fragrance of a thousand plumeria flowers.</p>
			<p>LKR 3,600</p>
			<button onclick="addToCart('Plumeria')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="sandalwood.jpeg" alt="Perfume 2">
			<h3>Sandalwood</h3>
			<p>Only for handsome people with extreamely good personalities.</p>
			<p>LKR 5,000</p>
			<button onclick="addToCart('Sandalwood')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="jasmine.jpeg" alt="Perfume 3">
			<h3>Jasmine</h3>
			<p>..</p>
			<p>LKR 750</p>
			<button onclick="addToCart('Jasmine')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="watermelon.jpeg" alt="Perfume 4">
			<h3>Watermelon</h3>
			<p>Get refershed with a fersh fruity scent and spend your day feeling refreshed.</p>
			<p>LKR 1,500</p>
			<button onclick="addToCart('Watermelon')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="vanilla.jpeg" alt="Perfume 5">
			<h3>Vanilla</h3>
			<p>Only for people who are extreamely heart warming.</p>
			<p>LKR 12,000</p>
			<button onclick="addToCart('Vanilla')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="bergamot.jpeg" alt="Perfume 6">
			<h3>Bergamot</h3>
			<p>A citrusy spark for those who lead with confidence.</p>
			<p>LKR 11,000</p>
			<button onclick="addToCart('Bergamot')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="rosemary.jpeg" alt="Perfume 7">
			<h3>Rosemary</h3>
			<p>Crisp and herbaceous, rosemary awakens the senses with earthy elegance and timeless freshness.</p>
			<p>LKR 12,000</p>
			<button onclick="addToCart('Rosemary')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="cherry.jpeg" alt="Perfume 8">
			<h3>Cherry</h3>
			<p>Sweet, bold and playful cherry bursts with juicy charm and a flirtatious finish that lingers.</p>
			<p>LKR 1,000</p>
			<button onclick="addToCart('Cherry')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="wallapatta.jpeg" alt="Perfume 9">
			<h3>Wallapatta</h3>
			<p>Deep, woody and mysterious wallapatta embodies strength and luxury with every earthy note.</p>
			<p>LKR 3,500</p>
			<button onclick="addToCart('Wallapatta')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="saffron.jpeg" alt="Perfume 10">
			<h3>Saffron</h3>
			<p>Rich, warm and exotic saffron weaves a golden trail of spice andelegance in every drop.</p>
			<p>LKR 2,500</p>
			<button onclick="addToCart('Saffron')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="cashmere.jpeg" alt="Perfume 11">
			<h3>Cashmere</h3>
			<p>Introducing the newest guest who stole the essence of a forest.</p>
			<p>LKR 2,000</p>
			<button onclick="addToCart('Cashmere')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="mint.jpeg" alt="Perfume 12">
			<h3>Mint</h3>
			<p>The symbol of freshness is the pomegranate.</p>
			<p>LKR 4,000</p>
			<button onclick="addToCart('Mint')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="lavender.jpeg" alt="Perfume 13">
			<h3>Lavender</h3>
			<p>Brings you a gentle, pleasant purple hue.</p>
			<p>LKR 1,000</p>
			<button onclick="addToCart('Lavender')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="cinnamon.jpeg" alt="Perfume 14">
			<h3>Cinnamon</h3>
			<p>Keep your day attractive and captivating be the first member to join the spicy fragrance.</p>
			<p>LKR 5,000</p>
			<button onclick="addToCart('Cinnamon')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="agarwood.jpeg" alt="Perfume 15">
			<h3>Agarwood</h3>
			<p>Show your personality to the world.</p>
			<p>LKR 12,000</p>
			<button onclick="addToCart('Agarwood')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="peony.jpeg" alt="Perfume 16">
			<h3>Peony</h3>
			<p>The freshness and softness to a flower petal bathed in moonlight.</p>
			<p>LKR 10,000</p>
			<button onclick="addToCart('Peony')">Add to Cart</button>
		</div>

		<div class="product">
			<img src="rose.jpeg" alt="Perfume 17">
			<h3>Rose</h3>
			<p>The pure fragrance of roses awakens hearts.</p>
			<p>LKR 2,200</p>
			<button onclick="addToCart('Rose')">Add to Cart</button>
		</div>

	</div>

</section>

<section class="section" id="contact">
	<h2>Contact Us</h2>
	<p>Email:info@fragranzaperfume.com</p>
	<p>Phone:+94 77 123 4567</p>
</section>

<footer>
	&copy;2024 Fragranza.All right reserved.
</footer>

<script>
	let cartCount=0;
	function addToCart(productName){
		cartCount++;
		document.getElementById("cart-count").textContent=cartCount;
		alert(productName+"added to cart!");
	}
</script>

</body>
</html>
