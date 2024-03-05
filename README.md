# @cmi-dair/skeleton-themes

Child Mind Institute's Skeleton themes.

## Getting Started

To install this theme, run the following command:

```bash
npm install @cmi-dair/skeleton-themes
```

In your `tailwind.config.ts` file, add the custom theme as follows:

```typescript
import { cmiLight } from '@cmi-dair/skeleton-themes'

export default {
    ...,
    plugins: [
        skeleton({
            themes: {
                custom: [cmiLight]
            }
        })
    ]
} satisfies Config;

```

Next, in your root `+layout.svelte` add the following:

```svelte
<script>
    import '@cmi-dair/skeleton-themes/cmi.postcss';
</script>
```
