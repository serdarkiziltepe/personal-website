<template>
  <div class="header-menu">
    <div class="open-menu">
      <i class="fas fa-bars"></i>

      <nav class="primary-menu">
        <ul>
          <li>
            <a href>Home</a>
          </li>
          <li>
            <a href>About</a>
          </li>
          <li>
            <a href>Blogs</a>
          </li>
          <li>
            <a href>Publications</a>
          </li>
          <li>
            <a href>Contact</a>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>
<style  lang="scss">
.header-menu {
  position: absolute;
  top: 0px;
  right: 0px;
  height: 100vh;
  padding: 50px;

  ul {
    padding-left: 0;
    li {
      margin-top: 20px;

      &:first-child {
        margin-top: 0;
      }

      &:hover {
        &::before {
          content: "Cooming Soon";
          position: absolute;
          left: -100%;
          color: white;
          font-weight: 100;
          padding: 2px;
          font-size: 12px;
        }
      }
      a {
        color: white;
        text-decoration: none;
        list-style: none;
        font-size: 15px;
        text-transform: uppercase;
        transform: rotate(-90deg);
      }
    }
  }
}

.primary-menu {
  transform: translateX(150%);
  margin-top: 20px;
}

.open-menu {
  text-align: center;
  margin-bottom: 20px;
  cursor: pointer;
  i {
    color: white;
    font-size: 20px;
  }
}

.open-menu:hover {
  .primary-menu {
    transform: translateX(0%);
    animation: 4s appear;
    transition: 1s;
  }
}
</style>
