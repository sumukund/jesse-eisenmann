<script lang="ts">
  import NavBar from './lib/NavBar.svelte';
  import Home from './lib/Home.svelte';
  import SectionPage from './lib/SectionPage.svelte';
  import { navLinks, siteName, type PageId } from './lib/site';

  let currentPage: PageId = $state('home');

  const pageTitles: Record<Exclude<PageId, 'home'>, string> = Object.fromEntries(
    navLinks.map((link) => [link.id, link.label]),
  ) as Record<Exclude<PageId, 'home'>, string>;

  function navigate(page: PageId) {
    currentPage = page;
  }
</script>

<div class="layout">
  <header>
    <button type="button" class="site-name" onclick={() => navigate('home')}>
      {siteName}
    </button>
  </header>

  <div class="body">
    <NavBar {currentPage} onNavigate={navigate} />

    <main>
      {#if currentPage === 'home'}
        <Home />
      {:else}
        <SectionPage title={pageTitles[currentPage]} />
      {/if}
    </main>
  </div>
</div>

<style>
  .layout {
    min-height: 100svh;
    max-width: 960px;
    margin: 0 auto;
    padding: 2rem 1.5rem;
    box-sizing: border-box;
  }

  header {
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid var(--border);
  }

  .site-name {
    background: none;
    border: none;
    padding: 0;
    font-family: var(--heading);
    font-size: 2rem;
    font-weight: 500;
    letter-spacing: -0.02em;
    color: var(--text-h);
    cursor: pointer;
  }

  .site-name:hover {
    opacity: 0.75;
  }

  .body {
    display: flex;
    gap: 2rem;
    align-items: flex-start;
  }

  main {
    flex: 1;
    min-width: 0;
    padding-top: 0.25rem;
  }

  @media (max-width: 768px) {
    .layout {
      padding: 1.25rem 1rem;
    }

    .site-name {
      font-size: 1.5rem;
    }

    .body {
      flex-direction: column;
    }
  }
</style>
