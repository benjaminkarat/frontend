<template>
  <Frame>
    <template #navigation>
        <Navigation location="/">
        <NavigationSection
            :items="navItems"
            :rollup="{ after: 3, view: 'view', hide: 'hide', activePath: '/' }"
        />
        </Navigation>
    </template>
  </Frame>
</template>

<script>
import CirclePlusMinor from '@shopify/polaris-icons/dist/svg/CirclePlusMinor.svg';
import CustomersMajor from '@shopify/polaris-icons/dist/svg/CustomersMajor.svg';
import MeasurementMinor from '@shopify/polaris-icons/dist/svg/MeasurementMinor.svg';

export default {
  setup() {
    const navItems = [
        { url: '#', label: 'About You', icon: CustomersMajor, selected: true },
        { url: '#', label: 'Customization', icon: CirclePlusMinor },
        { url: '#', label: 'Measurement', icon: MeasurementMinor},
    ]
    return { navItems };
  },
}
</script>

<style>

</style>