<template>
    <el-menu :default-openeds="['1', '2', '3']" style="border-right: none; ">
        <el-menu-item index="3">
            <i class="el-icon-menu"></i>
            <span slot="title">控制台</span>
        </el-menu-item>
        <el-submenu index="1">
            <template slot="title"><i class="el-icon-user-solid"></i>个人中心</template>
            <el-menu-item-group>
                <template slot="title">文档管理</template>
                <el-menu-item index="1-1">我的项目</el-menu-item>
                <el-menu-item index="1-5">我的文章</el-menu-item>
                <el-menu-item index="1-6">我的笔记</el-menu-item>
            </el-menu-item-group>
            <el-menu-item-group>
                <template slot="title">信息</template>
                <el-menu-item index="1-3">基本信息</el-menu-item>
                <el-menu-item index="1-2">我的团队</el-menu-item>
                <el-menu-item index="1-4">安全设置</el-menu-item>
            </el-menu-item-group>
        </el-submenu>
        <el-menu-item index="2">
            <i class="el-icon-s-unfold"></i>
            <span slot="title">用户列表</span>
        </el-menu-item>

        <el-menu-item index="4">
            <i class="el-icon-s-tools"></i>
            <span slot="title">系统配置</span>
        </el-menu-item>
    </el-menu>
</template>

<script>
    import menu from '@/config/menu-config'

    export default {
        data () {
            return {
                menu: menu
            }
        },
        methods: {
            handleOpen (key, keyPath) {
                // console.log(key, keyPath)
            },
            handleClose (key, keyPath) {
                // console.log(key, keyPath)
            }
        }
    }
</script>

<style scoped>
  .over-hide{
    overflow: hidden;
  }

</style>
