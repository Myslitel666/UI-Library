<div>
    <Switch 
        checked = {checked}
        onClick = {toggleThemeMode}
    >
        <ActiveIcon slot="activeIcon" size="1.1rem" />
        <DisabledIcon slot="disabledIcon" size="1.1rem" />
    </Switch>
</div>

<script lang='ts'>
    import { toggleThemeMode } from '../../../store/ColorThemeStore';
    import Switch from "./Switch.svelte";
    import ActiveIcon from '../../icons/Dark.svelte';
    import DisabledIcon from '../../icons/Light.svelte';

    export let checked: boolean = false;                                    /* начальное состояние переключателя */
</script>