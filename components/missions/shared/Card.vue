<template>
  <div class="card">
    <slot />
  </div>
</template>

<style lang="sass" scoped>
.card
  width: 240px
  background-color: rgba(white, .05)
  display: flex
  flex-direction: column
  align-items: center
  margin: 20px
  padding: 20px 20px 0
  border-radius: 8px
  margin-top: 40px
  color: white
  animation: fade .5s
  transition: all .5s ease

  @media (min-width: 768px)
    margin-top: 60px
    width: 340px
    padding: 20px 30px 0

  &:hover
    transform: translateY(-10px)

  h3
    margin: 10px 0
    font-weight: 700
    font-size: 20px

    @media (min-width: 768px)
      font-size: 24px
</style>
