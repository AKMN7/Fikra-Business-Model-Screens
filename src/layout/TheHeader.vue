<template>
	<header class="header">
		<nav>
			<div class="logo">
				<img src="../assets/img/logo.svg" class="h-16" />
			</div>
			<input type="checkbox" id="menu-toggle" />
			<label for="menu-toggle" class="menu-icon">&#9776;</label>
			<ul class="menu">
				<li @click="closeMenu">
					<router-link v-if="!isLoggedIn" to="/signin" class="px-5 py-2 text-white rounded-full loginBtn">
						تسجيل الدخول
					</router-link>
				</li>
				<li @click="closeMenu">
					<router-link v-if="isLoggedIn" to="/profile" class="profileImg">
						<img src="../assets/img/user.svg" class="h-[50px]" alt="User" />
					</router-link>
				</li>
				<li @click="closeMenu">
					<router-link to="/prize">جائزة ابتكر </router-link>
				</li>
				<li @click="closeMenu">
					<router-link to="/events">الفعاليات</router-link>
				</li>
				<li @click="closeMenu">
					<router-link to="/library">مكتبة الابتكار</router-link>
				</li>
				<li><Dropdown /></li>
				<li @click="closeMenu">
					<router-link to="/">الرئيسية</router-link>
				</li>
			</ul>
		</nav>
	</header>
</template>

<script setup>
	import Dropdown from "../components/Dropdown.vue";
	import { ref } from "vue";
	const isLoggedIn = ref(true);

	const closeMenu = () => {
		document.getElementById("menu-toggle").checked = false;
	};
</script>

<style scoped>
	.header {
		z-index: 30;
		display: flex;
		align-items: center;
		justify-content: center;
	}

	nav {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 20px 30px;
		width: 90%;
	}

	.menu {
		display: flex;
		flex-direction: row-reverse;
		justify-content: center;
		align-items: center;
	}

	.menu a:not(.loginBtn, .profileImg) {
		display: block;
		padding: 20px 0px;
		font-size: 17px;
		font-weight: 500;
		color: #1e1e1e;
		margin-left: 50px;
		white-space: nowrap;
	}

	.menu-icon {
		display: none;
	}

	#menu-toggle {
		display: none;
	}

	#menu-toggle:checked ~ .menu {
		transform: scale(1, 1);
	}

	.loginBtn {
		background: linear-gradient(90deg, #007598 21.23%, #019390 75.88%);
		color: #f4fafb !important;
		border-radius: 20px;
		padding: 12px 20px;
		min-width: 156px !important;
		white-space: nowrap;
	}

	@media only screen and (max-width: 950px) {
		.header {
			justify-content: space-between;
		}

		nav {
			padding: 8px;
			width: 100%;
		}

		.menu {
			flex-direction: column-reverse;
			background-color: #fff;
			align-items: start;
			position: absolute;
			padding: 15px 30px;
			top: 80px;
			left: 0;
			width: 100%;
			z-index: 100;
			transform: scale(1, 0);
			transform-origin: top;
			transition: transform 0.3s ease-in-out;
			box-shadow: rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px;
		}

		.menu a {
			margin-left: 12px;
		}

		.menu li {
			margin-bottom: 10px;
			min-width: 30%;
		}

		.menu li:first-child {
			margin-top: 20px;
		}

		.menu-icon {
			display: flex;
			align-items: center;
			justify-content: center;
			color: #1e1e1e;
			font-size: 28px;
			cursor: pointer;
			margin: 0 0 -10px 10px;
		}

		.loginBtn {
			margin-top: 20px !important;
		}
	}
</style>
