<template>
  <AppProvider>
    <Layout>
      <LayoutSection>
        <Navigation />
      </LayoutSection>
      <LayoutSection :secondary="true">
        <CustomBanner>
          <p>Hello</p>
        </CustomBanner>
      </LayoutSection >
      <LayoutSection :secondary="true">
        <CustomBanner>
          <p>Hello 2</p>
        </CustomBanner>
      </LayoutSection >
      
    </Layout>
  </AppProvider>
</template>

<script>
import Navigation from './components/components/Navigation.vue'
import CustomBanner from './components/components/Banner.vue'
export default {
  components: {
    Navigation,
    CustomBanner
  }
}
</script>