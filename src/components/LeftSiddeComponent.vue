<script setup>

</script>

<template>
  <div class="left-side">
    <h1 class="title gradient">ПУТЕШЕСТВИЕ <br /><span class="text"> на красную планету</span>
    </h1>
    <button class="btn">Начать путешествие</button>
  </div>
</template>

<style scoped lang="scss">

// ====LEFT SIDE START=====
.gradient {
    width: fit-content;
    color: transparent;
	-webkit-background-clip: text;
    background-clip: text;
	background-image: linear-gradient(120deg, white, rgb(215, 54, 0)); 
}

.title {
    font-size: 3rem;
    text-transform: uppercase;
    margin: 0 0 90px;
    font-weight: 800;
    font-family: 'Roboto', sans-serif;
}

.text {
    font-size: 1rem;
}

.btn {
    font-size: .8rem;
    background-color: rgba(0, 0, 0, 0); /* Прозрачный фон */
    color: white;
    padding: 10px 25px;

    /* Делаем градиент бордеру */
    border: 1px solid transparent;
    border-image: linear-gradient(to left bottom,#0015ff 10%,  transparent 30%, transparent 70%, #0015ff 90%);
    border-image-slice: 1;

    transition: .6s;

    &:hover {
    border-image: linear-gradient(to left top,#0015ff 10%,  transparent 30%, transparent 70%, #0015ff 90%);
    border-image-slice: 1;
    
    transition: .6s;

    }
}
// ====LEFT SIDE END=====

@media (max-width: 726px) {
    
    .title {
        margin: 20px 0 25px;
        text-align: center;
        font-size: 2.8rem;
        line-height: .9;
    }
    .gradient {
        background-image: linear-gradient(240deg, white, rgb(215, 54, 0)); 
    }
    .btn {
        margin-left: 100px;
        background-color: rgba(0, 0, 0, .3);
    }
}

@media (max-width: 400px) {
    .title {
        font-size: 2.5rem;
    }
}

</style>
