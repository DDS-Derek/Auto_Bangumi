<script lang="ts" setup>
definePage({
  name: 'Index',
  redirect: '/bangumi',
});
</script>

<template>
  <div layout-container>
    <ab-topbar />

    <main layout-main>
      <ab-sidebar />

      <div layout-content>
        <ab-page-title :title="$route.name"></ab-page-title>

        <RouterView v-slot="{ Component }">
          <KeepAlive>
            <component :is="Component" />
          </KeepAlive>
        </RouterView>
      </div>
    </main>
  </div>
</template>
