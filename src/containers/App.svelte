<script>
    import { onMount } from 'svelte';
    import Main from '../widgets/Main.svelte';


    let data = {}
    const API = "https://api-pugstagram.herokuapp.com/?nickname=MiguelAngelMP&name=Miguel%20Angel"

    onMount(async () => {
        const response = await fetch(API);
        data = await response.json();
    })

</script>
<head>
    <meta charset="utf-8">
    <title>Icono en el navegador</title>
    <link type="image/png" sizes="16x16" rel="icon" href=".../icons8-películas-disney-16.png">
    <link rel="stylesheet" media="screen" href="https://fontlibrary.org//face/waltograph-disney" type="text/css"/>
</head>

<style>
    @import url('https://fontlibrary.org//face/waltograph-disney?family=disney:wght@300;400&display=swap');
    /* @import url('https://fonts.googleapis.com/css2?family=Lato:wght@300;400&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Lato:wght@300;400&family=Pacifico&display=swap'); */
    :global(body){
        background-color: var(--tertiary-background);
        /* background-image: url("../public/images/backgroundMoana5.jpeg");
        background-repeat: no-repeat;
        background-size:100%;  */
        color:var(--secondary-background);
        margin: 0;
        padding: 0;
        font-family: 'WaltographRegular';
        font-weight: normal;
        font-style: normal;
        text-align: center;
    }
    :global(h1,h2,h3){
        color:var(--secondary-background);
        font-family: 'WaltographRegular';
        font-weight: normal;
        font-style: normal;
        text-align: center;
    }
    :root{
        --primary-background: #c59b79;
	    --secondary-background: #FFFFFF;
	    --tertiary-background: #40b4fb;
    }
</style>
<Main>
</Main>