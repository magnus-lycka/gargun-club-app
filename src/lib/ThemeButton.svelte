<script>
    const darkTheme = 'luxury';
    const lightTheme = 'garden';

    const onload = el => {
        //waiting++
        el.addEventListener('load', () => {
            //waiting--
            //if (waiting === 0) {
                document.documentElement.setAttribute("data-theme", lightTheme);
            //}
        })
    }

    function nextTheme() {
        if (document.documentElement.getAttribute("data-theme") != lightTheme) {
            console.log('Go light');
            document.documentElement.setAttribute("data-theme", lightTheme);
        } else {
            document.documentElement.setAttribute("data-theme", darkTheme);
            console.log('Go dark');
        }
    }
</script>

<button class="btn btn-accent" on:click={nextTheme}>
    Light/Dark
</button> 
