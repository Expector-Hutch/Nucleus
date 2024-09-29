<script lang="ts">
    import { commands } from "../config/commands";
    import { Play, Run, GuiManagement, DocumentAdd, Folder, Document } from "carbon-icons-svelte";
</script>

<div id="toolbar">
    <button title="New" class="tool-bar-button" on:click={commands.addEditorTab.command}>
        <DocumentAdd size={20} />
    </button>
    <button title="Open" class="tool-bar-button" on:click={commands.openFile.command}>
        <Document size={20} />
    </button>
    <button title="Open Folder" class="tool-bar-button" on:click={commands.openFolder.command}>
        <Folder size={20} />
    </button>
    <button title="Build" class="tool-bar-button" on:click={commands.buildFile.command}>
        <GuiManagement size={20} />
    </button>
    <button title="Run" class="tool-bar-button" on:click={commands.runFile.command}>
        <Play size={20} />
    </button>
    <button title="Build & Run" class="tool-bar-button" on:click={commands.buildRunFile.command}>
        <Run size={20} />
    </button>
</div>

<style lang="scss">
    #toolbar {
        display: flex;
        align-items: center;
        padding-left: 5px;
    }
    .tool-bar-button {
        border: 0;
        outline: none;
        background-color: transparent;
        color: white;
        display: flex;
        align-items: center;
        height: 100%;
        width: 24px;
    }
</style>
