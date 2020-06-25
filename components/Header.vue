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
            <NLink to="/blog">Blog</NLink>
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
          content: "Coming Soon";
          position: absolute;
          left: -100%;
          color: black;
          font-weight: 100;
          padding: 2px;
          font-size: 12px;
        }
      }
      a {
        color: black;
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

  background-color: #ebecf0;
  text-shadow: 1px 1px 0 white;

  box-shadow: -5px -5px 20px white, 5px 5px 20px #babecc;
  transition: all 0.2s ease-in-out;
  cursor: pointer;
  font-weight: 600;

  height: 50px;
  width: 50px;

  display: flex;
  justify-content: center;
  align-items: center;

  i {
    color: black;
    font-size: 20px;
  }
}

// .open-menu:hover {
//   .primary-menu {
//     display: none;
//     transform: translateX(0%);
//     animation: 4s appear;
//     transition: 1s;
//   }
// }
</style>
