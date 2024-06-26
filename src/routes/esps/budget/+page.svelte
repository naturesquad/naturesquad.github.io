<script>
	import pieChart from '$lib/budgetPieChart.png';
	import studentFTEBarChart from '$lib/studentFTEBarChart.png';
</script>

<svelte:head>
	<title>ESPS - Budget</title>
	<meta name="description" content="Questions and answer about the Evergreen School District budget">
</svelte:head>

<p>
	We're here to answer your questions about the district's budget. Below are some frequently asked questions about the
	budget, and the district's financial situation. All of this information comes from the district's
	<a href="https://sites.google.com/evergreenps.org/budget-fiscal-services/budget">budget page</a>.
</p>

<details>
	<summary>How is the district funded?</summary>
	<p>
		The graph below shows the district’s major revenue sources for the 2022-23 school year. Over half of the district’s
		revenue comes from the state government. Much of the state revenue is for general use, but some of it is designated
		for special purposes, like special education and transportation. The district also receives money from the federal
		government that is designated for special purposes. The main local sources of revenue are the Operations Levy and
		the Technology Levy. The last revenue source is Federal <abbr title="Elementary and Secondary School Emergency Relief">ESSER</abbr> funds that were designed to provide COVID relief, but
		are expiring with the 2023-24 school year. ESSER funds will not be available for 2024-25.
	</p>

	<figure>
		<figcaption>2022-23 General Fund Revenue - $409,785,461</figcaption>
		<img alt="budget pie char" src={pieChart}>
	</figure>
</details>

<details>
	<summary>What is causing the budget shortfall?</summary>
	<p>The district is facing a $16 to $20 million budget shortfall for the 2024-25 school year.
		The biggest factor impacting the budget is enrollment. Enrollment in public education is in decline all over the
		state. Some of the district’s funding is allocated on a per student basis. With fewer students enrolled, the
		district receives less money. Another factor is that emergency COVID relief
		(<abbr title="Elementary and Secondary School Emergency Relief">ESSER</abbr>)
		funds are expiring in 2024. ESSER funds accounted for 5% of the district’s revenue in 2022-23.

	<p>Inflation is another major factor, with rising costs for supplies, electricity, and fuel for school buses all
		making a dent in the budget. Another factor is an underfunded special education mandate from the state. Our district
		is required to provide a certain level of support for students with special needs, but doesn’t receive enough
		funding from the state to cover the cost for that level of support.
	</p>
</details>

<details>
	<summary>How is enrollment changing over time?</summary>
	<p>Enrollment in our district has been on a steady decline for the past eight years, with a particularly sharp drop
		immediately following the 2020 pandemic. Middle school and high school enrollment levels have remained fairly
		consistent, with the most decline being seen at the elementary level. As elementary students get older, we will see
		a wave in enrollment decline go through our middle and high schools. Enrollment is predicted to continue to decrease
		at least through 2027.
		<img src={studentFTEBarChart} alt="student FTE bar chart">
</details>
<p class="last">Please visit the district’s
	<a href="https://sites.google.com/evergreenps.org/budget-fiscal-services/budget">budget page</a>
	for more information.
</p>

<style>
    .last {
        padding-block: 2rem;
    }


    summary {
        font-weight: bold;
        font-size: x-large;
        line-height: 3rem;
    }

    img {
        padding-top: 2rem;
    }

    details summary::after {
        height: 3rem;
    }
</style>