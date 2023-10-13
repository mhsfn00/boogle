<template>
    <div class="searchBar">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 searchIcon magnifyingGlass">
            <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
        </svg>
        <input class="searchInput" placeholder="Google search"/>
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 searchIcon microphone">
          <path stroke-linecap="round" stroke-linejoin="round" d="M12 18.75a6 6 0 006-6v-1.5m-6 7.5a6 6 0 01-6-6v-1.5m6 7.5v3.75m-3.75 0h7.5M12 15.75a3 3 0 01-3-3V4.5a3 3 0 116 0v8.25a3 3 0 01-3 3z" />
        </svg>
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 searchIcon camera">
            <path stroke-linecap="round" stroke-linejoin="round" d="M6.827 6.175A2.31 2.31 0 015.186 7.23c-.38.054-.757.112-1.134.175C2.999 7.58 2.25 8.507 2.25 9.574V18a2.25 2.25 0 002.25 2.25h15A2.25 2.25 0 0021.75 18V9.574c0-1.067-.75-1.994-1.802-2.169a47.865 47.865 0 00-1.134-.175 2.31 2.31 0 01-1.64-1.055l-.822-1.316a2.192 2.192 0 00-1.736-1.039 48.774 48.774 0 00-5.232 0 2.192 2.192 0 00-1.736 1.039l-.821 1.316z" />
            <path stroke-linecap="round" stroke-linejoin="round" d="M16.5 12.75a4.5 4.5 0 11-9 0 4.5 4.5 0 019 0zM18.75 10.5h.008v.008h-.008V10.5z" />
        </svg>
    </div>
</template>

<script>

</script>

<style scoped>
    .searchBar {
        height: 40px;
        background-color: #ffffff;
        border-radius: 30px;
        width: 40vw;
        display: flex;
        gap: 15px;
    }

    .searchIcon {
        color: #202124;
        align-self: center;
        position: relative;
        scale: calc(0.8);
    }
    
    .magnifyingGlass {
        left: 10px;
    }

    .microphone {
        right: 10px;
    }

    .camera {
        right: 15px;
    }   

    .searchInput {
        width: 90%;
        height: 70%;
        align-self: center;
        caret-color: black;
        caret-shape: block;
        color: #202124;
        margin-left: 10px;
    }

    ::placeholder {
        color: #64686d;
    }

    input:focus {
        outline: none;
    }
</style>