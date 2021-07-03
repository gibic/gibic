<section>
    <div class="card">
        <figure>
            <img src="/visual.svg" alt="index media">
        </figure>
        <div>
            <h3><a href="https://imi.remotivi.or.id/" target="_blank">Indeks Media Inklusif</a></h3>
            <p>HTML, CSS, JavaScript</p>
        </div>
    </div>
    <div class="card">
        <figure>
            <img src="/screenshot.png" alt="lab">
        </figure>
        <div>
            <h3><a href="https://altrlab.com/" target="_blank">ALTR</a></h3>
            <p>HTML, CSS, JavaScript</p>
        </div>
    </div>
    <div class="card">
        <figure>
            <img src="/screenshot2.png" alt="bersiasat">
        </figure>
        <div>
            <h3><a href="https://bersiasat.id/" target="_blank">Bersiasat</a></h3>
            <p>Wordpress Theme Development</p>
        </div>
    </div>
    <div class="card">
        <figure>
            <img src="/screenshot3.png" alt="spektakel">
        </figure>
        <div>
            <h3><a href="https://spektakel.id/" target="_blank">Spektakel</a></h3>
            <p>Laravel, HTML, CSS, JavaScript</p>
        </div>
    </div>
</section>

<style>
    .card {
        width: 80%;
        display: grid;
        grid-gap: 1rem;
        grid-template-columns: 1fr 3fr;
        margin: 1rem 0;
        border-radius: .5rem;
        border: var(--border);
        overflow: hidden;
        height: 100px;
        background-color: var(--dark);
    }
    figure {
        background-color: var(--white);
        height: 100px;
    }
    .card img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
    .card p {
        color: rgba(255, 255, 255, 0.445);
        margin: 0;
    }
    h3 {
        margin-bottom: 0;
    }
</style>