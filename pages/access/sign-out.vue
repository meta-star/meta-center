<template>
    <div class="max-w-2xl">
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
            Sign-out Sigma
        </h2>
        <p class="text-lg leading-8 text-gray-600">
            登出您的 Sigma 帳號
        </p>
        <p class="mt-6 text-lg leading-8 text-gray-600">
            您是否確定登出您的 Sigma 帳號？
        </p>
    </div>
    <div class="grid gap-x-8 gap-y-12 sm:grid-cols-2 sm:gap-y-16 xl:col-span-2">
        <div class="m-4 text-lg leading-8 text-gray-600">
            <div class="mb-6">若您確定登出帳號，請選擇「<Icon name="material-symbols:sign-language-outline" size="16" />」</div>
            <div class="flex justify-between">
                <button
                    class="px-8 rounded-lg bg-slate-400  text-white font-bold p-4 uppercase border-slate-500 border-t border-b border-r"
                    @click="onClickBtnCancel"
                >
                    <Icon name="material-symbols:cancel-outline" size="32" />
                </button>
                <button
                    class="px-8 rounded-lg bg-amber-400  text-white font-bold p-4 uppercase border-amber-500 border-t border-b border-r"
                    @click="onClickBtnSignOut"
                >
                    <Icon name="material-symbols:sign-language-outline" size="32" />
                </button>
            </div>
        </div>
    </div>
</template>

<script setup>
useHead({
  title: "Sign-out",
});

const router = useRouter();

function onClickBtnCancel() {
    router.back();
}

function onClickBtnSignOut() {
    router.push("/access");
}
</script>
