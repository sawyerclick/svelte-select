<script>
    import Select from '$lib/Select.svelte';

    let items = [
        { value: 'one', label: 'One' },
        { value: 'two', label: 'Two' },
        { value: 'three', label: 'Three' },
    ];

    let value;
</script>

<pre>{JSON.stringify(value, null, 2)}</pre>

<Select {items} multiple filterSelectedItems={false} bind:value />
