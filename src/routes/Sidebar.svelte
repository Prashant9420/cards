<script>
    
    const handleClick = (ind) =>()=>{
        val=ind
        open=!open
    }
    export let open = false
    export let val;

</script>

<aside class="absolute w-full h-full bg-gray-200 border-r-2 shadow-lg" style="border:2px solid green;width:20%" class:open>
	<nav class="p-12 text-xl">
		<div style=";display:flex;flex-direction:column;height:100vh;align-items:end;justify-content:space-between">
            <div role="button" on:click={handleClick(0)} style="border:20px solid grey;background-color:beige;width:100%;height:24%;border-radius:20px;text-align:center">
                <h2>HONDA</h2>
                <p style="font-size:small">Honda Motor Co., Ltd. is a Japanese public multinational conglomerate manufacturer of automobiles, motorcycles, and power equipment, headquartered in Minato, Tokyo, Japan.</p>
            </div>
            <div role="button" on:click={handleClick(1)} style="border:20px solid grey;background-color:beige;width:100%;height:24%;border-radius:20px;text-align:center">
                <h2>FORD</h2>
                <p style="font-size:small">Ford Motor Company is an American multinational automobile manufacturer headquartered in Dearborn, Michigan, United States.</p>
            </div>
            <div role="button" on:click={handleClick(2)} style="border:20px solid grey;background-color:beige;width:100%;height:24%;border-radius:20px;text-align:center">
                <h2>BMW</h2>
                <p style="font-size:small">Bayerische Motoren Werke AG, abbreviated as BMW, is a German multinational manufacturer of luxury vehicles and motorcycles headquartered in Munich, Bavaria, Germany.</p>
            </div>
            <div role="button" on:click={handleClick(3)} style="border:20px solid grey;background-color:beige;width:100%;height:24%;border-radius:20px;text-align:center">
                <h2>NISSAN</h2>
                <p style="font-size:small">Nissan Motor Co. Ltd., often shortened to Nissan, is a Japanese multinational automobile manufacturer headquartered in Nishi-ku, Yokohama, Japan.</p>
            </div>
        </div>
		
	</nav>
</aside>

<style>
	aside {
		left: 100%;
		transition: left 0.3s ease-in-out
	}
	
	.open {
		left: 0
	}
</style>