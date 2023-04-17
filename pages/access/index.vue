<template>
    <div class="max-w-2xl">
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
            Sign-in Sigma
        </h2>
        <p class="text-lg leading-8 text-gray-600">
            登入您的 Sigma 帳號
        </p>
        <p class="mt-6 text-lg leading-8 text-gray-600">
            你好，請問您需要什麼協助？
        </p>
    </div>
    <div class="grid gap-x-8 gap-y-12 sm:grid-cols-2 sm:gap-y-16 xl:col-span-2">
        <div class="m-4 text-lg leading-8 text-gray-600">
            <div class="mb-6">請輸入您的電子郵件：</div>
            <form class="flex">
                <input class="rounded-l-lg p-4 border-t mr-0 border-b border-l text-gray-800 border-gray-200 bg-white"
                    placeholder="your@mail.com" />
                <button class="px-8 rounded-r-lg bg-teal-400  text-white font-bold p-4 uppercase border-teal-500 border-t border-b border-r">
                    <Icon name="material-symbols:arrow-right-alt-rounded" size="32" />
                </button>
            </form>
        </div>
    </div>
</template>

<script setup>
useHead({
  title: "Sign-in",
});
</script>
