<template>
    <div class="max-w-2xl">
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
            元管理系統
        </h2>
        <p class="text-lg leading-8 text-gray-600">
            MetaStar Projects.
        </p>
        <p class="mt-6 text-lg leading-8 text-gray-600">
            你好，{{ username }}，請問您需要什麼協助？
        </p>
    </div>
    <ul role="list" class="grid gap-x-8 gap-y-12 sm:grid-cols-2 sm:gap-y-16 xl:col-span-2">
        <li v-for="item in items" :key="item.slug">
            <div class="flex items-center gap-x-6">
                <NuxtLink :to="item.slug">
                    <h3 class="text-base font-semibold leading-7 tracking-tight text-gray-900">
                        {{ item.title }}
                    </h3>
                    <p class="text-sm font-semibold leading-6 text-indigo-600">
                        {{ item.name }}
                    </p>
                </NuxtLink>
            </div>
        </li>
    </ul>
</template>
  
<script setup>
const username = "Unknown";

const items = [
    {
        name: "登出 Sigma 帳號",
        title: "Sign-out Sigma",
        slug: "access/sign-out",
    },
    {
        name: "更新 Sigma 帳號資訊",
        title: "Update Sigma account",
        slug: "account",
    },
    {
        name: "團隊管理",
        title: "Manage your Teams",
        slug: "teams",
    },
    {
        name: "虛擬運算中心",
        title: "Virtual compute center",
        slug: "computer",
    },
];
</script>
  