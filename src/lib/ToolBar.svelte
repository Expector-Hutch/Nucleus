<script lang="ts">
    import { commands } from "../config/commands";
</script>

<div id="toolbar">
    <div class="tool-bar-button" on:click={commands.buildFile.command}>
        <svg
            class="icon"
            style="vertical-align: middle; fill: currentcolor; overflow: hidden;"
            viewBox="0 0 1024 1024"
            version="1.1"
            xmlns="http://www.w3.org/2000/svg"
            ><path
                d="M948.607 245.269L535.785 21.964c-14.892-8.055-32.676-8.055-47.574 0.002L75.39 245.27a49.95 49.95 0 0 0-26.21 43.978v445.504a49.951 49.951 0 0 0 26.212 43.979l412.822 223.305c7.446 4.027 15.614 6.04 23.784 6.04s16.34-2.013 23.79-6.042L948.61 778.73a49.95 49.95 0 0 0 26.21-43.978V289.248a49.951 49.951 0 0 0-26.212-43.979z m-53.789 471.604L512 923.948 129.182 716.873V307.127L512 100.052l382.818 207.075v409.746zM243.17 317.723c-19.367-10.627-43.682-3.54-54.31 15.826-10.626 19.368-3.54 43.683 15.827 54.31l266.935 146.463v276.887c0 22.092 17.908 40 40 40s40-17.908 40-40V534.806l267.495-144.841c19.427-10.519 26.648-34.794 16.13-54.22s-34.797-26.649-54.222-16.129l-268.97 145.64L243.17 317.723z"
                p-id="8785"
            ></path></svg
        >
    </div>
    <div class="tool-bar-button" on:click={commands.runFile.command}>
        <svg
            class="icon"
            style="vertical-align: middle; fill: currentcolor; overflow: hidden;"
            viewBox="0 0 1024 1024"
            version="1.1"
            xmlns="http://www.w3.org/2000/svg"
            ><path
                d="M162.816 998.4a25.6256 25.6256 0 0 1-25.6-25.6V51.2a25.5744 25.5744 0 0 1 39.7056-21.3504l698.368 460.8a25.6256 25.6256 0 0 1 0 42.7008l-698.368 460.8c-4.2752 2.816-9.1904 4.2496-14.1056 4.2496z m25.6-899.6352v826.496L814.6944 512 188.416 98.7648z"
                p-id="4060"
            ></path></svg
        >
    </div>
    <div class="tool-bar-button" on:click={commands.buildRunFile.command}>
        <svg
            class="icon"
            style="vertical-align: middle; fill: currentcolor; overflow: hidden; --darkreader-inline-fill: currentcolor;"
            viewBox="0 0 1024 1024"
            version="1.1"
            xmlns="http://www.w3.org/2000/svg"
            ><path
                d="M64 128v768h896V128H64zM0 64h1024v896H0V64z"
            ></path><path
                d="M64 256h896v64H64zM448 704H768V768H448zM290.2784 772.548267l162.269867-162.269867L290.2784 448l-45.2608 45.252267 117.0176 117.026133L245.0176 727.296z"
            ></path></svg
        >
    </div>
</div>

<style lang="scss">
    #toolbar {
        display: flex;
    }
    .tool-bar-button {
        color: aliceblue;
        height: calc(100% - 3px);
        svg {
            height: calc(100% - 3px);
        }
    }
</style>
