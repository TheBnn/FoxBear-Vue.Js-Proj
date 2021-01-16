<template>
	<div class="header">
		<div class="container">
			<div class="header_menu">
				<nav class="menu">
					<div class="menu_item">
						<a href="#">Услуги</a>
					</div>
					<div class="menu_item">
						<a href="#">Меню</a>
					</div>
					<div class="menu_item menu_item__logo">
						<img class="logo" src="@/assets/logo.png" />
						<!--srcset="@/assets/logo@2x.png"-->
					</div>
					<div class="menu_item">
						<a href="#">Акции</a>
					</div>
					<div class="menu_item">
						<a href="#">Контакты</a>
					</div>
				</nav>
			</div>
			<div class="header_subInfo ">
				<div class="subInfo_elem">
					<div class="subInfo_fav">X</div>
					<div class="subInfo_info">
						Пн-сб 9:00-20:00 <br>
						Вс 9:00-18:00
					</div>
				</div>
				<div class="subInfo_elem">
					<div class="subInfo_fav">X</div>
					<div class="subInfo_info">
						+7 (925) 927 68 13 <br>
						+7 (916) 230 35 15
					</div>
				</div>
				<div class="subInfo_elem">
					<div class="subInfo_fav">X</div>
					<div class="subInfo_info">
						foxboar@mail.ru
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'headMenu',
		props: {

		}
	}
</script>

<style>
	.header {
		display: flex;
		background: #091A22;
	}

	.header .header_menu {
		display: flex;
		width: 100%;
		padding: 39px 0 46px;
	}

	.header .header_menu .menu {
		display: flex;
		flex-direction: row;
		justify-content: space-evenly;
		width: 100%;
	}

	.header .header_menu .menu .menu_item {
		display: flex;
		align-items: center;
	}

	.header .header_menu .menu .menu_item a {
		font-family: 'Gotham Pro';
		font-size: 26px;
		line-height: 35px;
		color: #FFFFFF;
		text-decoration: none;
		transition: .2s;
		position: relative;
	}

	.header .header_menu .menu .menu_item a:hover {
		transition: .2s;
	}

	.header .header_menu .menu .menu_item a:after {
		background: none repeat scroll 0 0 transparent;
		bottom: 0;
		content: "";
		display: block;
		height: 2px;
		left: 50%;
		position: absolute;
		background: #fff;
		transition: width 0.3s ease 0s, left 0.3s ease 0s;
		width: 0;
	}

	.header .header_menu .menu .menu_item a:hover:after {
		width: 100%;
		left: 0;
	}

	.header_subInfo {
		display: flex;
		width: 100%;
		font-family: 'Gotham Pro';
		justify-content: space-evenly;
		align-items: center;
		color: #D97943;
		font-size: 18px;
		padding-bottom: 23px;
		line-height: 25px;
	}

	.header_subInfo .subInfo_elem {
		display: flex;
		height: 100%;
	}

	.header_subInfo .subInfo_elem .subInfo_fav {
		padding-right: 44px;
	}
</style>