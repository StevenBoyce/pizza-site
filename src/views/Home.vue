<template>
  <div class="home">
    <h1>Thank you for your desire to eat DATPIZZADOUGH</h1>
    <div class="floating-block">
      <p>
        No, Marty, we've already agreed that having information about the future
        could be extremely dangerous. Even if your intentions are good, they
        could backfire drastically. Whatever you've got to tell me I'll find out
        through the natural course of time. What did you say? Ronald Reagon, the
        actor? Then who's vice president, Jerry Lewis? I suppose Jane Wymann is
        the first lady. Oh, if Paul calls me tell him I'm working at the
        boutique late tonight. Last night, Darth Vader came down from planet
        Vulcan. And he told me that if I didn't take Lorraine, that he'd melt my
        brain. <br />
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>

<style lang="less" scoped>
@import "../styles/globals";
.home {
  .floating-block {
    padding: 20px;
    margin: 80px 0 0 30px;
    background-color: @text-box-background;
    box-sizing: border-box;
    width: 50%;
    p {
      text-align: left;
    }
  }
}
</style>
