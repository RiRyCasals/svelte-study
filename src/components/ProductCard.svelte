<script lang="ts">
    export let productTitle: string;
    export let productUrl: string;
    export let productLink: string = "→ GitHub";
    export let cardColor: string = "blue";
    export let colorIntensity:string = "200";
    export let colorIntensityForHover:string = "100";
</script>

<div class="mt-4 py-4 bg-{cardColor}-{colorIntensity} hover:bg-{cardColor}-{colorIntensityForHover}">
    <h1>{ productTitle }</h1>
    <a href="{ productUrl }" target="_blank">{ productLink }</a>
</div>
