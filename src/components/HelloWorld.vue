<template>
	<div class="flex-container">
		<img :src="getImageURL" alt="alternate text" class="main-image" />
		<img
			src="/img/02.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('02.jpg')"
		/>
		<img
			src="/img/03.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('03.jpg')"
		/>
		<img
			src="/img/04.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('04.jpg')"
		/>
		<img
			src="/img/05.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('05.jpg')"
		/>
		<img
			src="/img/06.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('06.jpg')"
		/>
		<img
			src="/img/07.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('07.jpg')"
		/>
		<img
			src="/img/08.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('08.jpg')"
		/>
		<img
			src="/img/09.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('09.jpg')"
		/>
		<img
			src="/img/10.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('10.jpg')"
		/>
		<img
			src="/img/11.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('11.jpg')"
		/>
		<img
			src="/img/12.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('12.jpg')"
		/>
		<img
			src="/img/13.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('13.jpg')"
		/>
		<img
			src="/img/130_GSM.jpg"
			alt=""
			class="thumbnail"
			@click="setmainimage('130_GSM.jpg')"
		/>
	</div>
</template>

<script>
	export default {
		name: 'HelloWorld',
		props: {},
		components: {},

		data() {
			return {
				Image_URL: '02.jpg',
			};
		},
		computed: {
			getImageURL() {
				return '/img/' + this.Image_URL;
			},
		},

		methods: {
			setmainimage(pic) {
				this.Image_URL = pic;
			},
		},
	};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	.grid-container {
		display: flex;
		flex-direction: column;
	}
	.main-image {
		height: 80vh;
		width: 100%;
		display: block;
		margin: 0 auto;
	}
	/* .main-container {
		display: flex;
		margin-top: 0;
		margin-left: 0.1%;
		margin-right: 0.1%;
	} */
	.thumbnail {
		position: relative;
		height: 10%;
		width: 10%;
		padding-right: 10px;
		margin-top: 1%;
		margin-left: 10px;
		justify-content: space-evenly;
		flex-direction: row;
	}
	.thumbnail:hover {
		cursor: pointer;
	}
</style>
