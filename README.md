<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Image Banner</title>

<style>
body {
    margin: 0;
    font-family: Arial, sans-serif;
}

/* Banner Section */
.banner {
    position: relative;
    width: 100%;
    height: 500px;
    background: url("YOUR_IMAGE_LINK_HERE") no-repeat center center/cover;
    display: flex;
    align-items: center;
    justify-content: center;
}

/* Dark Overlay */
.banner::after {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.5);
}

/* Banner Content */
.banner-content {
    position: relative;
    color: #fff;
    text-align: center;
    z-index: 1;
}

.banner-content h1 {
    font-size: 48px;
    margin: 0;
}

.banner-content p {
    font-size: 20px;
    margin: 15px 0;
}

.banner-content button {
    padding: 12px 25px;
    font-size: 16px;
    border: none;
    background: #ff4c4c;
    color: white;
    cursor: pointer;
    border-radius: 5px;
    transition: 0.3s;
}

.banner-content button:hover {
    background: #e63939;
}

/* Responsive */
@media (max-width: 768px) {
    .banner {
        height: 350px;
    }
    .banner-content h1 {
        font-size: 32px;
    }
    .banner-content p {
        font-size: 16px;
    }
}
</style>
</head>

<body>

<section class="banner">
    <div class="banner-content">
        <h1>Your Main Heading</h1>
        <p>Your subtitle or description goes here</p>
        <button>Learn More</button>
    </div>
</section>

</body>
</html>
