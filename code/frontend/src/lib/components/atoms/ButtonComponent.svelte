<script lang="ts">

    interface Props {
        label: string,
        backgroundColor: string
    };

    let { label, backgroundColor }: Props = $props();

</script>

<button class={backgroundColor}>{label}</button>