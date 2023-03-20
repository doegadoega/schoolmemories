<script setup lang="ts">

const articles = ref<{ id: number, title: string }[]>([]);

articles.value = [{
  id: 1,
  title: "Nuxt3入門",
}, {
  id: 2,
  title: "Jest再入門",
}];
</script>

<template>
  <div>
	<header>
		<div class="flex">
			<label id="effect_title">
				<h3>School Memories</h3>
			</label>
		</div>
		<div class="right_">
			<h1>メモリアル映像制作</h1>
		</div>		
	</header>
    <div class="container">
		<div>
			<img src="@/assets/stock_474365622.jpg" 
				alt="Icon"
				class="mr-3" />

		</div>
    </div>
    <footer>
      © 2022 mamezou-tech
    </footer>
  </div>
</template>

<style scoped>
header {
  padding: 1rem;
}
footer {
  margin-top: 2rem;
  background-color: #8080ee;
  padding: 1rem;
}
.container {
  margin: 2rem;
}

.flex{
    display: flex;
    justify-content: space-between;
}
.flex>p{
    width: 49%;
}

.right_ {
	text-align: right;
	margin: 0 auto;
	font-weight: bold;
	padding-top: 10px;
	padding-bottom: 5px;
	font-size: small;
}
</style>

