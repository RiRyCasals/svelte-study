<script>
    import ProductCard from "../components/ProductCard.svelte";

    const dataList = [
        {
            productTitle: "arduioで作る電子ピアノ",
            productUrl: "https://github.com/RiRyCasals/arduino",
            cardColor: "indigo",
        },
        {
            productTitle: "笑い男アプリ",
            productUrl: "https://github.com/RiRyCasals/python-laughingman",
            cardColor: "blue",
        },
        {
            productTitle: "Nimのクロスコンパイル環境",
            productUrl: "https://github.com/RiRyCasals/nim-cross-compile-env",
            cardColor: "yellow",
        },
    ]
</script>

<title>Home</title>

<div class="text-center mx-20">
    <h1 class="text-3xl lg:text-6xl my-2">RiRy Casals</h1>
    <div class="my-2">
        <p>IT系の専門学校の学生です．</p>
        <p>Python でできることなら何でもやってます．</p>
        <p>ここ最近は Nim という言語に浮気しています．</p>
    </div>
    {#each dataList as data}
        <ProductCard
            productTitle={data.productTitle}
            productUrl={data.productUrl}
            cardColor={data.cardColor}
        />
    {/each}
</div>
