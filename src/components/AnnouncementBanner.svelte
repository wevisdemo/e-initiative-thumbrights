<script lang="ts">
	let isVisible = true;

	function close() {
		isVisible = false;
	}
</script>

{#if isVisible}
	<div class="fixed inset-x-0 top-0 z-[60] bg-primary text-white shadow-lg">
		<div
			class="mx-auto flex w-full max-w-screen-lg items-start justify-between gap-2 px-4 py-2 md:gap-4 md:py-3"
		>
			<div class="flex flex-1 flex-col items-start gap-2 md:flex-row md:gap-3">
				<span
					class="flex-shrink-0 rounded-full bg-white/20 px-2 py-0.5 text-xs font-bold"
				>
					ประกาศ
				</span>
				<p class="text-xs leading-snug">
					เนื่องจากร่าง พ.ร.บ. เดิมที่เผยแพร่ในเว็บไซต์ มีปัญหาทางเทคนิคการเขียน
					ทำให้ผลทางกฎหมายออกมาอาจถูกเข้าใจไปได้ว่า เป็นร่างที่มุ่งจะยกเลิกมาตรา
					112 และมาตราอื่น ๆ ซึ่งไม่ตรงตามสิ่งที่เครือข่ายฯ สื่อสารรณรงค์
					เราจึงปรับแก้การเขียนร่างให้ตรงตามเจตนารมณ์และหลักการที่มุ่งเสนอยกเลิกผลพวงคณะรัฐประหาร
					6 ตุลาฯ โดยเราได้ปรับแก้ร่างกฎหมายในวันที่ 16 ก.ค. 2569
					หากประชาชนคนใดที่ลงชื่อไปแล้ว
					และต้องการถอนการลงชื่อของตนเนื่องจากร่างที่เปลี่ยนแปลงไป
					สามารถติดต่อได้ทาง <a
						href="https://www.facebook.com/2519October6"
						class="underline"
						target="_blank">Facebook: เครือข่ายจัดงานรำลึก 6 ตุลาฯ</a
					>
				</p>
			</div>
			<button
				on:click={close}
				class="btn btn-ghost btn-xs flex-shrink-0 text-white hover:bg-white/20"
				aria-label="Close banner"
			>
				✕
			</button>
		</div>
	</div>
{/if}
