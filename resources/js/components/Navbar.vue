<template>
    <nav class="navbar">
        <div class="navbar-container">
            <a href="#" class="logo">
                Portfolio
            </a>

            <div class="nav-menu">
                <a href="#">Home</a>
                <a href="#about">Tentang Saya</a>
                <a href="#experience">Pengalaman</a>
                <a href="#education">Pendidikan</a>
                <a href="#skills">Keahlian</a>
                <a href="#portfolio">Portfolio</a>
            </div>
        </div>
    </nav>
</template>

<style scoped>
.navbar {
    width: 100%;
    background: white;
    border-bottom: 1px solid #eeeeee;
    position: sticky;
    top: 0;
    z-index: 100;
}

.navbar-container {
    max-width: 1200px;
    margin: auto;
    padding: 20px 30px;

    display: flex;
    align-items: center;
    justify-content: space-between;
}

.logo {
    font-size: 22px;
    font-weight: bold;
    color: #333;
    text-decoration: none;
}

.nav-menu {
    display: flex;
    gap: 28px;
}

.nav-menu a {
    color: #555;
    text-decoration: none;
    font-size: 15px;
}

.nav-menu a:hover {
    color: #000;
}

@media (max-width: 800px) {
    .navbar-container {
        flex-direction: column;
        gap: 15px;
    }

    .nav-menu {
        gap: 15px;
        flex-wrap: wrap;
        justify-content: center;
    }
}
</style>