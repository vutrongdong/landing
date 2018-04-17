<template>
	<div id="menu-top" >
		<div class="menu-top container">
			<img width="100px" class="nav navbar-left nav" src="./images/logobeeketing.png" alt="beeketing">
			<label for="toggle">&#9776;</label>
			<input type="checkbox" id="toggle">
			<ul class="nav navbar-nav navbar-right" style="margin-right:10px;">
				<li v-for="element in menu_top">
					<a v-bind:href='element.url' :class="element.class">{{element.name}}</a>
				</li>
			</ul>
		</div>
	</div>
</template>

<script>
	export default {
		data () {
			return {
				menu_top:[
				{name:'Features',url:'#'},
				{name:'Pricing',url:'#'},
				{name:'About',url:'#'},
				{name:'Login',url:'#'},
				{name:'Get Starts',url:'#',class:"btn btn-info"}
				]
			}
		}
	}
</script>

<style lang="scss">
	#menu-top{
		background: #fff;
		@media only screen and (min-width: 769px){
		img{
			margin:16px 0px 0px 15px;
		}
		label,input{
			display:none;
		}
		ul{
			margin: 20px 0px;
		}
		a{
			background: none;
			padding-top:10px;
			padding-bottom: 10px;
			font-size: 18px;
			color: #003d7c;
			&:hover{
				color: #0088ff;
			}
		}
		.btn{
			padding-top:10px;
			padding-bottom: 10px;
			background: #0088ff;
			color: #fff;
			&:hover{
				background: #2499ff;
				color: #fff;
			}
		}
	}
	@media only screen and (max-width: 768px){
	img{
		vertical-align: middle;
		margin: 7px 0px 0px 15px;
		float: left;
	}
	input{
		display: none;
	}
	label{
		display:block;
		float:right;
		color: black;
		margin: 22px 15px 0px 0px;
		font-size:20px;
	}
	input:checked +ul{
		display:block;
		margin: 10px 0px;
	}
	ul{
		clear: both;
		display:none;
		li{
			text-align:center;
			border:1px solid #fff;
			width:100%;
			background:#73D216;
			a{
				background: none;
				padding: 10px;
				font-size: 18px;
				color: #fff;
			}
			.btn{
				background: none;
			}
		}
	}
}

}

</style>