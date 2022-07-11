<script setup>
import MyTemp from "./components/MyTemp.vue";

// let arrNEw = [1, 2, 3, 4, 5]
let arrNEW = {
	1: "first",
	2: "second",
	3: "third",
	4: "fortyn",
	5: "fiftyn",

}
</script>

<template>
	{{ arrNEw }}

	<div class="predoK">
		<div class="blockForTest" v-for="(item, idx) in arrNEW" :key="idx">
			<MyTemp> {{ item }}</MyTemp>
		</div>


	</div>
</template>

<style lang="css">
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}

body {
	background: rgb(149, 156, 172);
	font-size: 20px;
}

.predoK {
	display: flex;
	padding: 0 15px;
	margin: 0 -10px;
	overflow: hidden;
}

.blockForTest {
	/* width: 150px; */
	height: 150px;
	border: 1px solid black;
	flex: 1 1 auto;
	margin: 0 10px;
}
</style>
