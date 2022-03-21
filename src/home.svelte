<script>
  import Icon from './icon.svelte'

  const name = 'Jeremiah Montoya'

  const links = {
    github: 'https://github.com/thisjeremiah',
    twitter: 'https://twitter.com/thisjeremiah',
    linkedin: 'https://www.linkedin.com/in/jeremiah-montoya-32a9a390',
    standardvision: 'https://www.standardvision.com/svrunner-software',
  }
</script>

<svelte:head>
  <title>JEREMIAH MONTOYA</title>
</svelte:head>

<main class="p-10 bg-gray-50">
  <div class="h-screen flex items-center justify-center w-full">
    <div class="flex flex-col gap-3">
      <h1 class="text-lg font-bold text-center uppercase">{name}</h1>
      <div class="flex justify-center gap-3">
        <a href="{links.github}" target="_blank">
          <Icon name="github" />
        </a>
        <a href="{links.standardvision}" target="_blank">
          <Icon name="standardvision" />
        </a>
        <a href="{links.linkedin}" target="_blank">
          <Icon name="linkedin" />
        </a>
        <a href="{links.twitter}" target="_blank">
          <Icon name="twitter" />
        </a>
      </div>
    </div>
  </div>
</main>
