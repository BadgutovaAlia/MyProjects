<nav>
    <div class="nav-container">
      <a href="/" class="nav-logo" title="Back to Homepage">Бадгутова Альфия</a>
      <div class="nav-links">
        {#each nav as link}
<a href={link.href} class="link">{link.title}</a>
{/each}
      </div>
    </div>
  </nav>
  <div class="container">
    <!-- Pages will be injected below -->
    <slot></slot>
  </div>
  <svelte:head>
    <title>Бадгутова Альфия</title>
    </svelte:head>
<script>
        const nav = [
        {
          title: 'Обо мне',
          href: '/about'
        },
        {
          title: 'Блог',
          href: '/blog'
        },
        {
          title: 'Портфолио',
          href: '/projects'
        },
        {
          title: 'Контакты',
          href: '/contacts'
        },
      ]
</script>
    