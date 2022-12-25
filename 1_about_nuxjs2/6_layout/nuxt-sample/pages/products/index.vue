<template>
  <div>
    一覧表示<br>
    <NuxtLink to="/products/create">新規作成</NuxtLink>
    <table>
      <tr>
        <th>商品番号</th>
        <th>商品名</th>
        <th>詳細</th>
        <th>編集</th>
      </tr>
      <tr>
        <td>1</td>
        <td>VTI</td>
        <td><NuxtLink to="/products/1/show">詳細</NuxtLink></td>
        <td><NuxtLink to="/products/1/edit">編集</NuxtLink></td>
      </tr>
      <tr>
        <td>2</td>
        <td>VTI2</td>
        <td><NuxtLink to="/products/2/show">詳細</NuxtLink></td>
        <td><NuxtLink to="/products/2/edit">編集</NuxtLink></td>
      </tr>
    </table>
    <br>
    <br>
    <div>
      <h1>自動インポート</h1>
      <NuxtLink to="/about">about</NuxtLink>
      <NuxtLogo />

      <h2>フォルダ名あり</h2>
      <BaseHeader />

      <h2>フォルダ名なし(nuxt.config.js編集)</h2>
      <Header />
      <div>
        - components: true,
        + components: {
            dirs: [
              '~/componets',
              '~/components/base'
            ]
          },
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>