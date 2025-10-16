# Project Responsive Web Design using Bootstrap
## Date: 16-10-2025

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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dribbble Clone</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <!-- Custom CSS -->
    <link rel="stylesheet" href="style.css">
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg bg-white border-bottom sticky-top">
        <div class="container">
            <a class="navbar-brand" href="#">
                <img src="https://cdn.dribbble.com/assets/logo-footer-hd-a05db77841b4b27c0bf23ec1378e97c988190dfe7d26e32e1faea7269f9e001b.png" alt="Dribbble" height="30">
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown">
                            Inspiration
                        </a>
                        <ul class="dropdown-menu">
                            <li><a class="dropdown-item" href="#">Explore Design Work</a></li>
                            <li><a class="dropdown-item" href="#">New & Noteworthy</a></li>
                            <li><a class="dropdown-item" href="#">Playoffs</a></li>
                        </ul>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Find Work</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Learn Design</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Go Pro</a>
                    </li>
                </ul>
                <form class="d-flex me-3" role="search">
                    <div class="input-group">
                        <span class="input-group-text bg-light border-end-0">
                            <i class="fas fa-search text-muted"></i>
                        </span>
                        <input class="form-control border-start-0" type="search" placeholder="Search" aria-label="Search">
                    </div>
                </form>
                <div class="d-flex gap-2">
                    <button class="btn btn-outline-dark">Sign in</button>
                    <button class="btn btn-pink">Sign up</button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="container py-4">
        <!-- Filters -->
        <div class="filters mb-4">
            <div class="d-flex justify-content-between align-items-center">
                <ul class="nav">
                    <li class="nav-item">
                        <a class="nav-link active" href="#">Popular</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">New & Noteworthy</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Goods for Sale</a>
                    </li>
                </ul>
                <div class="dropdown">
                    <button class="btn btn-light dropdown-toggle" type="button" data-bs-toggle="dropdown">
                        Following
                    </button>
                    <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="#">Following</a></li>
                        <li><a class="dropdown-item" href="#">Trending</a></li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Gallery Grid -->
        <div class="row g-4" id="masonry-grid">
            <!-- Shot Item 1 -->
            <div class="col-12 col-md-6 col-lg-4 shot-item">
                <div class="card">
                    <div class="shot-preview">
                        <img src="https://picsum.photos/400/300" class="card-img-top" alt="Design Shot">
                        <div class="shot-overlay">
                            <h5 class="shot-title">Amazing Design</h5>
                            <div class="shot-actions">
                                <button class="btn btn-light btn-sm"><i class="fas fa-heart"></i></button>
                                <button class="btn btn-light btn-sm"><i class="fas fa-bookmark"></i></button>
                            </div>
                        </div>
                    </div>
                    <div class="card-body">
                        <div class="d-flex align-items-center">
                            <img src="https://picsum.photos/32" class="rounded-circle me-2" alt="Avatar">
                            <div>
                                <h6 class="mb-0">Designer Name</h6>
                                <span class="badge bg-pro">Pro</span>
                            </div>
                            <div class="ms-auto">
                                <button class="btn btn-sm btn-light"><i class="fas fa-heart"></i> 150</button>
                                <button class="btn btn-sm btn-light"><i class="fas fa-eye"></i> 1.2k</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Shot Item 2 -->
            <div class="col-12 col-md-6 col-lg-4 shot-item">
                <div class="card">
                    <div class="shot-preview">
                        <img src="https://picsum.photos/401/300" class="card-img-top" alt="Design Shot">
                        <div class="shot-overlay">
                            <h5 class="shot-title">Creative Concept</h5>
                            <div class="shot-actions">
                                <button class="btn btn-light btn-sm"><i class="fas fa-heart"></i></button>
                                <button class="btn btn-light btn-sm"><i class="fas fa-bookmark"></i></button>
                            </div>
                        </div>
                    </div>
                    <div class="card-body">
                        <div class="d-flex align-items-center">
                            <img src="https://picsum.photos/33" class="rounded-circle me-2" alt="Avatar">
                            <div>
                                <h6 class="mb-0">Creative Studio</h6>
                                <span class="badge bg-team">Team</span>
                            </div>
                            <div class="ms-auto">
                                <button class="btn btn-sm btn-light"><i class="fas fa-heart"></i> 234</button>
                                <button class="btn btn-sm btn-light"><i class="fas fa-eye"></i> 2.5k</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <!-- Bootstrap JS and Popper.js -->
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.8/dist/umd/popper.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.min.js"></script>
</body>
</html>
```
CSS
```
/* Custom Variables */
:root {
    --dribbble-pink: #ea4c89;
    --hover-overlay: rgba(0, 0, 0, 0.5);
}

/* General Styles */
body {
    background-color: #f8f8f8;
    font-family: "Haas Grot Text R Web", "Helvetica Neue", Helvetica, Arial, sans-serif;
}

/* Navbar Customization */
.navbar {
    box-shadow: 0 0 8px rgba(0, 0, 0, 0.1);
}

.navbar-brand img {
    max-height: 24px;
}

.btn-pink {
    background-color: var(--dribbble-pink);
    color: white;
    border: none;
}

.btn-pink:hover {
    background-color: #e23177;
    color: white;
}

/* Search Bar */
.input-group .form-control {
    border-radius: 20px;
    padding-left: 40px;
}

.input-group .input-group-text {
    position: absolute;
    z-index: 4;
    border: none;
    background: transparent;
    padding-left: 15px;
}

/* Filters */
.filters .nav-link {
    color: #6e6d7a;
    font-weight: 500;
}

.filters .nav-link.active {
    color: #0d0c22;
    position: relative;
}

.filters .nav-link.active::after {
    content: '';
    position: absolute;
    bottom: -2px;
    left: 50%;
    transform: translateX(-50%);
    width: 20px;
    height: 2px;
    background-color: var(--dribbble-pink);
}

/* Shot Items */
.shot-item {
    margin-bottom: 24px;
}

.shot-preview {
    position: relative;
    overflow: hidden;
    border-radius: 8px;
}

.shot-preview img {
    width: 100%;
    height: auto;
    transition: transform 0.3s ease;
}

.shot-overlay {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: var(--hover-overlay);
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 20px;
    opacity: 0;
    transition: opacity 0.3s ease;
}

.shot-item:hover .shot-overlay {
    opacity: 1;
}

.shot-item:hover .shot-preview img {
    transform: scale(1.05);
}

.shot-title {
    color: white;
    margin: 0;
    font-size: 1rem;
}

.shot-actions {
    display: flex;
    gap: 8px;
}

/* Card Customization */
.card {
    border: none;
    border-radius: 8px;
    overflow: hidden;
    transition: transform 0.2s ease;
}

.card:hover {
    transform: translateY(-2px);
}

.card-body {
    padding: 12px;
}

/* Badges */
.badge.bg-pro {
    background-color: var(--dribbble-pink);
    color: white;
    font-weight: 400;
    font-size: 0.7rem;
}

.badge.bg-team {
    background-color: #0d0c22;
    color: white;
    font-weight: 400;
    font-size: 0.7rem;
}

/* Responsive Adjustments */
@media (max-width: 768px) {
    .shot-item {
        margin-bottom: 16px;
    }
    
    .filters .nav {
        overflow-x: auto;
        flex-wrap: nowrap;
        -webkit-overflow-scrolling: touch;
    }
}
```

## OUTPUT:
<img width="1917" height="886" alt="Screenshot 2025-10-15 111947" src="https://github.com/user-attachments/assets/d3c5c4a0-5df1-43c0-a8ae-a132aeaec0a9" />


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
