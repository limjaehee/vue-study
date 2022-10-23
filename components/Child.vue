<template>
  <div>
    <p>안녕하세요 저의 이름은 {{ user.name }} 입니다.</p>
    <p>{{ user.age }}살 이구요</p>
    <p v-if="user.type === 1">학생 입니다</p>
    <p v-else-if="user.type === 2">선생님 입니다</p>
    <p v-else-if="user.type === 3">관리자 입니다</p>
    <p v-else>유저 입니다.</p>
  </div>
</template>

<script>
export default {
  name: "VueStudyChild",
  inject: {
    user: {
      default: () => ({
        name: "아무개",
        age: 0,
        type: null,
      }),
    },
  },
};
</script>

<style lang="scss" scoped></style>
