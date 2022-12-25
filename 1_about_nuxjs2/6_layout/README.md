■レイアウトのカスタマイズ
編集する場合はlayouts/default.vueを作成する
<templeate>
  <div>
    全ページに表示
    <Nuxt />
  </div>
</template>

.nuxt/layoutsをコピーして.nuxtと同じ階層に貼り付け

■別のレイアウトを指定する場合
layouts/blog.vueを作成
pages/blog.vueの中でlayoutを指定する

export default {
  layout: 'blog'
}