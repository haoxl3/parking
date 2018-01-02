<template>
    <div class="container">
        <div class="search-container">
            <div class="search-text">北京<i class="iconfont">&#xe660;</i></div>
            <div class="search-box">
                <i class="iconfont">&#xe7d1;</i>
                <input type="text"/>
            </div>
        </div>
    </div>
</template>
<style lang="stylus">
.container{
  padding: 10px;
  background-color: #fff;
}
.search-container{
    display: flex;
    .search-text{
        width: 60px;
        line-height: 30px;
        overflow: hidden;
        position: relative;
        i{
            position: absolute;
            right: 4px;
            font-size: 12px;
        }
    }
    .search-box{
        flex: 1;
        border: 1px solid #ccc;
        padding: 0 10px 0 30px;
        border-radius: 20px;
        position: relative;
        height: 30px;
        i{
            position: absolute;
            top: 5px;
            left: 10px;
        }
        input{
            width: 100%;
            height: 100%;
        }
    }
}
</style>