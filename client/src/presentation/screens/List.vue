<script setup>
import { List, ListItem, ListCard } from '@/presentation/components'
</script>

<template>
  <List>
    <ListItem
      :title="'Ивент номер 892'"
      :subtitle="'тусовка лютая на станции метро лютая тут будет лютій движ всемх зовем к себе йоу лютая движуха '"
      :big-avatar="true"
      :right-icon="'settings-faq'"
      :avatar="{src: 'https://i.pinimg.com/236x/d5/d2/94/d5d29411853687bf56aac284de8650f6.jpg'}"
    />
    <ListItem
      :title="'dronto'"
      :subtitle="'dronto'"
      :big-avatar="true"
      :avatar="{src: 'https://i.pinimg.com/236x/d5/d2/94/d5d29411853687bf56aac284de8650f6.jpg'}"
    />
    <ListCard
      :title="'dronto fractalum'"
      :picture="'https://yt3.googleusercontent.com/UmuHBjKgIi2TD8HKImnH1ZWo7gkbjPv50mWbEyac2CzB7NzfBrFE1swklzBSAQT5q8rGITelsA=s900-c-k-c0x00ffffff-no-rj'"
    >
      <template #visible>
        <ListItem
          :title="'dronto'"
          :subtitle="'dronto'"
          :big-avatar="true"
          :avatar="{src: 'https://i.pinimg.com/236x/d5/d2/94/d5d29411853687bf56aac284de8650f6.jpg'}"
        />
      </template>
    </ListCard>
    <ListCard
      :title="'dronto'"
      :picture="'https://yt3.googleusercontent.com/UmuHBjKgIi2TD8HKImnH1ZWo7gkbjPv50mWbEyac2CzB7NzfBrFE1swklzBSAQT5q8rGITelsA=s900-c-k-c0x00ffffff-no-rj'"
    />
  </List>
</template>
