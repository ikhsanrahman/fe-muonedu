<template>
	<div>
		<h1>Harga</h1>
		<div class="columns">
			<div class="column" style="text-align: center" v-for='content in data' :key="content.id">
				<div class="card">
					<div class="card-content">
						<h2>{{content.title}}</h2>
						<hr>
						<h2 style="color:blue;"> <strong>Rp </strong>{{content.discount}}</h2>
						<h5> <b>Rp</b>{{content.price}}</h5>
						<hr>
						<div class="content">
							<h4>{{content.desc_1}}</h4>
							<hr>
							<h4>{{content.desc_2}}</h4>
							<hr>
							<h4>{{content.desc_3}}</h4>
							<hr>
							<h4>{{content.desc_4}}</h4>
						</div>
					</div>
					<b-button type="info" style='margin:0 0 20px 0;'> <a :href="content.link" title="">Daftar Sekarang</a></b-button>
				</div>   
			</div>
		</div>
		<hr>
		<foot/>
	</div>
</template>

<script>
	import Foot from '@/components/Homepage/footer.vue'
	export default {
		name: 'Price',
		components: {
			Foot
		},
		data () {
			return {
				data: [
					{
						title: 'Batch 1: Python Basic',
						price: '1.500.000',
						discount: '700.000',
						desc_1: 'Durasi selama 6 minggu',
						desc_2: 'Dilakukan secara full onsite',
						desc_3: 'Dibimbing oleh praktisi Python, Machine Learning dan Computer Vision Expert',
						desc_4: 'Materi level beginner',
						link: 'https://forms.gle/nRWpEdXzu9MdH8f69'
					},
					{
						title: 'Batch 1: Python Intermediate',
						price: '2.000.000',
						discount: '800.000',
						desc_1: 'Durasi selama 6 Minggu',
						desc_2: 'Dilakukan secara full onsite',
						desc_3: 'Dibimbing oleh praktisi Python, Machine Learning dan Computer Vision Expert',
						desc_4: 'Materi level Intermediate',
						link: 'https://forms.gle/8AaNS2fkhtWLyxT66'
					},
					{
						title: 'Batch 1: Python Advanced',
						price: '3.000.000',
						discount: '1.000.000',
						desc_1: 'Durasi selama 7 minggu',
						desc_2: 'Dilakukan secara full onsite',
						desc_3: 'Dibimbing oleh praktisi Python, Machine Learning dan Computer Vision Expert',
						desc_4: 'Materi level Advanced',
						link: 'https://forms.gle/X3FCGnvjoWKjEbMaA'
					}
				]
			}
		}
	}
</script>

<style scoped>
	h1 {
		text-align: center;
		font-size: 50px;
		font-weight: 400;
	}
	.columns {
		margin: 20px 10% 20px 10%;
	}
	.content {
		font-size: 14px;

	}
	.card-content h2 {
		font-size:30px;
	}
	.card-content h5 {
		text-decoration: line-through;
		padding-left: 20%;
	}
	
</style>