<template>
  <div class="relative">
    <div class="sticky top-0 flex h-screen flex-col items-center justify-center bg-green-400">
      <h2 class="text-4xl">Quasar Tailwind</h2>
      <p>Scroll Down</p>
    </div>
    <div
      class="sticky top-0 flex h-screen flex-col items-center justify-center bg-indigo-600 text-white"
    >
      <h2 class="mb-4 text-4xl">Example Component</h2>
      <example-component
        title="Example component"
        active
        :todos="todos"
        :meta="meta"
      ></example-component>
    </div>
    <div
      class="sticky top-0 flex h-screen flex-col items-center justify-center bg-purple-600 text-white"
    >
      <h2 class="text-4xl">The Third Title</h2>
      <p>Scroll Down</p>
    </div>
    <div
      class="sticky top-0 flex h-screen flex-col items-center justify-center bg-neutral-800 text-white"
    >
      <h2 class="text-4xl">The Fourth Title</h2>
    </div>
  </div>
</template>

<script lang="ts">
import { Todo, Meta } from 'components/models';
import ExampleComponent from 'components/ExampleComponent.vue';
import { defineComponent, ref } from 'vue';

export default defineComponent({
  name: 'IndexPage',
  components: { ExampleComponent },
  setup() {
    const todos = ref<Todo[]>([
      {
        id: 1,
        content: 'ct1',
      },
      {
        id: 2,
        content: 'ct2',
      },
      {
        id: 3,
        content: 'ct3',
      },
      {
        id: 4,
        content: 'ct4',
      },
      {
        id: 5,
        content: 'ct5',
      },
    ]);
    const meta = ref<Meta>({
      totalCount: 1200,
    });
    return { todos, meta };
  },
});
</script>
