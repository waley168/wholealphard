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
                    <a href="https://line.me/R/ti/p/@662hnbde" aria-label="Line" target="_blank" rel="noopener noreferrer"
                        style="--color: #1B64F6; --background-color: transparent;"
                        class="ast-builder-social-element ast-inline-flex ast-behance header-social-item"><span
                            class="ahfb-svg-iconset ast-inline-flex svg-baseline"><svg xmlns="http://www.w3.org/2000/svg"
                                viewBox="0 0 448 512">
                                <path
                                    d="M272.1 204.2v71.1c0 1.8-1.4 3.2-3.2 3.2h-11.4c-1.1 0-2.1-.6-2.6-1.3l-32.6-44v42.2c0 1.8-1.4 3.2-3.2 3.2h-11.4c-1.8 0-3.2-1.4-3.2-3.2v-71.1c0-1.8 1.4-3.2 3.2-3.2H219c1 0 2.1.5 2.6 1.4l32.6 44v-42.2c0-1.8 1.4-3.2 3.2-3.2h11.4c1.8-.1 3.3 1.4 3.3 3.1zm-82-3.2h-11.4c-1.8 0-3.2 1.4-3.2 3.2v71.1c0 1.8 1.4 3.2 3.2 3.2h11.4c1.8 0 3.2-1.4 3.2-3.2v-71.1c0-1.7-1.4-3.2-3.2-3.2zm-27.5 59.6h-31.1v-56.4c0-1.8-1.4-3.2-3.2-3.2h-11.4c-1.8 0-3.2 1.4-3.2 3.2v71.1c0 .9.3 1.6.9 2.2.6.5 1.3.9 2.2.9h45.7c1.8 0 3.2-1.4 3.2-3.2v-11.4c0-1.7-1.4-3.2-3.1-3.2zM332.1 201h-45.7c-1.7 0-3.2 1.4-3.2 3.2v71.1c0 1.7 1.4 3.2 3.2 3.2h45.7c1.8 0 3.2-1.4 3.2-3.2v-11.4c0-1.8-1.4-3.2-3.2-3.2H301v-12h31.1c1.8 0 3.2-1.4 3.2-3.2V234c0-1.8-1.4-3.2-3.2-3.2H301v-12h31.1c1.8 0 3.2-1.4 3.2-3.2v-11.4c-.1-1.7-1.5-3.2-3.2-3.2zM448 113.7V399c-.1 44.8-36.8 81.1-81.7 81H81c-44.8-.1-81.1-36.9-81-81.7V113c.1-44.8 36.9-81.1 81.7-81H367c44.8.1 81.1 36.8 81 81.7zm-61.6 122.6c0-73-73.2-132.4-163.1-132.4-89.9 0-163.1 59.4-163.1 132.4 0 65.4 58 120.2 136.4 130.6 19.1 4.1 16.9 11.1 12.6 36.8-.7 4.1-3.3 16.1 14.1 8.8 17.4-7.3 93.9-55.3 128.2-94.7 23.6-26 34.9-52.3 34.9-81.5z">
                                </path>
                            </svg></span></a>
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

        <div class="entry-content">
            <div class="content">
                <div class="section">
                    <i class="fa fa-rocket" aria-hidden="true"></i>
                    <h3>即時聯繫</h3>
                    <p>從事前訂車起，無論您是需要阿法租車，或是尋求Alphard租車服務，我們的客服人員都能隨時為您提供專業的諮詢並把關。我們瞭解每一位客戶的需求都是獨一無二的，因此，我們始終全程為您提供個性化的服務，以確保您的用車體驗能夠無縫銜接，且能滿足您的各種需求。</p>
                </div>

                <div class="section">
                    <i class="fa fa-check-circle" aria-hidden="true"></i>
                    <h3>合法可靠</h3>
                    <p>我們是政府立案的公司，完全符合政府的各種規定。我們不僅秉持著最高的安全和服務標準，更進一步對所有乘客進行全額投保，確保在您使用我們的阿法或Alphard租車服務時，能夠得到最完善的保障。我們的目標是提供安全可靠的服務，同時確保每位乘客都能擁有愉快的租車經驗。</p>
                </div>

                <div class="section">
                    <i class="fa fa-id-badge" aria-hidden="true"></i>
                    <h3>專業駕駛</h3>
                    <p>我們的駕駛員都是擁有職業執照的專業人員，且每位駕駛員都會定期接受嚴格的考核，以確保他們的專業技能始終保持在最高水準。此外，我們的團隊中也包括擁有國家級禮賓的豐富經驗的駕駛員。無論您選擇我們的阿法租車，或是Alphard租車，我們都確保您將得到最專業、最高水準的駕駛服務。</p>
                </div>
            </div>
        </div>
        <div class="footer-admin">
            <div class="social-media">
                <a href="https://line.me/R/ti/p/@662hnbde" class="icon-media" id="icon1" target="_blank"
                    rel=" noreferrer noopener"><img width="25px"
                        src="https://upload.wikimedia.org/wikipedia/commons/4/41/LINE_logo.svg"> Line預約</a>
                <a href="https://wa.me/886907701070" class="icon-media" id="icon2" target="_blank"
                    rel=" noreferrer noopener"><i class="fa fa-whatsapp fa-lg"></i> WhatsApp預約</a>
                <a href="javascript:void(0)" class="icon-media" id="icon3" @click="toggleImage"><i
                        class="fa fa-wechat fa-lg"></i> WeChat預約</a>
            </div>
        </div>
        <div id="image-container" class="image-container" v-show="isImageVisible">
            <img id="toggle-image" src="https://wholealphard.com/wp-content/uploads/2023/06/wc.png" alt="WeChat加入QRcode">
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            isMenuOpen: false,
            isImageVisible: false, // 新增的data property
        }
    },
    methods: {
        toggleMenu() {
            this.isMenuOpen = !this.isMenuOpen;
        },
        toggleImage() { // 新增的方法
            this.isImageVisible = !this.isImageVisible;
        }
    },
    head: {
        title: 'Your Page Title',
        meta: [
            { hid: 'description', name: 'description', content: 'Your Page Description' }
        ]
    }
}
</script>