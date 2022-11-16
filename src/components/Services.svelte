<script>
    const carousel = [
        '../img'
    ]
</script>
                                                                                       
<section class="servicesection" href=#services id="services">
    <div class="services">
        <div class="services1">
            <h3>Fit your needs</h3>
            <h1>My <br> Services.</h1>
        </div>
        <div class="services2"></div>
    </div>
    <div class="carousel"></div>
    <div class="background"></div>
</section>
<style>
.servicesection {
    display: flex;
}
.services {
    background: var(--lorange);
    width: 45%;
}
.services1 h1 {
    font-size: 4rem;
    offset: left 5px;
}
/* .services h2 {

} */
.carousel {
    background: url('../img/devpic.svg');
    background-size: contain;
    background-repeat: no-repeat;
    width: 55%;
}
</style>