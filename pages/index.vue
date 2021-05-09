<template>
  <CFlex
    d="flex"
    w="100vw"
    h="100vh"
    flex-dir="column"
    justify-content="center"
    align-items="center"
  >
    <CBox
      bg="#3d3d56"
      text-align="center"
      w="90%"
      max-width="320px"
      p="4"
      color="white"
      border-radius="6px"
    >
      <CStack spacing="3">
        <CText font-size="3xl">Login</CText>
        <CInput color="grey" placeholder="Login" />
        <CInput color="grey" placeholder="Password" />
        <CButton variant-color="blue" @click="print">Login</CButton>
      </CStack>
    </CBox>
  </CFlex>
</template>

<script>
export default {
  methods: {
    print() {
      // eslint-disable-next-line no-console
      console.log('batata')
      this.$router.push({
        path: '/home',
      })
    },
  },
}
</script>

<style></style>
