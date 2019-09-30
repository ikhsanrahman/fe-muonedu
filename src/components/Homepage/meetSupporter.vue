<template>
	<div class="container">
		<div class="title">
			<h1>Our Team</h1>
		</div>
		<div class="columns" style="margin:0 10% 0 10%">
			<div class="column" v-for="content in data" :key="content.id">
				<div class="columns" style="margin: 0 40px 0 40px">
					<div class="column">
						<img :src="content.url" style="width:60%;height:80%; padding:0;" alt="Placeholder Image">
					</div>
					<div class="column" style="padding:5% 0 0 0">
						{{content.description}}
					</div>
				</div>
			</div>
		</div>
	</div>	
	
</template>

<script>
	export default {
		data () {
			return {
				data: [
					{
						url: require('../../assets/image/vicky.jpeg'),
						description: 'Vicky adalah salah satu founder Muon yang pernah memiliki Keahlian Python dan sudah berpengalaman menjadi pembicara di sejumlah pelatihan dan juga seminar.'
					},
					{
						url: require('../../assets/image/ikhsan.jpeg'),
						description: 'Ikhsan adalah salah satu founder Muon yang pernah memiliki Keahlian Python dan sudah berpengalaman menjadi pembicara di sejumlah pelatihan dan juga seminar.'
					}
				]
			}
		}
	}
</script>

<style scoped>
	.container {
		padding: 40px 10px 10px 10px;
		text-align: center;
		border-bottom: 1px solid black;
	}
	.title h1 {
		font-size: 50px;
	}
</style>