# Praneet.github.io

![image](https://user-images.githubusercontent.com/94593299/221197116-d6608590-913c-4538-bb49-d9f43c65a119.png)
QR GENERATOR

![image](https://user-images.githubusercontent.com/94593299/221197166-36f5ab6a-badc-4845-810c-aec3ccb84b48.png)
URL SHORTNER


this has both Light mode(BETA) and dark mode

<!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device=width, initial-scale=1.0" />
    <title>QR_CODE_GENERATOR</title>
    <link rel="stylesheet" href="QR.css"/>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body>
<div class="video-bg">
    <video width="320" height="240" autoplay loop muted>
        <source
                src="https://assets.codepen.io/3364143/7btrrd.mp4"
                type="video/mp4"
        />
        Your browser does not support the video tag.
    </video>
</div>
<div class="dark-light">
    <svg
            viewBox="0 0 24 24"
            stroke="currentColor"
            stroke-width="1.5"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
    >
        <path d="M21 12.79A9 9 0 1111.21 3 7 7 0 0021 12.79z" />
    </svg>
</div>
<div class="app">
    <div class="header">
        <div class="menu-circle"></div>
    </div>
    <div class="wrapper">
        <div class="left-side">
            <div class="side-wrapper">
                <div class="side-title">Apps</div>
                <div class="side-menu">
                    <a href="#">
                        <svg viewBox="0 0 512 512">
                            <g xmlns="http://www.w3.org/2000/svg" fill="currentColor">
                                <path
                                        d="M0 0h128v128H0zm0 0M192 0h128v128H192zm0 0M384 0h128v128H384zm0 0M0 192h128v128H0zm0 0"
                                        data-original="#bfc9d1"
                                />
                            </g>
                            <path
                                    xmlns="http://www.w3.org/2000/svg"
                                    d="M192 192h128v128H192zm0 0"
                                    fill="currentColor"
                                    data-original="#82b1ff"
                            />
                            <path
                                    xmlns="http://www.w3.org/2000/svg"
                                    d="M384 192h128v128H384zm0 0M0 384h128v128H0zm0 0M192 384h128v128H192zm0 0M384 384h128v128H384zm0 0"
                                    fill="currentColor"
                                    data-original="#bfc9d1"
                            />
                        </svg>
                        QR Generator
                    </a>
                    <a href="url.html">
                        <svg viewBox="0 0 512 512" fill="currentColor">
                            <path
                                    d="M448.773 235.551A135.893 135.893 0 00451 211c0-74.443-60.557-135-135-135-47.52 0-91.567 25.313-115.766 65.537-32.666-10.59-66.182-6.049-93.794 12.979-27.612 19.013-44.092 49.116-45.425 82.031C24.716 253.788 0 290.497 0 331c0 7.031 1.703 13.887 3.006 20.537l.015.015C12.719 400.492 56.034 436 106 436h300c57.891 0 106-47.109 106-105 0-40.942-25.053-77.798-63.227-95.449z"
                            />
                        </svg>
                        Url Shortener
                    </a>
                </div>
            </div>
        </div>
        <div class="main-container">
            <div class="content-wrapper">
                <div class="content-wrapper-header">
                    <div class="content-wrapper-context">
                        <h3 class="img-content font-bold">QRGEN</h3>
                        <div class="content-text">
                            Convert your any text or link in QR Code with our QR GEN.
                        </div>
                        <button class="content-button">Start Today</button>
                    </div>
                    <img
                            class="content-wrapper-img"
                            src="https://assets.codepen.io/3364143/glass.png"
                            alt=""
                    />
                </div>
                <div class="flex w-full h-full">
                    <div class="p-4 my-3 h-full w-1/2 app-card">
                        <div class="sm:max-w-lg w-full p-10 bg-white rounded-xl z-10">
                            <div class="text-center">
                                <h2 class="mt-5 text-3xl font-bold text-gray-900">
                                    QR Generator
                                </h2>
                                <p class="mt-2 text-sm text-gray-400">
                                    Generate your QR Code with our QR Generator
                                </p>
                            </div>
                            <div class="mt-8 space-y-3">
                                <div class="grid grid-cols-1 space-y-2">
                                    <label
                                            class="text-sm font-bold text-gray-500 tracking-wide"
                                    >Text OR Url</label
                                    >
                                    <input
                                            class="text-gray-800 p-2 border border-gray-300 rounded-lg focus:outline-none focus:border-indigo-500"
                                            type="text"
                                            placeholder="www.google.com"
                                            id="qrText"
                                            onkeydown="generateQR()"
                                    />
                                </div>

                                <button
                                        type="submit"
                                        onclick="generateQR()"
                                        class="my-5 w-full flex justify-center bg-blue-500 text-gray-100 p-4 rounded-full tracking-wide font-semibold focus:outline-none focus:shadow-outline hover:bg-blue-600 shadow-lg cursor-pointer transition ease-in duration-300"
                                >
                                    Generate QR Code
                                </button>
                            </div>
                        </div>
                    </div>
                    <div class="p-4 my-3 h-full w-1/2 app-card flex justify-center gap-4">
                        <div class="flex items-center w-full flex-col gap-4">
                            <h3 class="img-content font-bold">QR Code</h3>
                            <img
                                    src="https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=QR+Code+Generator"
                                    alt=""
                                    width="150"
                                    height="150"
                                    class="object-contain shadow-md bg-white mt-4"
                                    id="qrImage"
                            />
                            <h2 class="text-2xl text-white" id="qrText2"></h2>
                        </div>

                        <div class="flex w-full gap-2">
                            <button
                                    id="pngdownload"
                                    class="flex items-center justify-center w-1/2 h-12 bg-sky-500 text-white font-bold rounded-l-lg"
                            >
                                DOWNLOAD
                            </button>
                            <button
                                    id="sharebutton"
                                    class="flex items-center justify-center w-1/2 h-12 bg-yellow-500 text-white font-bold rounded-r-lg"
                            >
                                SHARE
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="overlay-app"></div>
</div>
<script
        src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.3/jquery.min.js"
        integrity="sha512-STof4xm1wgkfm7heWqFJVn58Hm3EtS31XFaagaa8VMReCXAkQnJZ+jEy8PCC/iT18dFy95WcExNHFTqLyp72eQ=="
        crossorigin="anonymous"
        referrerpolicy="no-referrer"
></script>
<script src="qr.js"></script>
<script src=
                "https://cdnjs.cloudflare.com/ajax/libs/axios/0.19.2/axios.min.js">
</script>
<script>
    let imgBox = document.getElementById("imgBox");
    let qrImage = document.getElementById("qrImage");
    let qrText = document.getElementById("qrText");
    let sharebutton = document.getElementById("sharebutton");
    let pngdownload = document.getElementById("pngdownload");
    let qrText2 = document.getElementById("qrText2");

    function generateQR() {
        if (qrText.value.length > 0) {
            qrImage.src =
                "https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=" +
                qrText.value;
            qrText2.innerHTML = qrText.value;
        } else {
            qrText.classList.add("error");
            setTimeout(() => {
                qrText.classList.remove("error");
            }, 1000);
        }
    }

    pngdownload.onclick = function () {
        axios
        ({
            url: qrImage.src,
            method: "GET",
            responseType: "blob",
        })
            .then((response) => {
                const url = window.URL.createObjectURL(new Blob([response.data]));
                const link = document.createElement("a");
                link.href = url;
                link.setAttribute("download", "QR Code.png");
                document.body.appendChild(link);
                link.click();
            });
    };
    sharebutton.onclick = function () {
        if(navigator.share){
            navigator.share({
                title: 'QR Code',
                text: 'QR Code',
                url: qrImage.src,
            })
                .then(() => console.log('Successful share'))
                .catch((error) => console.log('Error sharing', error));
        }
    };
</script>
</body>
</html>



*/*{
    margin: 0;
    padding: 0;
    font-family: sans-serif;
    box-sizing: border-box;
}
body{
    background: #262a2f;
}
.container
{
    width: 400px;
    padding: 25px 35px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    background: #fff;
    border-radius: 10px;
}
.container p
{
    font-weight: 600;
    font-size: 15px;
    margin-bottom: 8px;
}
.container input
{
    width: 100%;
    height: 50px;
    border: 1px solid #494;
    outline: 0;
    padding: 10px;
    margin: 10px 0 20px;
    border-radius: 5px;
}
.container button
{
    width: 100%;
    height: 50px;
    background: #494;
    color: #fff;
    border: 0;
    outline: 0;
    border-radius: 5px;
    box-shadow: 0 10px 10px rgba(0,0,0,0.1);
    cursor: pointer;
    margin: 20px 0;
    font-weight:500;
}
#imgBox{
    width: 200px;
    border-radius: 5px;
    max-height: 0;
    overflow: hidden;
    transition: max-height 1s;
}
#imgBox img{
    width: 100%;
    padding: 10px;
}
#imgBox.show-img{
    max-height: 300px;
    margin: 10px auto;
    border: 1px solid #d1d1d1;
}
.error{
    animation:  shake 0.1s linear 10;
}
@keyframes shake {
    0%{
        transform: translateX(0);
    }
    25%{
        transform: translateX(-2px);
    }
    50%{
        transform: translateX(0);
    }
    75%{
        transform: translateX(2px);
    }
    100%{
        transform: translateX(0);
    }
}
*/
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap");
* {
    outline: none;
    box-sizing: border-box;
}

:root {
    --theme-bg-color: rgba(16 18 27 / 40%);
    --border-color: rgba(113 119 144 / 25%);
    --theme-color: #f9fafb;
    --inactive-color: rgb(113 119 144 / 78%);
    --body-font: "Poppins", sans-serif;
    --hover-menu-bg: rgba(12 15 25 / 30%);
    --content-title-color: #999ba5;
    --content-bg: rgb(146 151 179 / 13%);
    --button-inactive: rgb(249 250 251 / 55%);
    --dropdown-bg: #21242d;
    --dropdown-hover: rgb(42 46 60);
    --popup-bg: rgb(22 25 37);
    --search-bg: #14162b;
    --overlay-bg: rgba(36, 39, 59, 0.3);
    --scrollbar-bg: rgb(1 2 3 / 40%);
}

.light-mode {
    --theme-bg-color: rgb(255 255 255 / 31%);
    --theme-color: #3c3a3a;
    --inactive-color: #333333;
    --button-inactive: #3c3a3a;
    --search-bg: rgb(255 255 255 / 31%);
    --dropdown-bg: #f7f7f7;
    --overlay-bg: rgb(255 255 255 / 30%);
    --dropdown-hover: rgb(236 236 236);
    --border-color: rgb(255 255 255 / 35%);
    --popup-bg: rgb(255 255 255);
    --hover-menu-bg: rgba(255 255 255 / 35%);
    --scrollbar-bg: rgb(255 253 253 / 57%);
    --content-title-color: --theme-color;
}

html {
    box-sizing: border-box;
    -webkit-font-smoothing: antialiased;
}

body {
    font-family: sans-serif;
    background-image: url(https://wallpapershome.com/images/wallpapers/macos-big-sur-1280x720-dark-wwdc-2020-22655.jpg);
    background-size: cover;
    background-position: center;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    padding: 2em;
    width: 100%;
    height: 100vh;
}
@media screen and (max-width: 480px) {
    body {
        padding: 0.8em;
    }
}

.video-bg {
    position: fixed;
    right: 0;
    top: 0;
    width: 100%;
    height: 100%;
}
.video-bg video {
    width: 100%;
    height: 100%;
    -o-object-fit: cover;
    object-fit: cover;
}

img {
    max-width: 100%;
}

.dark-light {
    position: fixed;
    bottom: 50px;
    right: 30px;
    background-color:var(--dropdown-bg);
    box-shadow: -1px 3px 8px -1px rgba(0, 0, 0, 0.2);
    padding: 8px;
    border-radius: 50%;
    z-index: 3;
    cursor: pointer;
}
.dark-light svg {
    width: 24px;
    flex-shrink: 0;
    fill: #ffce45;
    stroke: #ffce45;
    transition: 0.5s;
}

.light-mode .dark-light svg {
    fill: transparent;
    stroke: var(--theme-color);
}
.light-mode .profile-img {
    border: 2px solid var(--theme-bg-color);
}
.light-mode .content-section ul {
    background-color: var(--theme-bg-color);
}
.light-mode .pop-up__title {
    border-color: var(--theme-color);
}
.light-mode .dropdown.is-active ul {
    background-color: rgba(255, 255, 255, 0.94);
}

body.light-mode:before,
body.light-mode .video-bg:before {
    content: "";
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100vh;
    background: linear-gradient(180deg, rgba(255, 255, 255, 0.72) 0%, rgba(255, 255, 255, 0.45) 100%);
    -webkit-backdrop-filter: saturate(3);
    backdrop-filter: saturate(3);
}

.app {
    background-color: var(--theme-bg-color);
    max-width: 1250px;
    max-height: 860px;
    height: 90vh;
    display: flex;
    flex-direction: column;
    overflow: hidden;
    position: relative;
    width: 100%;
    border-radius: 14px;
    backdrop-filter: blur(20px);
    -webkit-backdrop-filter: blur(20px);
    font-size: 15px;
    font-weight: 500;
}

.header {
    display: flex;
    align-items: center;
    flex-shrink: 0;
    height: 58px;
    width: 100%;
    border-bottom: 1px solid var(--border-color);
    padding: 0 30px;
    white-space: nowrap;
}
@media screen and (max-width: 480px) {
    .header {
        padding: 0 16px;
    }
}
.header-menu {
    display: flex;
    align-items: center;
}
.header-menu a {
    padding: 20px 30px;
    text-decoration: none;
    color: var(--inactive-color);
    border-bottom: 2px solid transparent;
    transition: 0.3s;
}
@media screen and (max-width: 610px) {
    .header-menu a:not(.main-header-link) {
        display: none;
    }
}
.header-menu a.is-active, .header-menu a:hover {
    color: var(--theme-color);
    border-bottom: 2px solid var(--theme-color);
}

.notify {
    position: relative;
}
.notify:before {
    content: "";
    position: absolute;
    background-color: #3a6df0;
    width: 6px;
    height: 6px;
    border-radius: 50%;
    right: 20px;
    top: 16px;
}
@media screen and (max-width: 1055px) {
    .notify {
        display: none;
    }
}

.menu-circle {
    width: 15px;
    height: 15px;
    background-color: #f96057;
    border-radius: 50%;
    box-shadow: 24px 0 0 0 #f8ce52, 48px 0 0 0 #5fcf65;
    margin-right: 195px;
    flex-shrink: 0;
}
@media screen and (max-width: 945px) {
    .menu-circle {
        display: none;
    }
}

.search-bar {
    height: 40px;
    display: flex;
    width: 100%;
    max-width: 400px;
    padding-left: 16px;
    border-radius: 4px;
}
.search-bar input {
    width: 100%;
    height: 100%;
    border: none;
    background-color: var(--search-bg);
    border-radius: 4px;
    font-family: var(--body-font);
    font-size: 15px;
    font-weight: 500;
    padding: 0 20px 0 40px;
    box-shadow: 0 0 0 2px rgba(134, 140, 160, 0.02);
    background-image: url("data:image/svg+xml;charset=UTF-8,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 56.966 56.966' fill='%23717790c7'%3e%3cpath d='M55.146 51.887L41.588 37.786A22.926 22.926 0 0046.984 23c0-12.682-10.318-23-23-23s-23 10.318-23 23 10.318 23 23 23c4.761 0 9.298-1.436 13.177-4.162l13.661 14.208c.571.593 1.339.92 2.162.92.779 0 1.518-.297 2.079-.837a3.004 3.004 0 00.083-4.242zM23.984 6c9.374 0 17 7.626 17 17s-7.626 17-17 17-17-7.626-17-17 7.626-17 17-17z'/%3e%3c/svg%3e");
    background-size: 14px;
    background-repeat: no-repeat;
    background-position: 16px 48%;
    color: var(--theme-color);
}
.search-bar input::-moz-placeholder {
    font-family: var(--body-font);
    color: var(--inactive-color);
    font-size: 15px;
    font-weight: 500;
}
.search-bar input:-ms-input-placeholder {
    font-family: var(--body-font);
    color: var(--inactive-color);
    font-size: 15px;
    font-weight: 500;
}
.search-bar input::placeholder {
    font-family: var(--body-font);
    color: var(--inactive-color);
    font-size: 15px;
    font-weight: 500;
}

.header-profile {
    display: flex;
    align-items: center;
    padding: 0 16px 0 40px;
    margin-left: auto;
    flex-shrink: 0;
}
.header-profile svg {
    width: 22px;
    color: #f9fafb;
    flex-shrink: 0;
}

.notification {
    position: relative;
}
.notification-number {
    position: absolute;
    background-color: #3a6df0;
    width: 16px;
    height: 16px;
    border-radius: 50%;
    font-size: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #fff;
    right: -6px;
    top: -6px;
}
.notification + svg {
    margin-left: 22px;
}
@media screen and (max-width: 945px) {
    .notification + svg {
        display: none;
    }
}

.profile-img {
    width: 32px;
    height: 32px;
    border-radius: 50%;
    -o-object-fit: cover;
    object-fit: cover;
    border: 2px solid var(--theme-color);
    margin-left: 22px;
}

.wide .header-menu,
.wide .header-profile {
    display: none;
}
.wide .search-bar {
    max-width: 600px;
    margin: auto;
    transition: 0.4s;
    box-shadow: 0 0 0 1px var(--border-color);
    padding-left: 0;
}
.wide .menu-circle {
    margin-right: 0;
}

.wrapper {
    display: flex;
    flex-grow: 1;
    overflow: hidden;
}

.left-side {
    flex-basis: 240px;
    border-right: 1px solid var(--border-color);
    padding: 26px;
    overflow: auto;
    flex-shrink: 0;
}
@media screen and (max-width: 945px) {
    .left-side {
        display: none;
    }
}

.side-wrapper + .side-wrapper {
    margin-top: 20px;
}

.side-title {
    color: var(--inactive-color);
    margin-bottom: 14px;
}

.side-menu {
    display: flex;
    flex-direction: column;
    white-space: nowrap;
}
.side-menu a {
    text-decoration: none;
    color: var(--theme-color);
    display: flex;
    align-items: center;
    font-weight: 400;
    padding: 10px;
    font-size: 14px;
    border-radius: 6px;
    transition: 0.3s;
}
.side-menu a:hover {
    background-color: var(--hover-menu-bg);
}
.side-menu svg {
    width: 16px;
    margin-right: 8px;
}

.updates {
    position: relative;
    top: 0;
    right: 0;
    margin-left: auto;
    width: 18px;
    height: 18px;
    font-size: 11px;
}

.main-header {
    display: flex;
    align-items: center;
    border-bottom: 1px solid var(--border-color);
    height: 58px;
    flex-shrink: 0;
}
.main-header .header-menu {
    margin-left: 150px;
}
@media screen and (max-width: 1055px) {
    .main-header .header-menu {
        margin: auto;
    }
}
.main-header .header-menu a {
    padding: 20px 24px;
}

.main-container {
    display: flex;
    flex-direction: column;
    flex-grow: 1;
}

.menu-link-main {
    text-decoration: none;
    color: var(--theme-color);
    padding: 0 30px;
}
@media screen and (max-width: 1055px) {
    .menu-link-main {
        display: none;
    }
}

.content-wrapper {
    display: flex;
    flex-direction: column;
    color: var(--theme-color);
    padding: 20px 40px;
    height: 100%;
    overflow: auto;
    background-color: var(--theme-bg-color);
}
@media screen and (max-width: 510px) {
    .content-wrapper {
        padding: 20px;
    }
}
.content-wrapper-header {
    display: flex;
    align-items: center;
    width: 100%;
    justify-content: space-between;
    background-image: url("https://www.transparenttextures.com/patterns/cubes.png"), linear-gradient(to right top, #cf4af3, #e73bd7, #f631bc, #fd31a2, #ff3a8b, #ff4b78, #ff5e68, #ff705c, #ff8c51, #ffaa49, #ffc848, #ffe652);
    border-radius: 14px;
    padding: 20px 40px;
}
@media screen and (max-width: 415px) {
    .content-wrapper-header {
        padding: 20px;
    }
}
.content-wrapper.overlay {
    pointer-events: none;
    transition: 0.3s;
    background-color: var(--overlay-bg);
}

.overlay-app {
    width: 100%;
    height: 100%;
    position: fixed;
    left: 0;
    top: 0;
    pointer-events: all;
    background-color: rgba(36, 39, 59, 0.8);
    opacity: 0;
    visibility: hidden;
    transition: 0.3s;
}
.overlay-app.is-active {
    visibility: visible;
    opacity: 1;
}

.img-content {
    font-weight: 500;
    font-size: 17px;
    display: flex;
    align-items: center;
    margin: 0;
}
.img-content svg {
    width: 28px;
    margin-right: 14px;
}

.content-text {
    font-weight: 400;
    font-size: 14px;
    margin-top: 16px;
    line-height: 1.7em;
    color: #ebecec;
    display: -webkit-box;
    -webkit-line-clamp: 4;
    -webkit-box-orient: vertical;
    overflow: hidden;
    text-overflow: ellipsis;
}

.content-wrapper-context {
    max-width: 350px;
}

.content-button {
    background-color: #3a6df0;
    border: none;
    padding: 8px 26px;
    color: #fff;
    border-radius: 20px;
    margin-top: 16px;
    cursor: pointer;
    transition: 0.3s;
    white-space: nowrap;
}

.content-wrapper-img {
    width: 186px;
    -o-object-fit: cover;
    object-fit: cover;
    margin-top: -25px;
    -o-object-position: center;
    object-position: center;
}
@media screen and (max-width: 570px) {
    .content-wrapper-img {
        width: 110px;
    }
}

.content-section {
    margin-top: 30px;
    display: flex;
    flex-direction: column;
}
.content-section-title {
    color: var(--content-title-color);
    margin-bottom: 14px;
}
.content-section ul {
    display: flex;
    flex-direction: column;
    width: 100%;
    height: 100%;
    justify-content: space-around;
    background-color: var(--content-bg);
    padding-left: 0;
    margin: 0;
    border-radius: 14px;
    border: 1px solid var(--theme-bg-color);
    cursor: pointer;
}
.content-section ul li {
    list-style: none;
    padding: 10px 18px;
    display: flex;
    align-items: center;
    font-size: 16px;
    width: 100%;
    height: 100%;
    white-space: nowrap;
    transition: 0.3s;
}
.content-section ul li:hover {
    background-color: var(--theme-bg-color);
}
.content-section ul li:hover:first-child {
    border-radius: 13px 13px 0 0;
}
.content-section ul li:hover:last-child {
    border-radius: 0 0 13px 13px;
}
.content-section ul li + li {
    border-top: 1px solid var(--border-color);
}
.content-section ul svg {
    width: 28px;
    border-radius: 6px;
    margin-right: 16px;
    flex-shrink: 0;
}

.products {
    display: flex;
    align-items: center;
    width: 150px;
}
@media screen and (max-width: 480px) {
    .products {
        width: 120px;
    }
}

.status {
    margin-left: auto;
    width: 140px;
    font-size: 15px;
    position: relative;
}
@media screen and (max-width: 700px) {
    .status {
        display: none;
    }
}
.status-circle {
    width: 6px;
    height: 6px;
    background-color: #396df0;
    position: absolute;
    border-radius: 50%;
    top: 4px;
    left: -20px;
}
.status-circle.green {
    background-color: #3bf083;
}
.status-button {
    font-size: 15px;
    margin-top: 0;
    padding: 6px 24px;
}
@media screen and (max-width: 390px) {
    .status-button {
        padding: 6px 14px;
    }
}
.status-button.open {
    background: none;
    color: var(--button-inactive);
    border: 1px solid var(--button-inactive);
}
.status-button:not(.open):hover {
    color: #fff;
    border-color: #fff;
}

.content-button:not(.open):hover {
    background: #1e59f1;
}

.menu {
    width: 5px;
    height: 5px;
    background-color: var(--button-inactive);
    border-radius: 50%;
    box-shadow: 7px 0 0 0 var(--button-inactive), 14px 0 0 0 var(--button-inactive);
    margin: 0 12px;
}

@media screen and (max-width: 415px) {
    .adobe-product .menu {
        display: none;
    }
}
.dropdown {
    position: relative;
    height: 53px;
    width: 40px;
    top: -24px;
    display: flex;
    left: -5px;
    background: transparent;
    border: none;
    cursor: pointer;
}
.dropdown ul {
    position: absolute;
    background: var(--dropdown-bg);
    height: 110px;
    width: 120px;
    right: 0;
    top: 20px;
    pointer-events: none;
    opacity: 0;
    transform: translatey(10px);
    transition: all 0.4s ease;
}
.dropdown ul li a {
    text-decoration: none;
    color: var(--theme-color);
    font-size: 12px;
}

.dropdown.is-active ul {
    opacity: 1;
    pointer-events: all;
    transform: translatey(25px);
}
.dropdown.is-active ul li:hover {
    background-color: var(--dropdown-hover);
}

.button-wrapper {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    width: 187px;
    margin-left: auto;
}
@media screen and (max-width: 480px) {
    .button-wrapper {
        width: auto;
    }
}

.pop-up {
    position: absolute;
    padding: 30px 40px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    overflow-y: auto;
    box-shadow: 0px 6px 30px rgba(0, 0, 0, 0.4);
    transition: all 0.3s;
    z-index: 10;
    background-color: var(--popup-bg);
    width: 500px;
    visibility: hidden;
    opacity: 0;
    border-radius: 6px;
    display: flex;
    flex-direction: column;
    white-space: normal;
}
@media screen and (max-width: 570px) {
    .pop-up {
        width: 100%;
    }
}
.pop-up.visible {
    visibility: visible;
    opacity: 1;
}
.pop-up__title {
    padding-bottom: 20px;
    border-bottom: 1px solid var(--border-color);
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.pop-up__subtitle {
    white-space: normal;
    margin: 20px 0;
    font-size: 14px;
    font-weight: 400;
    line-height: 1.8em;
}
.pop-up__subtitle a {
    color: var(--theme-color);
}

.content-button-wrapper .content-button.status-button.open.close {
    width: auto;
}

.content-section .close {
    margin-right: 0;
    width: 24px;
}

.checkbox-wrapper {
    display: flex;
    align-items: center;
    font-size: 14px;
    font-weight: 400;
}
.checkbox-wrapper + .checkbox-wrapper {
    margin: 20px 0 40px;
}

.checkbox {
    display: none;
}

.checkbox + label {
    display: flex;
    align-items: center;
}
.checkbox + label:before {
    content: "";
    margin-right: 10px;
    width: 15px;
    height: 15px;
    border: 1px solid var(--theme-color);
    border-radius: 4px;
    cursor: pointer;
    flex-shrink: 0;
}

.checkbox:checked + label:before {
    background-color: #3a6df0;
    border-color: #3a6df0;
    background-image: url("data:image/svg+xml;charset=UTF-8,%3csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' viewBox='0 0 24 24' fill='none' stroke='%23fff' stroke-width='3' stroke-linecap='round' stroke-linejoin='round' class='feather feather-check'%3e%3cpath d='M20 6L9 17l-5-5'/%3e%3c/svg%3e");
    background-position: 50%;
    background-size: 12px;
    background-repeat: no-repeat;
}

.content-button-wrapper {
    margin-top: auto;
    margin-left: auto;
}
.content-button-wrapper .open {
    margin-right: 8px;
}

.apps-card {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    width: calc(100% + 20px);
}

.app-card {
    display: flex;
    flex-direction: column;
    width: 100%;
    font-size: 16px;
    background-color: var(--content-bg);
    border-radius: 14px;
    border: 1px solid var(--theme-bg-color);
    padding: 20px;
    cursor: pointer;
    transition: 0.3s ease;
}
.app-card:hover {
    transform: scale(1.02);
    background-color: var(--theme-bg-color);
}
.app-card svg {
    width: 28px;
    border-radius: 6px;
    margin-right: 12px;
    flex-shrink: 0;
}
.app-card + .app-card {
    margin-left: 20px;
}
.app-card span {
    display: flex;
    align-items: center;
}
.app-card__subtext {
    font-size: 14px;
    font-weight: 400;
    line-height: 1.6em;
    margin-top: 20px;
    border-bottom: 1px solid var(--border-color);
    padding-bottom: 20px;
}
.app-card-buttons {
    display: flex;
    align-items: center;
    margin-left: auto;
    margin-top: 16px;
}
@media screen and (max-width: 1110px) {
    .app-card {
        width: calc(50% - 20px);
    }
    .app-card:last-child {
        margin-top: 20px;
        margin-left: 0px;
    }
}
@media screen and (max-width: 565px) {
    .app-card {
        width: calc(100% - 20px);
        margin-top: 20px;
    }
    .app-card + .app-card {
        margin-left: 0;
    }
}

::-webkit-scrollbar {
    width: 6px;
    border-radius: 10px;
}

::-webkit-scrollbar-thumb {
    background: var(--scrollbar-bg);
    border-radius: 10px;
}
