<template>
  <div class="header-menu">
    <!-- <div class="hamburger-icon">
      <i class="fas fa-bars"></i>
    </div>-->
    <div>
      <nav>
        <ul>
          <li>
            <nuxt-link to="/blogs">Blogs</nuxt-link>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>


<style  lang="scss">
.header-menu {
  position: absolute;
  right: 0;
  top: 0;
  padding: 30px;
  nav {
    ul {
      padding-left: 0;
      li {
        list-style: none;
        margin: 10px;
        display: inline-block;
        &:last-child {
          margin-right: 0;
        }
        a {
          color: #ae1100;
          text-shadow: 1px 1px 0 white;
          text-transform: uppercase;
          font-weight: bold;

          &:hover {
            text-shadow: 1px 2px 0 white;
            animation: 1s appear;
          }
        }
      }
    }
  }
}

.hamburger-icon {
  background-color: #ebecf0;
  text-shadow: 1px 1px 0 white;
  margin: 50px auto;

  box-shadow: -2px -2px 5px white, 2px 2px 5px #babecc;
  transition: all 0.2s ease-in-out;
  cursor: pointer;
  font-weight: 600;

  height: 50px;
  width: 50px;

  margin-bottom: 20px;
  display: flex;
  justify-content: center;
  align-items: center;

  &:hover {
    box-shadow: -5px -5px 20px white, 5px 5px 20px #babecc;
  }
}
</style>
