<script setup lang="ts">
import { UploadRawFile } from '@zi-shui/components/upload/src/upload';

  const handleBeforeUpload = (rawFile:UploadRawFile)=>{

    // return false;
    return true
  }
</script>

<template>
  <z-upload multiple :before-upload="handleBeforeUpload" action="http://localhost:4000/upload" drag>
    <z-button>点我上传</z-button>
  </z-upload>
</template>
