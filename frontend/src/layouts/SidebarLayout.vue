<template>
    <main class="layout">
        <div class="layout__sidebar sidebar">
            <router-link :to="{ name: 'HomeView' }" class="logo layout__logo">
                <img src="@/assets/img/logo.svg" alt="Конструктор пиццы" width="90" height="40" />
            </router-link>

            <slot name="sidebar" />
        </div>

        <div class="layout__content">
            <slot />
        </div>
    </main>
</template>

<style lang="scss">
@import "@/assets/scss/ds-system/ds.scss";
@import "@/assets/scss/sidebar.scss";
</style>