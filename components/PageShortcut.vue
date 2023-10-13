<template>
    <div class="shortcut" v-if="title">
        <div class="circle">
            <div class="innerCircle" v-if="title">
                <span>{{ centerLetter }}</span>
            </div>
        </div>
        <p>{{ title }}</p>
    </div>
    <div class="shortcut" v-else>
        <div class="circle">
            <div class="innerCircle">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M12 4.5v15m7.5-7.5h-15" />
                </svg>
            </div>
        </div>
        <p>Add shortcut</p>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                centerLetter: String,
                innerColor: String,
            };
        },

        computed() {
            return {
                'innerCircle-bg-color': this.color ? this.color : "#aaaaaa",
            }
        },

        props: {
            title: String,
            address: String,
            color: String,
        },

        methods: {
            getCenterLetter() {
                const centerLetter = this.title ? this.title.charAt(0) : '#'; 
                return centerLetter;
            },
        },

        mounted()  {
            this.centerLetter = this.getCenterLetter();
        }
 
    }
    // const shortcutCard = defineProps({
    //     title: String,
    //     linkSource: String,
    //     color: String,
    // });

    

    // const centerLetter = computed(() => {
    //     return shortcutCard.title ? shortcutCard.title.charAt(0) : '#';
    // });

    // const innerColor = computed(() => {
    //     return shortcutCard.color ? shortcutCard.color : 'rgb(88, 88, 88)'; 
    // })

    // onMounted(() => {
    //     document.getElementById('innerColor').style.backgroundColor = innerColor;
    //     // if (shortcutCard.color) {
    //     //     console.log("if", shortcutCard.color, typeof(shortcutCard.color));
    //     //     document.getElementById('innerColor').style.backgroundColor = shortcutCard.color;
    //     // }
    // });

    // const innerColor = computed(() => {
    //     if (shortcutCard.color) {
    //         document.getElementById('innerCircle').style.backgroundColor = shortcutCard.color
    //     } else {
    //         document.getElementById('innerCircle').style.backgroundColor = '#505050'
    //     }
    // })

</script>
    
<style scoped>
    .circle {
        background-color: #202124;
        width: 50px;
        height: 50px;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .innerCircle {
        width: 25px;
        height: 25px;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: var(innerCircle-bg-color);
    }

    .shortcut {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 10px;
        font-size: 14px;
        cursor: pointer;
        padding: 15px;
        border-radius: 4px;
        width: 110px;
        height: 130px;
    }

    .shortcut:hover {
        background-color: #505050;
    }

</style>