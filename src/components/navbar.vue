<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
import { Avatar } from 'flowbite-vue'
</script>
<template>
    <Navbar>
      <template #logo>
        <NavbarLogo link="https://www.google.com/" alt="Flowbite logo" image-url="logo-removebg-preview.png">
          Rival Nugraha
        </NavbarLogo>
      </template>
      <template #default="{isShowMenu}">
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink is-active>Beranda</NavbarLink>
          <NavbarLink>Tentang</NavbarLink>
          <NavbarLink>Asal Sekolah</NavbarLink>
          <NavbarLink>Bakat</NavbarLink>
        </NavbarCollapse>
      </template>
      <template #right-side>
        <Avatar status="online" bordered rounded img="riska.jpg.jfif" class="mr-2.5" />
      </template>
    </Navbar>
</template>
