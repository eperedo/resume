<template>
	<div id="app">
		<resume-header></resume-header>
		<resume-time-line></resume-time-line>
		<resume-profile></resume-profile>
		<p class="float-experience">Experience*</p>
	</div>
</template>

<script>
import ResumeHeader from './components/Header';
import ResumeTimeLine from './components/TimeLine';
import ResumeProfile from './components/Profile';

export default {
	name: 'app',
	components: {
		ResumeHeader,
		ResumeProfile,
		ResumeTimeLine,
	},
};
</script>

<style lang="scss">
* {
	font-family: 'Roboto-Medium', sans-serif;
	font-size: 16px;
}

#app {
	display: grid;
	grid-template-columns: 1.8fr 1fr;
}

.float-experience {
	color: map-get($colors, blue);
	font-family: map-get($fonts, black);
	font-size: 216px;
	left: -36%;
	letter-spacing: -1.01px;
	margin: 0;
	opacity: 0.1;
	position: absolute;
	top: 86%;
	transform: rotate(-270deg);
}

.float-skills {
	bottom: -166%;
	color: map-get($colors, blue);
	font-family: map-get($fonts, black);
	font-size: 216px;
	letter-spacing: -1.01px;
	margin: 0;
	opacity: 0.1;
	position: absolute;
	right: -17%;
	transform: rotate(-90deg);
}

@media (max-width: 990px) {
	#app {
		grid-template-columns: 1fr;
	}
	.float-experience,
	.float-skills {
		display: none;
	}
}
</style>
