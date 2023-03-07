<template>
  <Banner
    title="Hello World"
    status="success"
    :action="{ content: 'Action', url:'https://google.com' }"
    :secondaryAction="{ content: 'View all', url:'https://google.com' }"
    @dismiss="dismissHandler"
>
    <slot></slot>
</Banner>
</template>

<script>
</script>