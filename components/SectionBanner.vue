<template>
  <div class="tm-section-container">
    <div class="cards">
      <a
        href="https://hackatomv.devpost.com/rules"
        target="_blank"
        rel="noreferrer noopener"
        class="bg"
      >
        <div class="left">
          <img
            src="/brandmark/hackatom-brandmark-v-white.svg"
            alt="Hackatom brandmark"
            class="top-right"
          />
          <div class="left__title-left tm-rf2 tm-bold tm-lh-title">
            View the rules
          </div>
          <div
            class="left__desc-left tm-rf-1 tm-rf0-l-up tm-lh-copy tm-measure-narrow"
          >
            hackatomv.devpost.com/rules
          </div>
        </div>
      </a>
      <a
        href="https://discord.com/channels/669268347736686612/746658605213810779"
        target="_blank"
        rel="noreferrer noopener"
        class="container"
      >
        <div class="left">
          <div class="left__title-right tm-rf2 tm-bold tm-lh-title">
            Join the conversation
          </div>
          <div
            class="left__desc-right tm-rf-1 tm-rf0-l-up tm-lh-copy tm-measure-narrow"
          >
            Chat with mentors and other Cosmosnauts in the
            <span class="tm-rf0 tm-code">#hackatom-v</span> channel of the
            Cosmos Community Discord.
          </div>
        </div>
      </a>
    </div>
  </div>
</template>

<style lang="stylus" scoped>
/deep/
  .tm-code
    color var(--primary-600)

.cards
  padding-bottom var(--spacing-10)
  display grid
  grid-template-columns 1fr 1fr
  gap var(--spacing-7)
  grid-column 1 / span 12
  max-width $max-width-9
  center()

.bg
  min-height var(--spacing-13)
  position relative
  display flex
  flex-direction row
  justify-content space-between
  background linear-gradient(180deg, #1D1D1D 0%, #2E2D2D 100%)
  border 2px solid var(--dark-gray)
  box-shadow var(--elevation-16)
  border-radius 0.75rem
  hover-elevation 24
  hover-raise()

.container
  min-height var(--spacing-13)
  position relative
  display flex
  flex-direction row
  justify-content space-between
  background var(--near-black)
  border 2px solid var(--dark-gray)
  box-shadow var(--elevation-16)
  border-radius 0.75rem
  background-image url('/bg/poker-tables.jpg')
  background-repeat no-repeat
  background-position top center
  background-size 100% auto
  hover-elevation 24
  hover-raise()

  &:hover,
  &:focus
    background-size 105% auto
    .right__icon
      transform translateX(3px)

.top-right
  top 1.5rem
  right 1.5rem
  position absolute

.left
  padding var(--spacing-12) var(--spacing-7) var(--spacing-7)
  display flex
  align-items flex-start
  justify-content flex-end
  flex-direction column

  &__title-left
    margin-bottom var(--spacing-5)
    color var(--white)
    position relative

    &::after
      content "↗"
      position absolute
      bottom 0.266em
      padding-left 0.1875em
      font-size 0.85em
      line-height 1
      transition transform 0.2s ease-out 0s

  &__desc-left
    color var(--white-700)

  &__title-right
    margin-bottom var(--spacing-5)
    color var(--white)
    position relative

    &::after
      content "↗"
      position absolute
      bottom 0.266em
      padding-left 0.1875em
      font-size 0.85em
      line-height 1
      transition transform 0.2s ease-out 0s

  &__desc-right
    color var(--white-700)

@media $breakpoint-xsmall-only
  .cards
    grid-template-columns auto

@media $breakpoint-medium
  .container
    background-position right center
    background-size auto 100%
    &:hover,
    &:focus
      background-size auto 103%

  .left
    padding-top var(--spacing-7)
</style>
