<template>
    <div class="containerPage">
        <header>
            <div class="upperRightsideContainer">
                <div class="linkContainer">
                    <a href="https://mail.google.com/mail/u/0/#inbox" class="link">Gmail</a>
                </div>
                <div class="linkContainer">
                    <a href="" class="link">Images</a>
                </div>
                <div class="indexComponent">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 5.25h16.5m-16.5 4.5h16.5m-16.5 4.5h16.5m-16.5 4.5h16.5" />
                    </svg>
                </div>
                <div class="indexComponent">
                    <div class="componentInnerCircle">
                        <p>M</p>
                    </div>
                </div>
            </div>
        </header>
        <div class="body">
            <div class="logoContainer">
                <p id="logo">Boogle</p>
            </div>
            <div class="searchBar">
                <SearchBar/>
            </div>
            <div class="recentPages">
                <RecentPages />
            </div>
        </div>
        <footer>
            <div class="mhsfn">
                © mhsfn
            </div>
        </footer>
    </div>
</template>

<script>

</script>

<style scoped>
    .linkContainer {
        margin-right: 15px;
    }
    
    .componentInnerCircle {
        background-color: #78909c;
        border-radius: 50%;
        width: 30px;
        height: 30px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .indexComponent {
        cursor: pointer;
        border-radius: 50%;
        width: 45px;
        height: 45px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .indexComponent:hover {
        background-color: #505050;
    }

    .link {
        font-size: 13px;
    }

    .link:hover {
        text-decoration: underline;
    }

    .containerPage {
        background-color: #35363a;     
        color: #ffffff;
        position: absolute;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        font-family: sans-serif;
    }
    .upperRightsideContainer {
        display: flex;
        flex-direction: row;
        /* gap: 15px; */
        justify-content: right;
        margin: 15px;
        align-items: center;
    }
    .mhsfn {
        display: flex;
        flex-direction: row;
        gap: 15px;
        justify-content: right;
        margin: 15px;
    }

    .body {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        left: 50%;
        right: 50%;
        bottom: 50%;
        top: 50%;
    }

    .logoContainer {
        margin-top: 75px;
    }
    .searchBar {
        margin: 10px;
    }

    footer {
        position: absolute;
        bottom: 0;
        right: 0;
    }

    #logo {
        font-size: 90px;
    }
</style>