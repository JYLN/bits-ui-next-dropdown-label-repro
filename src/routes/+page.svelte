<script lang="ts">
	import { DropdownMenu } from 'bits-ui';
</script>

<main class="grid min-h-screen place-content-center">
	<DropdownMenu.Root>
		<DropdownMenu.Trigger
			class="inline-flex items-center justify-center rounded-md border-2 px-3 py-2"
		>
			Open
		</DropdownMenu.Trigger>
		<DropdownMenu.Content sideOffset={4} class="min-w-[8rem] rounded-md border p-1 shadow-md">
			<DropdownMenu.Group>
				<!-- <DropdownMenu.Label></DropdownMenu.Label> -->
				<!-- ERRORS OUT:
          Property 'Label' does not exist on type
          'typeof import("../node_modules/bits-ui/dist/bits/dropdown-menu/exports")'.ts(2339)
        -->
				<DropdownMenu.Item>Some item</DropdownMenu.Item>
			</DropdownMenu.Group>
		</DropdownMenu.Content>
	</DropdownMenu.Root>
</main>
