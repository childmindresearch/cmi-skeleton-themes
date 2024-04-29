<script lang="ts">
	import { ListBox, ListBoxItem } from '@skeletonlabs/skeleton';

	let valueSingle: string = 'books';
	let valueMultiple: string[] = ['books', 'movies'];
</script>

Single selection:
<ListBox>
	<ListBoxItem bind:group={valueSingle} name="medium" value="books">Books</ListBoxItem>
	<ListBoxItem bind:group={valueSingle} name="medium" value="movies">Movies</ListBoxItem>
	<ListBoxItem bind:group={valueSingle} name="medium" value="tv">TV</ListBoxItem>
</ListBox>

<br />
Multiple Selection:
<ListBox multiple>
	<ListBoxItem bind:group={valueMultiple} name="medium" value="books">Books</ListBoxItem>
	<ListBoxItem bind:group={valueMultiple} name="medium" value="movies">Movies</ListBoxItem>
	<ListBoxItem bind:group={valueMultiple} name="medium" value="tv">TV</ListBoxItem>
</ListBox>
