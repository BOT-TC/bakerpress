---
prev: Bob's Your Uncle
---

# Unit 2: Time to Get Making

---
{{ 1 + 1 }}

---
<span v-for="i in 7">{{ i }}</span>

<script setup>
import { useData } from 'vitepress'
import AddCountBtn from '../../components/AddCountBtn.vue'
import YouTube from '../../components/YouTube.vue'

const { page } = useData()
</script>

<pre>{{ page }}</pre>

::: v-pre
`{{ This will be displayed as-is }}`
:::

<AddCountBtn />

<YouTube vid="BsvxiBaUC3U" border="1" />
