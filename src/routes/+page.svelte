<script lang="ts">
	let items = [
		{
			url: 'https://election.matichon.co.th/results',
			name: 'Matichon',
			imgUrl: 'https://election.matichon.co.th/assets/logo/share.jpeg'
		},
		{
			url: 'https://election2566.thestandard.co',
			name: 'THE STANDARD',
			imgUrl: 'https://election2566.thestandard.co/images/cover.png'
		},
		{
			url: 'https://thvote66.thematter.co',
			name: 'The MATTER',
			imgUrl: 'https://thvote66.thematter.co/og.png'
		},
		{
			url: 'https://election66.thaipbs.or.th/result',
			name: 'Thai PBS',
			imgUrl: 'https://election66-asset.thaipbs.or.th/cover-images/main.png'
		},
		{
			url: 'https://www.thairath.co.th/election66',
			name: 'THAIRATH',
			imgUrl: 'https://static2.thairath.co.th/__media/election2023/S5529629.jpg'
		},
		{
			url: 'https://www.ectreport.com/overview',
			name: 'ECT',
			imgUrl: 'https://www.ectreport.com/logos/ect-logo.png'
		},
		{
			url: 'https://vote66.workpointtoday.com',
			name: 'workpointTODAY',
			imgUrl: 'https://election66.tillitsdone.com/election2023_cover.png'
		},
		{
			url: 'https://wecheck66th.com',
			name: 'wecheck',
			imgUrl: 'https://wecheck66th.com/wecheck66.png'
		},
		{
			url: 'https://vote66.voicetv.co.th',
			name: 'Voice TV',
			imgUrl: 'https://vote66.voicetv.co.th/share.jpg'
		},
		{
			url: 'https://election66.nationtv.tv/report/party/?zone_id=0-0-0',
			name: 'NATION TV',
			imgUrl: 'https://election66.nationtv.tv/OG_elect_result.png'
		},
		{
			url: 'https://www.vote62.com/',
			name: 'VOTE 62',
			imgUrl: 'https://vote62.com/img/og/og-image.png?t=1'
		}
	];
</script>

<div class="container mx-auto">
	<h1 class="text-3xl text-gray-800 text-center font-semibold my-8 uppercase">
		รวมเว็บไซต์รายงานผลคะแนนเลือกตั้ง 2566
	</h1>

	<div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-5 gap-4">
		{#each items as item}
			<div
				class="relative rounded-xl overflow-hidden bg-gray-100 outline outline-gray-200 shadow-sm group transition transform"
			>
				<a href={item.url} target="_blank">
					<img src={item.imgUrl} alt={item.name} class="aspect-video w-full" loading="lazy" />
					<div
						class="
          absolute -bottom-[36px] left-0 right-0
          text-white text-base font-semibold
          px-2.5 py-1.5
          bg-black/20 backdrop-blur-sm
          rounded-t-lg
          group-hover group-hover:bottom-0 group-hover:transition-all
        "
					>
						{item.name}
					</div>
				</a>
			</div>
		{/each}
	</div>
</div>
