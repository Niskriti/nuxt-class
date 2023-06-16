<template>
<div>
    <header>
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
            <div class="container">
                <a class="navbar-brand" href="#">Navbar</a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <nuxt-link to="/" class="nav-link">home</nuxt-link>
                        </li>
                        <li class="nav-item">
                            <nuxt-link to="/about" class="nav-link">about</nuxt-link>
                        </li>
                        <li class="nav-item">
                            <nuxt-link to="/contact" class="nav-link">contact</nuxt-link>
                        </li>
                        <li class="nav-item">
                            <nuxt-link to="/service" class="nav-link">service</nuxt-link>
                        </li>
                        <li class="nav-item">
                            <nuxt-link to="/products" class="nav-link">products</nuxt-link>
                        </li>
                    </ul>
                    <form class="d-flex">
                        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                        <button class="btn btn-outline-success" type="submit">Search</button>
                    </form>
                </div>
            </div>
        </nav>
    </header>

    <main>
        <slot></slot>
    </main>

    <footer>
        <section>
            <div class="container">
                <div class="row">
                    <div class="col-md-3">
                        <img src="https://codeit.com.np/images/1642171339codeIT%20logo.png" alt="" width="300 px">
                        <p>9862130505,025-525163</p>
                        <p>info@code-it.com.np</p>
                        <p>prithvi path,Dharan</p>
                    </div>
                    <div class="col-md-3">
                        <h1>Quick links</h1>
                        <p>about us</p>
                        <p>contact us</p>
                        <p>gallery</p>
                        <p>Blog</p>
                    </div>
                    <div class="col-md-3">
                        <h1>Bank Accout Detail</h1>
                        <p>Bank:Nepal Bank limited</p>
                        <p>Accout name: Code-it</p>
                        <p>Ac/no.: 608090700000</p>
                        <P>Branch: Dharan</P>
                        <img src="https://codeit.com.np/asset/img/fonepay-bg.png" alt="" width="100 px">
                        <img src="https://codeit.com.np/asset/img/codeit-qr.jpg" alt="" width="150 px">
                    </div>
                    <div class="col-md-3">
                <h1>Download App</h1>
                <p>Download our mobile app</p>
                <img src="https://codeit.com.np/mobile/appstore.png" alt="">
                <img src="https://codeit.com.np/mobile/googleplay.png" alt="">
            </div>
                </div>
                

            </div>
           

        </section>
    </footer>

</div>
</template>
