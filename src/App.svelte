<script lang="ts">
import { onMount } from 'svelte';
import { H5P } from 'h5p-standalone'; // ES6
// const { H5P } = require('h5p-standalone'); AMD
// const { H5P } = 'H5PStandalone'; // object destructuring
let el: HTMLElement;
let options: any;
onMount(() => {
    el = document.getElementById('h5p-container');
    options = {
        h5pJsonPath: '/deneme-597-1504109/',
        frameJs: '/frame.bundle.js',
        frameCss: '/styles/h5p.css',
    };

    new H5P(el, options);
});


</script>


<div id='h5p-container'></div>