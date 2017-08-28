<template>
	<section class="time-line">
		<time-line-item v-for="item in timeline" v-bind:key="item.id" v-bind:item="item">
		</time-line-item>
		<div class="sources">
			<a target="_blank" rel="noopener" href="https://www.sketchappsources.com/free-source/1137-material-design-resume-style-sketch-freebie-resouces.html">
				Design thanks to sketch resources
			</a>
		</div>
	</section>
</template>

<script>

import TimeLineItem from './TimeLineItem';

function data() {
	return {
		timeline: [
			{
				id: 1,
				companyName: 'FullFactory',
				duration: {
					number: ' - ',
					type: 'Present',
				},
				position: 'Full Stack Developer',
				jobs: ['Build web applications using VueJs 1/2',
					'Build json rest apis using NodeJs, HapiJs, Objection and other fun stuff.'],
			},
			{
				id: 2,
				companyName: 'Abakio S.A.C',
				duration: {
					number: '6',
					type: 'Years',
				},
				position: 'Lead Developer',
				jobs: ['Lead developer of the development section.',
					'Constant training of the developers in charge with talks, courses, workshops, etc.',
					'Create and update the initial structure of all the projects in the different technologies that the company work with.'],
			},
			{
				id: 3,
				companyName: 'Universidad Católica Sedes Sapientiae',
				duration: {
					number: '1',
					type: 'Year',
				},
				position: 'Developer',
				jobs: ['Migration of desktop applications from Fox Pro to .NET.',
					'Building web application who allows search job opportunities for the students of the university.'],
			},
			{
				id: 4,
				companyName: 'I.S.T El Buen Pastor',
				duration: {
					number: '6',
					type: 'Months',
				},
				position: 'Developer',
				jobs: ['Creation of desktop application that allows to evaluate the teachers of the institution.'],
			},
		],
	};
}

export default {
	name: 'resume-time-line',
	components: {
		TimeLineItem,
	},
	data,
};
</script>

<style lang="scss" scoped>
.sources {
	text-align: right;

	a {
		bottom: 2%;
		position: absolute;
		right: 2%;
	}
}

.time-line {
	display: flex;
	flex-direction: column;
	margin-top: 7%;
	padding-left: 7%;
	position: relative;
}
</style>

