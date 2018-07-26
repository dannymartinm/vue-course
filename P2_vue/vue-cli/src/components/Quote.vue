<template>
    <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="panel panel-default">
            <div class="panel-body quote">
                <slot></slot>
            </div>
        </div>
    </div>
</template>
<script>
</script>
<style>
.panel-body {
  font-family: "Courier New", Courier, monospace;
  font-size: 24px;
  color: #6e6e6e;
}
.quote {
  cursor: pointer;
}

.panel {
  border-style: "1px solid green";
}
.quote:hover {
  background-color: #ffe2e2;
}
</style>
