<script>


</script>
<div class="background">
    
    <div class="projects">
        My <br>Projects.
    </div>
    <div class="spacer">
        <a href=/projects>Take a Peek</a> 
    </div>
</div>

<style>

.background {
    background-image: url(../img/background.png);
    min-height: 400px;
    background-size: cover;
}
.background {
    display: grid;
    grid-template-columns:  50%, 50%;
}
.projects{
    margin-top: 0em;
    grid-column-start: 2;
    font-size: 4rem;
    text-align: center;
}
.spacer {
   font-size: 2em;
   grid-column-start: 2;
   text-align: center;
}
.spacer a {
    margin-top: 5rem;
    font-size: 1.4rem;
    text-underline-offset: .6rem;
    transition: .3s ease-in-out;
    color: var(--black);
    
}
.spacer a:hover {
    color: var(--white)
}
</style>