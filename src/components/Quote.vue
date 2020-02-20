<template>
    <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="panel panel-default">
            <div class="panel-body quote">
                <slot></slot>
            </div>
        </div>
    </div>
</template>

<style>
    .panel-body {
        font-family: 'Tangerine', serif;
        font-size: 48px;
        text-shadow: 4px 4px 4px #aaa;
    }
    .quote {
        cursor: pointer;
    }
    .quote:hover {
        background-color: #ffe2e2;
    }
</style>