<template>
    <div>
        <h2 class="nav-tab-wrapper">
            <span class="plugin-name">{{ $t('Ninja Tables') }}</span>

            <router-link active-class="nav-tab-active" exact :class="['nav-tab']"
                         :to="{ name: 'home' }"
            >
                {{ $t('Home') }}
            </router-link>

            <router-link active-class="nav-tab-active" exact :class="['nav-tab']"
                         :to="{ name: 'tools' }"
            >
                {{ $t('Tools') }}
            </router-link>
            
            <router-link active-class="nav-tab-active" exact :class="['nav-tab']"
                         :to="{ name: 'help' }"
            >
                {{ $t('Help') }}
            </router-link>
        </h2>

        <router-view></router-view>
    </div>
</template>

<script type="text/babel">
    export default {
        name: 'Home',
    }
</script>

<style>
    .plugin-name {
        float: left;
        padding: 8px 0;
    }
</style>

