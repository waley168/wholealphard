<template>
    <div>
        <header>
            <div class="container">
                <div class="logo">
                    <img class="logo-img" src="https://wholealphard.com/wp-content/uploads/2023/06/whole_alphard_logo.png"
                        alt="logo">
                    <a href="https://wholealphard.com/" rel="home" itemprop="url" class="site-title">總發豪華汽車出租</a>
                </div>

                <div class="menu desktop">
                    <nav>
                        <ul>
                            <li><a href="https://wholealphard.com/">首頁</a></li>
                            <li><a href="https://wholealphard.com/about/">關於總發</a></li>
                            <li class="dropdown">
                                <a href="https://wholealphard.com/alphard/">ALPHARD租車</a>
                                <div class="dropdown-content">
                                    <a href="https://wholealphard.com/alphard-rental/">租車詳細流程</a>
                                    <a href="https://wholealphard.com/alphard-qa/">承租注意事項</a>
                                </div>
                            </li>
                            <li><a href="https://wholealphard.com/faq/">常見問題</a></li>
                            <li><a href="https://wholealphard.com/contact/">聯絡我們</a></li>
                            <li><a href="https://wholealphard.com/portfolio/">花絮集錦</a></li>
                        </ul>
                    </nav>
                </div>
                <div class="social-icons">
                    <a href="#"><i class="social-icon social-icon-facebook"></i>tet</a>
                    <a href="#"><i class="social-icon social-icon-twitter"></i></a>
                    <a href="#"><i class="social-icon social-icon-instagram"></i></a>
                </div>
                <div class="menu-toggle" @click="toggleMenu">&#9776;</div>

            </div>
        </header>

        <div class="menu mobile" v-if="isMenuOpen">
            <nav>
                <ul>
                    <li><a href="https://wholealphard.com/">首頁</a></li>
                    <li><a href="https://wholealphard.com/about/">關於總發</a></li>
                    <li><a href="https://wholealphard.com/alphard/">ALPHARD租車</a></li>
                    <li><a href="https://wholealphard.com/faq/">常見問題</a></li>
                    <li><a href="https://wholealphard.com/contact/">聯絡我們</a></li>
                    <li><a href="https://wholealphard.com/portfolio/">花絮集錦</a></li>
                </ul>
            </nav>
        </div>

        <div class="header-space"></div>

        <slot />
    </div>
</template>

<script>
export default {
    data() {
        return {
            isMenuOpen: false,
        }
    },
    methods: {
        toggleMenu() {
            this.isMenuOpen = !this.isMenuOpen;
        }
    },
    head: {
        title: 'Your Page Title',
        meta: [
            { hid: 'description', name: 'description', content: 'Your Page Description' }
        ],
        link: [
            { rel: 'stylesheet', href: 'https://cdn.jsdelivr.net/npm/fork-awesome@1.2.0/css/fork-awesome.min.css' }
        ]
    }
}
</script>