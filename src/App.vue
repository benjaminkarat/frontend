<template>
  <AppProvider>
    <Layout>
      <LayoutSection>
        <Navigation />
      </LayoutSection>
      <LayoutSection :secondary="true">
        <Banner
          title="Hello World"
          status="success"
          :action="{ content: 'Action', url:'https://google.com' }"
          :secondaryAction="{ content: 'View all', url:'https://google.com' }"
          @dismiss="dismissHandler"
        >
            <p>Hello I am a Shopify looking thing</p>
        </Banner>
      </LayoutSection >
      <LayoutSection :secondary="true">
        <Banner
          title="Hello World"
          status="success"
          :action="{ content: 'Action', url:'https://google.com' }"
          :secondaryAction="{ content: 'View all', url:'https://google.com' }"
          @dismiss="dismissHandler"
        >
            <p>Hello I am a Shopify looking thing</p>
        </Banner>
      </LayoutSection >
      
    </Layout>
  </AppProvider>
</template>

<script>
import Navigation from './Navigation.vue'
export default {
  components: {
    Navigation
  }
}
</script>