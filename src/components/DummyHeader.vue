<template>
  <header class="navbar">
    <div class="left">
      <img
        src="https://g.foolcdn.com/static/affiliates/project/images/AscentLogo.svg"
        alt="the ascent"
      />
    </div>
    <div class="right">
      <ul class="nav-links">
        <li class="nav-link">
          Credit Cards
          <font-awesome-icon :icon="['fa', 'chevron-down']" size="xs" />
        </li>
        <li class="nav-link">
          Banking
          <font-awesome-icon :icon="['fa', 'chevron-down']" size="xs" />
        </li>
        <li class="nav-link">
          Brokerages
          <font-awesome-icon :icon="['fa', 'chevron-down']" size="xs" />
        </li>
        <li class="nav-link">
          Loans
          <font-awesome-icon :icon="['fa', 'chevron-down']" size="xs" />
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "DummyHeader"
};
</script>

<style scoped>
.navbar {
  display: flex;
  flex-direction: row;
  align-items: center;
  height: 5.7rem;
  box-shadow: rgba(0, 0, 0, 0.1) 0 1px 1px 0;
  padding: 0 2.2rem;
}

.left {
  width: 40%;
  padding-left: 6rem;
}

img {
  cursor: pointer;
}

.right {
  width: 60%;
  padding-right: 6rem;
}

.nav-links {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  list-style: none;
}

.nav-link {
  font-size: 1.6rem;
  line-height: 25px;
  padding: 10px 30px;
  cursor: pointer;
}

@media (max-width: 768px) {
  .left {
    display: flex;
    justify-content: center;
    width: 100%;
    padding: 0;
  }

  .right {
    display: none;
  }

  img {
    margin: 0 auto;
  }
}
</style>
