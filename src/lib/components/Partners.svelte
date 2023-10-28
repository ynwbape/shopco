<script>
    import zara from "../../assets/img/brands/zara.png"
    import versace from "../../assets/img/brands/versace.png"
    import prada from "../../assets/img/brands/prada.png"
    import gucci from "../../assets/img/brands/gucci.png"
    import cklein from "../../assets/img/brands/calvinklein.png"

    const brands = [zara, versace, prada, gucci, cklein]
</script>

<div class="partners">
    {#each brands as brand }
        <div class="brand">
            <img src={brand} alt="Marques Partenaires">
        </div>
    {/each}
</div>

<style>
    .partners {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 141px;
        height: 162px;
        background-color: var(--black);
        animation: infinite linear 2s reverse both;
    }

    .brand img {
        height: 44px;
    }

    @keyframes loop {
        from {
            transform: rotateY(0deg);
        }  
        to {
            transform: rotateY(360deg);
        }
    }
</style>