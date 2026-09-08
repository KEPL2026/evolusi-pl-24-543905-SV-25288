<template>
    <main>
        <section class="hero">
            <div class="hero-content">
                <p class="subtitle">SELAMAT DATANG DI PORTFOLIO SAYA</p>

                <h1>
                    Halo, saya
                    <span>Nama Ayah</span>
                </h1>

                <p class="description">
                    Seorang profesional dengan pengalaman dan keahlian
                    di bidang yang saya tekuni.
                </p>

                <a href="#about" class="button">
                    Tentang Saya
                </a>
            </div>
        </section>

        <section id="about" class="about">
            <p class="subtitle">TENTANG SAYA</p>

            <h2>Pengalaman dan perjalanan saya</h2>

            <p>
                Website ini berisi informasi mengenai profil,
                pengalaman kerja, pendidikan, keahlian, dan
                portfolio yang telah saya kerjakan.
            </p>
        </section>
    </main>
</template>

<style scoped>
.hero {
    min-height: 75vh;
    display: flex;
    align-items: center;
    padding: 60px 10%;
    background: #f5f5f5;
}

.hero-content {
    max-width: 700px;
}

.subtitle {
    font-size: 14px;
    font-weight: bold;
    letter-spacing: 2px;
    color: #777;
}

h1 {
    font-size: 52px;
    line-height: 1.2;
    margin: 15px 0;
}

h1 span {
    display: block;
    color: #555;
}

.description {
    font-size: 18px;
    line-height: 1.7;
    color: #666;
    margin-bottom: 30px;
}

.button {
    display: inline-block;
    padding: 12px 24px;
    background: #333;
    color: white;
    text-decoration: none;
    border-radius: 5px;
}

.button:hover {
    background: #555;
}

.about {
    padding: 80px 10%;
    text-align: center;
}

.about h2 {
    font-size: 32px;
    margin: 15px 0;
}

.about > p:last-child {
    max-width: 650px;
    margin: auto;
    line-height: 1.7;
    color: #666;
}

@media (max-width: 700px) {
    h1 {
        font-size: 38px;
    }

    .hero {
        padding: 50px 7%;
    }
}
</style>