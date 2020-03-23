<script>
  import { onMount } from "svelte";

  let showMobileMenu = false;

  const navItems = [
    { label: "Home", href: "." },
    { label: "Services", href: "services" },
    { label: "News", href: "news" },
    { label: "Contact", href: "contact" }
  ];

  const handleMobileIconClick = () => (showMobileMenu = !showMobileMenu);

  // Media match query handler
  const mediaQueryHandler = e => {
    // Reset mobile state
    if (!e.matches) {
      showMobileMenu = false;
    }
  };

  // Attach media query listener on mount hook
  onMount(() => {
    const mediaListener = window.matchMedia("(max-width: 767px)");

    mediaListener.addListener(mediaQueryHandler);
  });
  export let segment;
</script>

<style>
  nav {
    background-color: #4971c7;
    font-family: "Helvetica Neue", "Helvetica", "Arial", sans-serif;
    height: 65px;
  }

  .inner {
    padding-left: 20px;
    padding-right: 20px;
    margin: auto;
    box-sizing: border-box;
    display: flex;
    align-items: center;
    height: 100%;
    float: right;
  }

  .mobile-icon {
    width: 25px;
    height: 14px;
    position: relative;
    cursor: pointer;
    display: inline-block;
    margin-left: 20px;
    margin-top: 25px;
  }

  .mobile-icon:after,
  .mobile-icon:before,
  .middle-line {
    content: "";
    position: absolute;
    width: 100%;
    height: 2px;
    background-color: #fff;
    transition: all 0.4s;
    transform-origin: center;
  }

  .mobile-icon:before,
  .middle-line {
    top: 0;
  }

  .mobile-icon:after,
  .middle-line {
    bottom: 0;
  }

  .mobile-icon:before {
    width: 66%;
  }

  .mobile-icon:after {
    width: 33%;
  }

  .middle-line {
    margin: auto;
  }

  .mobile-icon:hover:before,
  .mobile-icon:hover:after,
  .mobile-icon.active:before,
  .mobile-icon.active:after,
  .mobile-icon.active .middle-line {
    width: 100%;
  }

  .mobile-icon.active:before,
  .mobile-icon.active:after {
    top: 50%;

    transform: rotate(-45deg);
  }

  .mobile-icon.active .middle-line {
    transform: rotate(45deg);
  }

  .navbar-list {
    display: none;
    width: 100%;
    margin: 0;
    padding: 0 40px;
    z-index: 99;
  }

  .navbar-list.mobile {
    background-color: rgba(0, 0, 0, 0.8);
    position: fixed;
    display: block;
    height: calc(100% - 65px);
    bottom: 0;
    left: 0;
  }

  .navbar-list li {
    list-style-type: none;
    position: relative;
  }

  .navbar-list li:before {
    content: "";
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 1px;
    background-color: #454342;
  }

  .navbar-list a {
    color: #fff;
    text-decoration: none;
    display: flex;
    height: 65px;
    align-items: center;
    padding: 0 10px;
    font-size: 18px;
  }

  @media only screen and (min-width: 767px) {
    .mobile-icon {
      display: none;
    }

    .navbar-list {
      display: flex;
      padding: 0;
    }

    .navbar-list a {
      display: inline-flex;
    }
  }

  .logo {
    display: inline-block;
    margin-left: 20px;
    margin-top: 12px;
    color: white;
    font-size: 25px;
  }

  a:hover {
    background-color: #3b5998;
  }

  a {
    text-decoration: none;
    padding: 5px;
  }
</style>

<nav>
  <div
    on:click={handleMobileIconClick}
    class={`mobile-icon${showMobileMenu ? ' active' : ''}`}>
    <div class="middle-line" />
  </div>
  <div class="logo">
    <a href=".">Websolver</a>
  </div>
  <div class="inner">
    <ul class={`navbar-list${showMobileMenu ? ' mobile' : ''}`}>
      {#each navItems as item}
        <li>
          <div class="topnav-right">
            <a
              aria-current={segment === undefined ? 'page' : undefined}
              href={item.href}>
              {item.label}
            </a>
          </div>
        </li>
      {/each}
    </ul>
  </div>
</nav>
