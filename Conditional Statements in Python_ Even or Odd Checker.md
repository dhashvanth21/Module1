<!DOCTYPE html>
<!-- saved from url=(0121)https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md -->
<html lang="en" data-color-mode="auto" data-light-theme="light" data-dark-theme="light" data-a11y-animated-images="system" data-a11y-link-underlines="true" data-turbo-loaded=""><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8"><style>.ͼ1.cm-focused {outline: 1px dotted #212121;}
.ͼ1 {position: relative !important; box-sizing: border-box; display: flex !important; flex-direction: column;}
.ͼ1 .cm-scroller {display: flex !important; align-items: flex-start !important; font-family: monospace; line-height: 1.4; height: 100%; overflow-x: auto; position: relative; z-index: 0;}
.ͼ1 .cm-content[contenteditable=true] {-webkit-user-modify: read-write-plaintext-only;}
.ͼ1 .cm-content {margin: 0; flex-grow: 2; flex-shrink: 0; display: block; white-space: pre; word-wrap: normal; box-sizing: border-box; padding: 4px 0; outline: none;}
.ͼ1 .cm-lineWrapping {white-space: pre-wrap; white-space: break-spaces; word-break: break-word; overflow-wrap: anywhere; flex-shrink: 1;}
.ͼ2 .cm-content {caret-color: black;}
.ͼ3 .cm-content {caret-color: white;}
.ͼ1 .cm-line {display: block; padding: 0 2px 0 6px;}
.ͼ1 .cm-layer > * {position: absolute;}
.ͼ1 .cm-layer {position: absolute; left: 0; top: 0; contain: size style;}
.ͼ2 .cm-selectionBackground {background: #d9d9d9;}
.ͼ3 .cm-selectionBackground {background: #222;}
.ͼ2.cm-focused .cm-selectionBackground {background: #d7d4f0;}
.ͼ3.cm-focused .cm-selectionBackground {background: #233;}
.ͼ1 .cm-cursorLayer {pointer-events: none;}
.ͼ1.cm-focused .cm-cursorLayer {animation: steps(1) cm-blink 1.2s infinite;}
@keyframes cm-blink {50% {opacity: 0;}}
@keyframes cm-blink2 {50% {opacity: 0;}}
.ͼ1 .cm-cursor, .ͼ1 .cm-dropCursor {border-left: 1.2px solid black; margin-left: -0.6px; pointer-events: none;}
.ͼ1 .cm-cursor {display: none;}
.ͼ3 .cm-cursor {border-left-color: #444;}
.ͼ1 .cm-dropCursor {position: absolute;}
.ͼ1.cm-focused .cm-cursor {display: block;}
.ͼ2 .cm-activeLine {background-color: #cceeff44;}
.ͼ3 .cm-activeLine {background-color: #99eeff33;}
.ͼ2 .cm-specialChar {color: red;}
.ͼ3 .cm-specialChar {color: #f78;}
.ͼ1 .cm-gutters {flex-shrink: 0; display: flex; height: 100%; box-sizing: border-box; left: 0; z-index: 200;}
.ͼ2 .cm-gutters {background-color: #f5f5f5; color: #6c6c6c; border-right: 1px solid #ddd;}
.ͼ3 .cm-gutters {background-color: #333338; color: #ccc;}
.ͼ1 .cm-gutter {display: flex !important; flex-direction: column; flex-shrink: 0; box-sizing: border-box; min-height: 100%; overflow: hidden;}
.ͼ1 .cm-gutterElement {box-sizing: border-box;}
.ͼ1 .cm-lineNumbers .cm-gutterElement {padding: 0 3px 0 5px; min-width: 20px; text-align: right; white-space: nowrap;}
.ͼ2 .cm-activeLineGutter {background-color: #e2f2ff;}
.ͼ3 .cm-activeLineGutter {background-color: #222227;}
.ͼ1 .cm-panels {box-sizing: border-box; position: sticky; left: 0; right: 0;}
.ͼ2 .cm-panels {background-color: #f5f5f5; color: black;}
.ͼ2 .cm-panels-top {border-bottom: 1px solid #ddd;}
.ͼ2 .cm-panels-bottom {border-top: 1px solid #ddd;}
.ͼ3 .cm-panels {background-color: #333338; color: white;}
.ͼ1 .cm-tab {display: inline-block; overflow: hidden; vertical-align: bottom;}
.ͼ1 .cm-widgetBuffer {vertical-align: text-top; height: 1em; width: 0; display: inline;}
.ͼ1 .cm-placeholder {color: #888; display: inline-block; vertical-align: top;}
.ͼ1 .cm-highlightSpace:before {content: attr(data-display); position: absolute; pointer-events: none; color: #888;}
.ͼ1 .cm-highlightTab {background-image: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" width="200" height="20"><path stroke="%23888" stroke-width="1" fill="none" d="M1 10H196L190 5M190 15L196 10M197 4L197 16"/></svg>'); background-size: auto 100%; background-position: right 90%; background-repeat: no-repeat;}
.ͼ1 .cm-trailingSpace {background-color: #ff332255;}
.ͼ1 .cm-button {vertical-align: middle; color: inherit; font-size: 70%; padding: .2em 1em; border-radius: 1px;}
.ͼ2 .cm-button:active {background-image: linear-gradient(#b4b4b4, #d0d3d6);}
.ͼ2 .cm-button {background-image: linear-gradient(#eff1f5, #d9d9df); border: 1px solid #888;}
.ͼ3 .cm-button:active {background-image: linear-gradient(#111, #333);}
.ͼ3 .cm-button {background-image: linear-gradient(#393939, #111); border: 1px solid #888;}
.ͼ1 .cm-textfield {vertical-align: middle; color: inherit; font-size: 70%; border: 1px solid silver; padding: .2em .5em;}
.ͼ2 .cm-textfield {background-color: white;}
.ͼ3 .cm-textfield {border: 1px solid #555; background-color: inherit;}
.ͼ1 .cm-tooltip.cm-tooltip-autocomplete > ul > li, .ͼ1 .cm-tooltip.cm-tooltip-autocomplete > ul > completion-section {padding: 1px 3px; line-height: 1.2;}
.ͼ1 .cm-tooltip.cm-tooltip-autocomplete > ul > li {overflow-x: hidden; text-overflow: ellipsis; cursor: pointer;}
.ͼ1 .cm-tooltip.cm-tooltip-autocomplete > ul > completion-section {display: list-item; border-bottom: 1px solid silver; padding-left: 0.5em; opacity: 0.7;}
.ͼ1 .cm-tooltip.cm-tooltip-autocomplete > ul {font-family: monospace; white-space: nowrap; overflow: hidden auto; max-width: 700px; max-width: min(700px, 95vw); min-width: 250px; max-height: 10em; height: 100%; list-style: none; margin: 0; padding: 0;}
.ͼ2 .cm-tooltip-autocomplete ul li[aria-selected] {background: #17c; color: white;}
.ͼ2 .cm-tooltip-autocomplete-disabled ul li[aria-selected] {background: #777;}
.ͼ3 .cm-tooltip-autocomplete ul li[aria-selected] {background: #347; color: white;}
.ͼ3 .cm-tooltip-autocomplete-disabled ul li[aria-selected] {background: #444;}
.ͼ1 .cm-completionListIncompleteTop:before, .ͼ1 .cm-completionListIncompleteBottom:after {content: "···"; opacity: 0.5; display: block; text-align: center;}
.ͼ1 .cm-tooltip.cm-completionInfo {position: absolute; padding: 3px 9px; width: max-content; max-width: 400px; box-sizing: border-box;}
.ͼ1 .cm-completionInfo.cm-completionInfo-left {right: 100%;}
.ͼ1 .cm-completionInfo.cm-completionInfo-right {left: 100%;}
.ͼ1 .cm-completionInfo.cm-completionInfo-left-narrow {right: 30px;}
.ͼ1 .cm-completionInfo.cm-completionInfo-right-narrow {left: 30px;}
.ͼ2 .cm-snippetField {background-color: #00000022;}
.ͼ3 .cm-snippetField {background-color: #ffffff22;}
.ͼ1 .cm-snippetFieldPosition {vertical-align: text-top; width: 0; height: 1.15em; display: inline-block; margin: 0 -0.7px -.7em; border-left: 1.4px dotted #888;}
.ͼ1 .cm-completionMatchedText {text-decoration: underline;}
.ͼ1 .cm-completionDetail {margin-left: 0.5em; font-style: italic;}
.ͼ1 .cm-completionIcon {font-size: 90%; width: .8em; display: inline-block; text-align: center; padding-right: .6em; opacity: 0.6; box-sizing: content-box;}
.ͼ1 .cm-completionIcon-function:after, .ͼ1 .cm-completionIcon-method:after {content: 'ƒ';}
.ͼ1 .cm-completionIcon-class:after {content: '○';}
.ͼ1 .cm-completionIcon-interface:after {content: '◌';}
.ͼ1 .cm-completionIcon-variable:after {content: '𝑥';}
.ͼ1 .cm-completionIcon-constant:after {content: '𝐶';}
.ͼ1 .cm-completionIcon-type:after {content: '𝑡';}
.ͼ1 .cm-completionIcon-enum:after {content: '∪';}
.ͼ1 .cm-completionIcon-property:after {content: '□';}
.ͼ1 .cm-completionIcon-keyword:after {content: '🔑︎';}
.ͼ1 .cm-completionIcon-namespace:after {content: '▢';}
.ͼ1 .cm-completionIcon-text:after {content: 'abc'; font-size: 50%; vertical-align: middle;}
.ͼ1 .cm-tooltip {z-index: 100; box-sizing: border-box;}
.ͼ2 .cm-tooltip {border: 1px solid #bbb; background-color: #f5f5f5;}
.ͼ2 .cm-tooltip-section:not(:first-child) {border-top: 1px solid #bbb;}
.ͼ3 .cm-tooltip {background-color: #333338; color: white;}
.ͼ1 .cm-tooltip-arrow:before, .ͼ1 .cm-tooltip-arrow:after {content: ''; position: absolute; width: 0; height: 0; border-left: 7px solid transparent; border-right: 7px solid transparent;}
.ͼ1 .cm-tooltip-above .cm-tooltip-arrow:before {border-top: 7px solid #bbb;}
.ͼ1 .cm-tooltip-above .cm-tooltip-arrow:after {border-top: 7px solid #f5f5f5; bottom: 1px;}
.ͼ1 .cm-tooltip-above .cm-tooltip-arrow {bottom: -7px;}
.ͼ1 .cm-tooltip-below .cm-tooltip-arrow:before {border-bottom: 7px solid #bbb;}
.ͼ1 .cm-tooltip-below .cm-tooltip-arrow:after {border-bottom: 7px solid #f5f5f5; top: 1px;}
.ͼ1 .cm-tooltip-below .cm-tooltip-arrow {top: -7px;}
.ͼ1 .cm-tooltip-arrow {height: 7px; width: 14px; position: absolute; z-index: -1; overflow: hidden;}
.ͼ3 .cm-tooltip .cm-tooltip-arrow:before {border-top-color: #333338; border-bottom-color: #333338;}
.ͼ3 .cm-tooltip .cm-tooltip-arrow:after {border-top-color: transparent; border-bottom-color: transparent;}
.ͼ1 .cm-tooltip.cm-tooltip-autocomplete {border: 0; background-color: transparent;}
.ͼ1 .cm-tooltip.cm-tooltip-autocomplete > ul {font-family: SFMono-Regular, Consolas, 'Liberation Mono', Menlo, monospace; font-size: 12px; background-color: var(--bgColor-default, var(--color-canvas-default)); border: 1px solid var(--borderColor-default, var(--color-border-default)); border-radius: var(--borderRadius-medium); box-shadow: var(--shadow-resting-medium, var(--color-shadow-medium)); min-width: auto;}
.ͼ1 .cm-tooltip.cm-tooltip-autocomplete li[role="option"] {padding: 2px 8px; margin: 0; color: var(--fgColor-default, var(--color-fg-default)); white-space: pre;}
.ͼ1 .cm-tooltip.cm-tooltip-autocomplete li[role="option"]:first-child {border-top-left-radius: var(--borderRadius-medium); border-top-right-radius: var(--borderRadius-medium);}
.ͼ1 .cm-tooltip.cm-tooltip-autocomplete li[role="option"]:last-child {border-bottom-left-radius: var(--borderRadius-medium); border-bottom-right-radius: var(--borderRadius-medium);}
.ͼ1 .cm-tooltip.cm-tooltip-autocomplete ul li[aria-selected], .ͼ1 .cm-tooltip.cm-tooltip-autocomplete ul li[aria-selected] .cm-completionDetail {color: var(--fgColor-onEmphasis, var(--color-fg-on-emphasis)); background: var(--bgColor-accent-emphasis, var(--color-accent-emphasis));}
.ͼ1 .cm-completionDetail {padding-left: 8px; color: var(--fgColor-muted, var(--color-fg-muted)); font-size: var(--fontSize-small); font-style: normal;}
.ͼ1 .cm-panel.cm-search [name=close] {position: absolute; top: 0; right: 4px; background-color: inherit; border: none; font: inherit; padding: 0; margin: 0;}
.ͼ1 .cm-panel.cm-search input, .ͼ1 .cm-panel.cm-search button, .ͼ1 .cm-panel.cm-search label {margin: .2em .6em .2em 0;}
.ͼ1 .cm-panel.cm-search input[type=checkbox] {margin-right: .2em;}
.ͼ1 .cm-panel.cm-search label {font-size: 80%; white-space: pre;}
.ͼ1 .cm-panel.cm-search {padding: 2px 6px 4px; position: relative;}
.ͼ2 .cm-searchMatch {background-color: #ffff0054;}
.ͼ3 .cm-searchMatch {background-color: #00ffff8a;}
.ͼ2 .cm-searchMatch-selected {background-color: #ff6a0054;}
.ͼ3 .cm-searchMatch-selected {background-color: #ff00ff8a;}
.ͼ1.cm-focused .cm-matchingBracket {background-color: #328c8252;}
.ͼ1.cm-focused .cm-nonmatchingBracket {background-color: #bb555544;}
.ͼ6 {color: var(--codeMirror-syntax-fgColor-keyword, var(--color-codemirror-syntax-keyword));}
.ͼ7 {color: var(--codeMirror-syntax-fgColor-comment, var(--color-codemirror-syntax-comment));}
.ͼ8 {color: var(--codeMirror-matchingBracket-fgColor, var(--color-codemirror-matchingbracket-text));}
.ͼ9 {color: var(--codeMirror-syntax-fgColor-string, var(--color-codemirror-syntax-string));}
.ͼa {color: var(--codeMirror-syntax-fgColor-constant, var(--color-codemirror-syntax-constant));}
.ͼb {color: var(--codeMirror-syntax-fgColor-constant, var(--color-codemirror-syntax-constant));}
.ͼc {color: var(--codeMirror-syntax-fgColor-entity, var(--color-codemirror-syntax-entity));}
.ͼd {color: var(--codeMirror-syntax-fgColor-variable, var(--color-codemirror-syntax-variable));}
.ͼe {color: inherit;}
.ͼf {font-weight: bold; color: inherit !important;}
.ͼg {color: var(--codeMirror-syntax-fgColor-comment, var(--color-codemirror-syntax-comment));}
.ͼh {text-decoration: underline;}
.ͼi {font-style: italic;}
.ͼj {font-weight: bold;}
.ͼk {text-decoration: line-through;}
.ͼ5 {background: var(--codeMirror-bgColor, var(--color-codemirror-bg)); color: var(--codeMirror-fgColor, var(--color-codemirror-text)); cursor: text;}
.ͼ5 .cm-gutters {background: var(--codeMirror-gutters-bgColor, var(--color-codemirror-gutters-bg)); border-right-width: 0;}
.ͼ5 .cm-lineNumbers .cm-gutterElement {color: var(--codeMirror-lineNumber-fgColor, var(--color-codemirror-linenumber-text)); font-family: var(--fontStack-monospace); font-size: var(--codeMirror-gutter-fontSize, var(--codeMirror-content-fontSize, 12px)); line-height: 20px; padding: 0 16px 0 16px;}
.ͼ5 .cm-content {caret-color: var(--codeMirror-cursor-fgColor, var(--color-codemirror-cursor)); font-family: var(--fontStack-monospace); font-size: var(--codeMirror-content-fontSize, 12px); background: var(--codeMirror-lines-bgColor, var(--color-codemirror-lines-bg)); line-height: 20px; padding-top: 8px;}
.ͼ5.cm-focused .cm-selectionBackground, .ͼ5 .cm-selectionBackground, .ͼ5 .cm-content ::selection {background-color: var(--codeMirror-selection-bgColor, var(--color-codemirror-selection-bg, #d7d4f0));}
.ͼ5.cm-focused {outline: none;}
.ͼ5.hide-help-until-focus.cm-focused .cm-panels-bottom {display: block;}
.ͼ5.hide-help-until-focus .cm-panels-bottom {display: none;}
.ͼ5.hide-help .cm-panels-top {display: none; position: absolute;}
.ͼ5 .cm-content ::-moz-selection {background-color: var(--codeMirror-selection-bgColor, var(--color-codemirror-selection-bg, #d7d4f0));}
.ͼ5 .cm-activeLine {background-color: var(--codeMirror-activeline-bgColor, var(--color-codemirror-activeline-bg));}
.ͼ5 .cm-line {padding-left: 16px;}
.ͼ5 .cm-help-panel {background: var(--bgColor-muted, var(--color-canvas-subtle)); padding: 7px 10px; margin: 0; font-size: 13px; line-height: 16px; color: var(--fgColor-muted, var(--color-fg-muted)); cursor: default;}
.ͼ5 .cm-panels-bottom {border-top: var(--borderWidth-thin, 1px) solid var(--borderColor-default, var(--color-border-default)); background: none;}
.js-upload-markdown-image .ͼ5 .cm-panels-bottom {bottom: 30px !important;}
.ͼ5 .cm-panel.cm-search {background: var(--bgColor-muted, var(--color-canvas-subtle)); padding: 8px; font-size: 16px;}
.ͼ5 .cm-panel.cm-search > button {border-radius: 6px; padding: 4px 8px; background: var(--codeMirror-bgColor, var(--color-codemirror-bg)); color: var(--button-default-fgColor-rest, var(--color-btn-text)); border: 1px solid var(--button-default-borderColor-rest, var(--color-btn-border)); text-transform: capitalize;}
.ͼ5 .cm-panel.cm-search > label {color: var(--fgColor-default, var(--color-fg-default)); text-transform: capitalize; font-size: 12px;}
.ͼ5 .cm-panel.cm-search > input {border-radius: 6px; padding: 4px 8px; background: var(--bgColor-default, var(--color-canvas-default)); color: var(--fgColor-default, var(--color-fg-default)); border: 1px solid var(--borderColor-default, var(--color-border-default)); font-size: 12px;}
.ͼ5 .cm-panel.cm-search > button[name="close"] {padding: 4px;}
.ͼ5 .cm-panels-top {border-bottom: var(--borderWidth-thin, 1px) solid var(--color-border-default); background: none;}
.ͼ5 .cm-panel.cm-search input, .ͼ5 .cm-panel.cm-search button, .ͼ5 .cm-panel.cm-search label {margin-right: 8px; margin-bottom: 4px; margin-top: 4px; margin-left: 0;}
.ͼ5 .cm-lintRange {cursor: help; background-image: none !important;}
.ͼ5 .cm-placeholder {height: 1em; color: var(--fgColor-muted);}
.ͼ5.custom-tooltips .cm-tooltip {border: none !important; background-color: transparent !important;}
.ͼ5.custom-tooltips .cm-diagnostic {padding: 0; margin-left: 0 !important; border-left: none !important; white-space: unset;}
.ͼ4 {height: 85vh; min-height: ; width: 100%;}
</style><style type="text/css">.turbo-progress-bar {
  position: fixed;
  display: block;
  top: 0;
  left: 0;
  height: 3px;
  background: #0076ff;
  z-index: 2147483647;
  transition:
    width 300ms ease-out,
    opacity 150ms 150ms ease-in;
  transform: translate3d(0, 0, 0);
}
</style>
    
  
  
  
  
  
  

  

  <link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/light-74231a1f3bbb.css"><link data-color-theme="light_high_contrast" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/light_high_contrast-83beb16e0ecf.css"><link data-color-theme="light_colorblind" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/light_colorblind-f91b0f603451.css"><link data-color-theme="light_colorblind_high_contrast" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/light_colorblind_high_contrast-5aebfa54b215.css"><link data-color-theme="light_tritanopia" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/light_tritanopia-6e122dab64fc.css"><link data-color-theme="light_tritanopia_high_contrast" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/light_tritanopia_high_contrast-b32664e28b79.css"><link data-color-theme="dark" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark-8a995f0bacd4.css"><link data-color-theme="dark_high_contrast" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark_high_contrast-9ac301c3ebe5.css"><link data-color-theme="dark_colorblind" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark_colorblind-cd826e8636dc.css"><link data-color-theme="dark_colorblind_high_contrast" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark_colorblind_high_contrast-131d53fe187c.css"><link data-color-theme="dark_tritanopia" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark_tritanopia-18119e682df0.css"><link data-color-theme="dark_tritanopia_high_contrast" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark_tritanopia_high_contrast-63c0358957ba.css"><link data-color-theme="dark_dimmed" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark_dimmed-f37fb7684b1f.css"><link data-color-theme="dark_dimmed_high_contrast" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark_dimmed_high_contrast-8f371c75debd.css">

    <link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/primer-primitives-225433424a87.css">
    <link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/primer-b8b91660c29d.css">
    <link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/global-67417a636023.css">
    <link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/github-86c50480e726.css">
  <link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/repository-4fce88777fa8.css">
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/code-177d21388df8.css">

  


  <script type="application/json" id="client-env">{"locale":"en","featureFlags":["alternate_user_config_repo","api_insights_show_missing_data_banner","billing_sku_level_budgets","codespaces_prebuild_region_target_update","contentful_lp_flex_features_actions","contentful_lp_flex_features_code_review","contentful_lp_flex_features_code_search","contentful_lp_flex_features_codespaces","contentful_lp_flex_features_discussions","contentful_lp_flex_features_issues","contentful_lp_footnotes","copilot_chat_attach_images","copilot_chat_attachments","copilot_chat_custom_instructions","copilot_chat_interview_survey","copilot_chat_opening_thread_switch","copilot_chat_repo_custom_instructions_preview","copilot_chat_vision_in_claude","copilot_chat_wholearea_dd","copilot_default_4_1_preview","copilot_dotcom_chat_file_upload","copilot_duplicate_thread","copilot_free_to_paid_telem","copilot_immersive_issue_preview","copilot_immersive_rename_thread_scoped_issue","copilot_new_immersive_references_ui","copilot_no_floating_button","copilot_read_shared_conversation","copilot_share_active_subthread","copilot_share_forbidden_error","copilot_swe_agent_stop_sessions","copilot_task_oriented_assistive_prompts","copilot_topics_as_references","copilot_ui_refs","copilot_use_capi_default_model","direct_to_salesforce","dotcom_chat_client_side_skills","fetch_nonce_headers","ghost_pilot_confidence_truncation_25","ghost_pilot_confidence_truncation_40","github_models_o3_mini_streaming","insert_before_patch","issues_dashboard_no_redirects","issues_react_blur_item_picker_on_close","issues_react_create_milestone","issues_react_dashboard_save_query_refresh","issues_react_include_bots_in_pickers","issues_react_prohibit_title_fallback","issues_react_remove_placeholders","lifecycle_label_name_updates","link_contact_sales_swp_marketo","marketing_pages_search_explore_provider","memex_mwl_filter_field_delimiter","memex_roadmap_drag_style","nonreporting_relay_graphql_status_codes","primer_react_css_modules_ga","primer_react_select_panel_with_modern_action_list","remove_child_patch","repository_suggester_elastic_search","sample_network_conn_type","site_proxima_australia_update","site_proxima_usa_update","swp_enterprise_contact_form","use_paginated_org_picker_cost_center_form","use_paginated_repo_picker_cost_center_form","viewscreen_sandbox"],"login":"dhashvanth21"}</script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/wp-runtime-ad5938acbdf4.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_oddbird_popover-polyfill_dist_popover-fn_js-a8c266e5f126.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_mini-throttle_dist_index_js-node_modules_stacktrace-parser_dist_s-1d3d52-83b9e5876876.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_failbot_failbot_ts-05558583be72.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/environment-388ce24ed839.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_primer_behaviors_dist_esm_index_mjs-c44edfed7f0d.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_selector-observer_dist_index_esm_js-d01a0e57231b.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_relative-time-element_dist_index_js-b96cbf526995.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_auto-complete-element_dist_index_js-node_modules_github_catalyst_-8e9f78-55b81350dfdb.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_text-expander-element_dist_index_js-1f6d08804998.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_filter-input-element_dist_index_js-node_modules_github_remote-inp-d8c643-8f1926754a8d.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_markdown-toolbar-element_dist_index_js-c66bd68a4bd8.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_mini-throttle_dist_index_js-node_modules_github_combobox-nav_dist-97536f-dfe529d68ce6.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_file-attachment-element_dist_index_js-node_modules_primer_view-co-63644b-8ff09ec17bfc.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/github-elements-2a8f4c0f6796.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/element-registry-db730b446f70.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_braintree_browser-detection_dist_browser-detection_js-node_modules_githu-bb80ec-2562029d640d.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_lit-html_lit-html_js-c4df7c1117d4.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_morphdom_dist_morphdom-esm_js-300e8e4e0414.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_fzy_js_index_js-node_modules_github_paste-markdown_dist_index_js-63a26702fa42.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_turbo_dist_turbo_es2017-esm_js-5271e9c887b5.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_remote-form_dist_index_js-node_modules_delegated-events_dist_inde-893f9f-3f95b0ff87ec.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_color-convert_index_js-1a149db8dc99.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_quote-selection_dist_index_js-node_modules_github_session-resume_-c1aa61-fcfd98d65693.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_updatable-content_updatable-content_ts-94844e3a0328.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/app_assets_modules_github_behaviors_task-list_ts-app_assets_modules_github_sso_ts-ui_packages-900dde-0f4d4815e497.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/app_assets_modules_github_sticky-scroll-into-view_ts-c4ec66fdacae.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/app_assets_modules_github_behaviors_ajax-error_ts-app_assets_modules_github_behaviors_include-d0d0a6-4ec1f4ce6c03.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/app_assets_modules_github_behaviors_commenting_edit_ts-app_assets_modules_github_behaviors_ht-83c235-c29d73bf4798.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/behaviors-28d108d85ae7.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_delegated-events_dist_index_js-node_modules_github_catalyst_lib_index_js-ea8eaa-99d4543be0a1.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/notifications-global-a37edf3c60b9.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_mini-throttle_dist_index_js-node_modules_virtualized-list_es_inde-5cfb7e-bb1cda3be5d8.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_remote-form_dist_index_js-node_modules_delegated-events_dist_inde-70450e-49f5490071bd.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/app_assets_modules_github_ref-selector_ts-21f53f51c151.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/codespaces-7391d956861f.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_filter-input-element_dist_index_js-node_modules_github_remote-inp-3eebbd-0b00a75e597d.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_mini-throttle_dist_decorators_js-node_modules_delegated-events_di-e161aa-49841a06612b.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_file-attachment-element_dist_index_js-node_modules_github_remote--3c9c82-7675fa4c404c.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/repositories-c81438e961aa.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_mini-throttle_dist_index_js-node_modules_github_catalyst_lib_inde-dbbea9-b7a14570d384.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/code-menu-52f2057a8e7d.js.download"></script>
  
  <link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/primer-react.d2117d7623cc63123645.module.css">
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/notifications-subscriptions-menu.e5e6e593370c808590a5.module.css">


  



  
  
  
  

    
  


  


    


  
  

  
  

    



  

  




    

  

    

    

      

      

    
    
    

      
  
  


      
      


      


      
      
      

        


  <meta http-equiv="x-pjax-version" content="b269c56ef8006e74940905426f423850ba412c31564cccb2aa411c1da8ad3fe9" data-turbo-track="reload">
  <meta http-equiv="x-pjax-csp-version" content="352e51c42d5f5727a7c545752bf34d1f83f40219e7036c6959817149a51651bc" data-turbo-track="reload">
  <meta http-equiv="x-pjax-css-version" content="4ebb44a95a488b0e8784b5704ba7499677af7a8cb1a7b3ee134cb797826a67f2" data-turbo-track="reload">
  <meta http-equiv="x-pjax-js-version" content="1466b8415281fc3b12960939d134f6e4668aabfa27ec5ad20a07cf11e6ab7fba" data-turbo-track="reload">

  

      
  

  



      


    


  

  

  

  
  
  




  
  

  

  <style data-styled="active" data-styled-version="5.3.11"></style><style id="ms-consent-banner-main-styles">.w8hcgFksdo30C8w-bygqu{color:#000}.ydkKdaztSS0AeHWIeIHsQ a{color:#0067B8}.erL690_8JwUW-R4bJRcfl{background-color:#EBEBEB;border:none;color:#000}.erL690_8JwUW-R4bJRcfl:enabled:hover{color:#000;background-color:#DBDBDB;box-shadow:0px 4px 10px rgba(0,0,0,0.25);border:none}.erL690_8JwUW-R4bJRcfl:enabled:focus{background-color:#DBDBDB;box-shadow:0px 4px 10px rgba(0,0,0,0.25);border:2px solid #000}.erL690_8JwUW-R4bJRcfl:disabled{opacity:1;color:rgba(0,0,0,0.2);background-color:rgba(0,0,0,0.2);border:none}._1zNQOqxpBFSokeCLGi_hGr{border:none;background-color:#0067B8;color:#fff}._1zNQOqxpBFSokeCLGi_hGr:enabled:hover{color:#fff;background-color:#0067B8;box-shadow:0px 4px 10px rgba(0,0,0,0.25);border:none}._1zNQOqxpBFSokeCLGi_hGr:enabled:focus{background-color:#0067B8;box-shadow:0px 4px 10px rgba(0,0,0,0.25);border:2px solid #000}._1zNQOqxpBFSokeCLGi_hGr:disabled{opacity:1;color:rgba(0,0,0,0.2);background-color:rgba(0,120,215,0.2);border:none}._23tra1HsiiP6cT-Cka-ycB{position:relative;display:flex;z-index:9999;width:100%;background-color:#F2F2F2;justify-content:space-between;text-align:left}div[dir="rtl"]._23tra1HsiiP6cT-Cka-ycB{text-align:right}._1Upc2NjY8AlDn177YoVj0y{margin:0;padding-left:5%;padding-top:8px;padding-bottom:8px}div[dir="rtl"] ._1Upc2NjY8AlDn177YoVj0y{margin:0;padding:8px 5% 8px 0;float:none}._23tra1HsiiP6cT-Cka-ycB svg{fill:none;max-width:none;max-height:none}._1V_hlU-7jdtPiooHMu89BB{display:table-cell;padding:12px;width:24px;height:24px;font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:normal;font-size:24px;line-height:0}.f6QKJD7fhSbnJLarTL-W-{display:table-cell;vertical-align:middle;padding:0;font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:normal;font-size:13px;line-height:16px}.f6QKJD7fhSbnJLarTL-W- a{text-decoration:underline}._2j0fmugLb1FgYz6KPuB91w{display:inline-block;margin-left:5%;margin-right:5%;min-width:40%;min-width:calc((150px + 3 * 4px) * 2 + 150px);min-width:-webkit-fit-content;min-width:-moz-fit-content;min-width:fit-content;align-self:center;position:relative}._1XuCi2WhiqeWRUVp3pnFG3{margin:4px;padding:5px;min-width:150px;min-height:36px;vertical-align:top;cursor:pointer;font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:normal;font-size:15px;line-height:20px;text-align:center}._1XuCi2WhiqeWRUVp3pnFG3:focus{box-sizing:border-box}._1XuCi2WhiqeWRUVp3pnFG3:disabled{cursor:not-allowed}._2bvsb3ubApyZ0UGoQA9O9T{display:block;position:fixed;z-index:10000;top:0;left:0;width:100%;height:100%;background-color:rgba(255,255,255,0.6);overflow:auto;text-align:left}div[dir="rtl"]._2bvsb3ubApyZ0UGoQA9O9T{text-align:right}div[dir="rtl"] ._2bvsb3ubApyZ0UGoQA9O9T{left:auto;right:0}.AFsJE948muYyzCMktdzuk{position:relative;top:8%;margin-bottom:40px;margin-left:auto;margin-right:auto;box-sizing:border-box;width:640px;background-color:#fff;border:1px solid #0067B8}._3kWyBRbW_dgnMiEyx06Fu4{float:right;z-index:1;margin:2px;padding:12px;border:none;cursor:pointer;font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:normal;font-size:13px;line-height:13px;display:flex;align-items:center;text-align:center;color:#666;background-color:#fff}div[dir="rtl"] ._3kWyBRbW_dgnMiEyx06Fu4{margin:2px;padding:12px;float:left}.uCYvKvHXrhjNgflv1VqdD{position:static;margin-top:36px;margin-left:36px;margin-right:36px}._17pX1m9O_W--iZbDt3Ta5r{margin-top:0;margin-bottom:12px;font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:600;font-size:20px;line-height:24px;text-transform:none}._1kBkHQ1V1wu3kl-YcLgUr6{height:446px;overflow:auto}._20_nXDf6uFs9Q6wxRXG-I-{margin-top:0;font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:normal;font-size:15px;line-height:20px}._20_nXDf6uFs9Q6wxRXG-I- a{text-decoration:underline}dl._2a0NH_GDQEQe5Ynfo7suVH{margin-top:36px;margin-bottom:0;padding:0;list-style:none;text-transform:none}dt._3j_LCPv7fyXv3A8FIXVwZ4{margin-top:20px;float:none;font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:600;font-size:18px;line-height:24px;list-style:none}.k-vxTGFbdq1aOZB2HHpjh{margin:0;padding:0;border:none}._2Bucyy75c_ogoU1g-liB5R{margin:0;padding:0;border-bottom:none;font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:600;font-size:18px;line-height:24px;text-transform:none}._63gwfzV8dclrsl2cfd90r{display:inline-block;margin-top:0;margin-bottom:13px;font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:normal;font-size:15px;line-height:20px}._1l8wM_4mRYGz3Iu7l3BZR7{display:block}._2UE03QS02aZGkslegN_F-i{display:inline-block;position:relative;left:5px;margin-bottom:13px;margin-right:34px;padding:3px}div[dir="rtl"] ._2UE03QS02aZGkslegN_F-i{margin:0 0 13px 34px;padding:3px;float:none}div[dir="rtl"] ._2UE03QS02aZGkslegN_F-i{left:auto;right:5px}._23tra1HsiiP6cT-Cka-ycB *::before,._2bvsb3ubApyZ0UGoQA9O9T *::before,._23tra1HsiiP6cT-Cka-ycB *::after,._2bvsb3ubApyZ0UGoQA9O9T *::after{box-sizing:inherit}._1HSFn0HzGo6w4ADApV8-c4{outline:2px solid rgba(0,0,0,0.8)}input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2{display:inline-block;position:relative;margin-top:0;margin-left:0;margin-right:0;height:0;width:0;border-radius:0;cursor:pointer;outline:none;box-sizing:border-box;-webkit-appearance:none;-moz-appearance:none;appearance:none}input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2+label::before{display:block;position:absolute;top:5px;left:3px;height:19px;width:19px;content:"";border-radius:50%;border:1px solid #000;background-color:#fff}div[dir="rtl"] input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2+label::before{left:auto;right:3px}input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:not(:disabled)+label:hover::before{border:1px solid #0067B8}input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:not(:disabled)+label:hover::after{display:block;position:absolute;top:10px;left:8px;height:9px;width:9px;content:"";border-radius:50%;background-color:rgba(0,0,0,0.8)}div[dir="rtl"] input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:not(:disabled)+label:hover::after{left:auto;right:8px}input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:not(:disabled)+label:focus::before{border:1px solid #0067B8}input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:not(:disabled)+label:focus::after{display:block;position:absolute;top:10px;left:8px;height:9px;width:9px;content:"";border-radius:50%;background-color:#000}div[dir="rtl"] input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:not(:disabled)+label:focus::after{left:auto;right:8px}input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:checked+label::after{display:block;position:absolute;top:10px;left:8px;height:9px;width:9px;content:"";border-radius:50%;background-color:#000}div[dir="rtl"] input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:checked+label::after{left:auto;right:8px}input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:disabled+label{cursor:not-allowed}input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:disabled+label::before{border:1px solid rgba(0,0,0,0.2);background-color:rgba(0,0,0,0.2)}._3RJzeL3l9Rl_lAQEm6VwdX{display:block;position:static;float:right;margin-top:0;margin-bottom:0;margin-left:19px;margin-right:0;padding-top:0;padding-bottom:0;padding-left:8px;padding-right:0;width:80%;width:calc(100% - 19px);font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:normal;font-size:15px;line-height:20px;text-transform:none;cursor:pointer;box-sizing:border-box}div[dir="rtl"] ._3RJzeL3l9Rl_lAQEm6VwdX{margin:0 19px 0 0;padding:0 8px 0 0;float:left}.nohp3sIG12ZBhzcMnPala{margin-top:20px;margin-bottom:48px}._2uhaEsmeotZ3P-M0AXo2kF{padding:0;width:278px;height:36px;cursor:pointer;font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:normal;font-size:15px;line-height:20px;text-align:center}._2uhaEsmeotZ3P-M0AXo2kF:focus{box-sizing:border-box}._2uhaEsmeotZ3P-M0AXo2kF:disabled{cursor:not-allowed}._3tOu1FJ59c_xz_PmI1lKV5{float:right;padding:0;width:278px;height:36px;cursor:pointer;font-family:Segoe UI, SegoeUI, Arial, sans-serif;font-style:normal;font-weight:normal;font-size:15px;line-height:20px;text-align:center}._3tOu1FJ59c_xz_PmI1lKV5:focus{box-sizing:border-box}._3tOu1FJ59c_xz_PmI1lKV5:disabled{cursor:not-allowed}div[dir="rtl"] ._3tOu1FJ59c_xz_PmI1lKV5{margin:0;padding:0;float:left}@media only screen and (max-width: 768px){._2j0fmugLb1FgYz6KPuB91w,._1Upc2NjY8AlDn177YoVj0y{padding-top:8px;padding-bottom:12px;padding-left:3.75%;padding-right:3.75%;margin:0;width:92.5%}._23tra1HsiiP6cT-Cka-ycB{display:block}._1XuCi2WhiqeWRUVp3pnFG3{margin-bottom:8px;margin-left:0;margin-right:0;width:100%}._2bvsb3ubApyZ0UGoQA9O9T{overflow:hidden}.AFsJE948muYyzCMktdzuk{top:1.8%;width:93.33%;height:96.4%;overflow:hidden}.uCYvKvHXrhjNgflv1VqdD{margin-top:24px;margin-left:24px;margin-right:24px;height:100%}._1kBkHQ1V1wu3kl-YcLgUr6{height:62%;height:calc(100% - 188px);min-height:50%}._2uhaEsmeotZ3P-M0AXo2kF{width:100%}._3tOu1FJ59c_xz_PmI1lKV5{margin-bottom:12px;margin-left:0;width:100%}div[dir="rtl"] ._3tOu1FJ59c_xz_PmI1lKV5{margin:0 0 12px 0;padding:0;float:none}}@media only screen and (max-width: 768px) and (orientation: landscape), only screen and (max-height: 260px), only screen and (max-width: 340px){.AFsJE948muYyzCMktdzuk{overflow:auto}}@media only screen and (max-height: 260px), only screen and (max-width: 340px){._1XuCi2WhiqeWRUVp3pnFG3{min-width:0}._3kWyBRbW_dgnMiEyx06Fu4{padding:3%}.uCYvKvHXrhjNgflv1VqdD{margin-top:3%;margin-left:3%;margin-right:3%}._17pX1m9O_W--iZbDt3Ta5r{margin-bottom:3%}._1kBkHQ1V1wu3kl-YcLgUr6{height:calc(79% - 64px)}.nohp3sIG12ZBhzcMnPala{margin-top:5%;margin-bottom:10%}._3tOu1FJ59c_xz_PmI1lKV5{margin-bottom:3%}div[dir="rtl"] ._3tOu1FJ59c_xz_PmI1lKV5{margin:0 0 3% 0;padding:0;float:none}}
</style><style type="text/css" id="ms-consent-banner-theme-styles">._23tra1HsiiP6cT-Cka-ycB {
            background-color: #24292f !important;
        }.w8hcgFksdo30C8w-bygqu {
            color: #ffffff !important;
        }.ydkKdaztSS0AeHWIeIHsQ a {
            color: #d8b9ff !important;
        }._2bvsb3ubApyZ0UGoQA9O9T {
            background-color: rgba(23, 23, 23, 0.8) !important;
        }.AFsJE948muYyzCMktdzuk {
            background-color: #24292f !important;
            border: 1px solid #d8b9ff !important;
        }._3kWyBRbW_dgnMiEyx06Fu4 {
            color: #d8b9ff !important;
            background-color: #24292f !important;
        }._1zNQOqxpBFSokeCLGi_hGr {
            border: 1px solid #ffffff !important;
            background-color: #ffffff !important;
            color: #1f2328 !important;
        }._1zNQOqxpBFSokeCLGi_hGr:enabled:hover {
            color: #1f2328 !important;
            background-color: #d8b9ff !important;
            box-shadow: none !important;
            border: 1px solid transparent !important;
        }._1zNQOqxpBFSokeCLGi_hGr:enabled:focus {
            background-color: #d8b9ff !important;
            box-shadow: none !important;
            border: 2px solid #ffffff !important;
        }._1zNQOqxpBFSokeCLGi_hGr:disabled {
            opacity: 0.5 !important;
            color: #1f2328 !important;
            background-color: #ffffff !important;
            border: 1px solid transparent !important;
        }.erL690_8JwUW-R4bJRcfl {
            border: 1px solid #eaeef2 !important;
            background-color: #32383f !important;
            color: #ffffff !important;
        }.erL690_8JwUW-R4bJRcfl:enabled:hover {
            color: #ffffff !important;
            background-color: #24292f !important;
            box-shadow: none !important;
            border: 1px solid #ffffff !important;
        }.erL690_8JwUW-R4bJRcfl:enabled:focus {
            background-color: #24292f !important;
            box-shadow: none !important;
            border: 2px solid #6e7781 !important;
        }.erL690_8JwUW-R4bJRcfl:disabled {
            opacity: 0.5 !important;
            color: #ffffff !important;
            background-color: #424a53 !important;
            border: 1px solid #6e7781 !important;
        }input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2 + label::before {
            border: 1px solid #d8b9ff !important;
            background-color: #24292f !important;
        }._1HSFn0HzGo6w4ADApV8-c4 {
            outline: 2px solid #ffffff !important;
        }input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:checked + label::after {
            background-color: #d8b9ff !important;
        }input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2 + label:hover::before {
            border: 1px solid #ffffff !important;
        }input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2 + label:hover::after {
            background-color: #ffffff !important;
        }input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2 + label:focus::before {
            border: 1px solid #ffffff !important;
        }input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2 + label:focus::after {
            background-color: #d8b9ff !important;
        }input[type="radio"]._1dp8Vp5m3HwAqGx8qBmFV2:disabled + label::before {
            border: 1px solid rgba(227, 227, 227, 0.2) !important;
            background-color: rgba(227, 227, 227, 0.2) !important;
        }</style><link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/repo-creation.87fdb1bc10edf8198059.module.css"><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/primer-react-cf8d019de009.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/react-core-2e45a8c586a0.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/react-lib-248ff5a58e4e.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/octicons-react-9fd6ca6872cc.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_emotion_is-prop-valid_dist_emotion-is-prop-valid_esm_js-node_modules_emo-b1c483-9589ee80fc4f.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_catalyst_lib_index_js-node_modules_primer_live-region-element_dis-b2aea6-980db0e5dd58.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_dompurify_dist_purify_es_mjs-d13e3af1f7a5.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_document-metadata_document-metadata_ts-ui_packages_history_history_ts-ui_packages-417c81-a0c3c1a41581.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_paths_index_ts-08fcbb3f0e88.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_app-uuid_app-uuid_ts-ui_packages_custom-properties-editing_hooks_use-edit-custom--84d010-0897f7a4b39d.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/repo-creation-4c0190463f69.js.download"></script><style type="text/css" id="ms-consent-banner-theme-styles"></style><link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/insights-e68c777ffec1.css"><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/forks-69fd26313c56.js.download"></script><link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/react-code-view.304141ebc07a046c05cd.module.css"><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_lodash-es__Stack_js-node_modules_lodash-es__Uint8Array_js-node_modules_l-4faaa6-bdfd153f605f.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_lodash-es_isEqual_js-d3919b3d0f3d.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_tanstack_react-query_build_modern_queryOptions_js-node_modules_react-int-52413b-8c99d3c9132c.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_focus-visible_dist_focus-visible_js-node_modules_github_hydro-analytics--e21ffd-34e19bb44764.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_ref-selector_RefSelector_tsx-07d3a848f730.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_commit-attribution_index_ts-ui_packages_commit-checks-status_index_ts-ui_packages-762eaa-12eaa372da2a.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_app-uuid_app-uuid_ts-ui_packages_repos-file-tree-view_repos-file-tree-view_ts-ui_-f1cc33-29d65b920c66.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_code-view-shared_hooks_use-canonical-object_ts-ui_packages_code-view-shared_hooks-cd3541-677c2c477dc2.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/app_assets_modules_github_blob-anchor_ts-ui_packages_code-nav_code-nav_ts-ui_packages_filter--8253c1-7a601ea5c641.js.download"></script><script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/react-code-view-8e7538824e1b.js.download"></script><script type="application/json" id="client-env">{"locale":"en","featureFlags":["alternate_user_config_repo","api_insights_show_missing_data_banner","billing_sku_level_budgets","codespaces_prebuild_region_target_update","contentful_lp_flex_features_actions","contentful_lp_flex_features_code_review","contentful_lp_flex_features_code_search","contentful_lp_flex_features_codespaces","contentful_lp_flex_features_discussions","contentful_lp_flex_features_issues","contentful_lp_footnotes","copilot_chat_attach_images","copilot_chat_attachments","copilot_chat_custom_instructions","copilot_chat_interview_survey","copilot_chat_opening_thread_switch","copilot_chat_repo_custom_instructions_preview","copilot_chat_vision_in_claude","copilot_chat_wholearea_dd","copilot_default_4_1_preview","copilot_dotcom_chat_file_upload","copilot_duplicate_thread","copilot_free_to_paid_telem","copilot_immersive_issue_preview","copilot_immersive_rename_thread_scoped_issue","copilot_new_immersive_references_ui","copilot_no_floating_button","copilot_read_shared_conversation","copilot_share_active_subthread","copilot_share_forbidden_error","copilot_swe_agent_stop_sessions","copilot_task_oriented_assistive_prompts","copilot_topics_as_references","copilot_ui_refs","copilot_use_capi_default_model","direct_to_salesforce","dotcom_chat_client_side_skills","fetch_nonce_headers","ghost_pilot_confidence_truncation_25","ghost_pilot_confidence_truncation_40","github_models_o3_mini_streaming","insert_before_patch","issues_dashboard_no_redirects","issues_react_blur_item_picker_on_close","issues_react_create_milestone","issues_react_dashboard_save_query_refresh","issues_react_include_bots_in_pickers","issues_react_prohibit_title_fallback","issues_react_remove_placeholders","lifecycle_label_name_updates","link_contact_sales_swp_marketo","marketing_pages_search_explore_provider","memex_mwl_filter_field_delimiter","memex_roadmap_drag_style","nonreporting_relay_graphql_status_codes","primer_react_css_modules_ga","primer_react_select_panel_with_modern_action_list","remove_child_patch","report_hydro_web_vitals","repository_suggester_elastic_search","sample_network_conn_type","site_proxima_australia_update","site_proxima_usa_update","swp_enterprise_contact_form","use_paginated_org_picker_cost_center_form","use_paginated_repo_picker_cost_center_form","viewscreen_sandbox"],"login":"dhashvanth21"}</script><link rel="dns-prefetch" href="https://github.githubassets.com/"><link rel="dns-prefetch" href="https://avatars.githubusercontent.com/"><link rel="dns-prefetch" href="https://github-cloud.s3.amazonaws.com/"><link rel="dns-prefetch" href="https://user-images.githubusercontent.com/"><link rel="preconnect" href="https://github.githubassets.com/" crossorigin=""><link rel="preconnect" href="https://avatars.githubusercontent.com/"><link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/light-74231a1f3bbb.css"><title>Module1/Conditional Statements in Python: Even or Odd Checker.md at main · Kiran437228/Module1</title><meta name="route-pattern" content="/:user_id/:repository/blob/*name(/*path)" data-turbo-transient=""><meta name="route-controller" content="blob" data-turbo-transient=""><meta name="route-action" content="show" data-turbo-transient=""><meta name="fetch-nonce" content="v1:75ea35dc-9409-f3c3-903c-f1f3c0393ed3"><meta name="current-catalog-service-hash" content="f3abb0cc802f3d7b95fc8762b94bdcb13bf39634c40c357301c4aa1d67a256fb"><meta name="request-id" content="DCAA:266E0A:B8066:E3BEC:6824E870" data-turbo-transient="true"><meta name="html-safe-nonce" content="d7a50e8dee2d92e0efc964a19788ef06732669ab602056aa9302dcaa30afa678" data-turbo-transient="true"><meta name="visitor-payload" content="eyJyZWZlcnJlciI6Imh0dHBzOi8vZ2l0aHViLmNvbS9LaXJhbjQzNzIyOC9Nb2R1bGUxL2Jsb2IvbWFpbi9Db25kaXRpb25hbCUyMFN0YXRlbWVudHMlMjBpbiUyMFB5dGhvbiUzQSUyMEV2ZW4lMjBvciUyME9kZCUyMENoZWNrZXIubWQiLCJyZXF1ZXN0X2lkIjoiRENBQToyNjZFMEE6QjgwNjY6RTNCRUM6NjgyNEU4NzAiLCJ2aXNpdG9yX2lkIjoiNTk2NzcwNDM5NDkxMzA0MDYxNSIsInJlZ2lvbl9lZGdlIjoiY2VudHJhbGluZGlhIiwicmVnaW9uX3JlbmRlciI6ImlhZCJ9" data-turbo-transient="true"><meta name="visitor-hmac" content="f5d6cee7104f1e47cbb08b05f5f054d1990ae6c98969a8b4529c785d582d24c1" data-turbo-transient="true"><meta name="hovercard-subject-tag" content="repository:974415414" data-turbo-transient=""><meta name="github-keyboard-shortcuts" content="repository,source-code,file-tree,copilot" data-turbo-transient="true"><meta name="selected-link" value="repo_source" data-turbo-transient=""><link rel="assets" href="https://github.githubassets.com/"><meta name="google-site-verification" content="Apib7-x98H0j5cPqHWwSMm6dNU4GmODRoqxLiDzdx9I"><meta name="octolytics-url" content="https://collector.github.com/github/collect"><meta name="octolytics-actor-id" content="182338033"><meta name="octolytics-actor-login" content="dhashvanth21"><meta name="octolytics-actor-hash" content="590703ea93008dd4abccb6523a54ac6bdeabcea6f1d7a6c8aca578fd270c998a"><meta name="analytics-location" content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-turbo-transient="true"><meta name="user-login" content="dhashvanth21"><link rel="sudo-modal" href="https://github.com/sessions/sudo_modal"><meta name="turbo-cache-control" content="no-preview" data-turbo-transient=""><meta name="turbo-cache-control" content="no-cache" data-turbo-transient=""><meta data-hydrostats="publish"><meta name="go-import" content="github.com/Kiran437228/Module1 git https://github.com/Kiran437228/Module1.git"><meta name="octolytics-dimension-user_id" content="182343513"><meta name="octolytics-dimension-user_login" content="Kiran437228"><meta name="octolytics-dimension-repository_id" content="974415414"><meta name="octolytics-dimension-repository_nwo" content="Kiran437228/Module1"><meta name="octolytics-dimension-repository_public" content="true"><meta name="octolytics-dimension-repository_is_fork" content="true"><meta name="octolytics-dimension-repository_parent_id" content="966686068"><meta name="octolytics-dimension-repository_parent_nwo" content="Silambarasi63/Module1"><meta name="octolytics-dimension-repository_network_root_id" content="966686068"><meta name="octolytics-dimension-repository_network_root_nwo" content="Silambarasi63/Module1"><meta name="turbo-body-classes" content="logged-in env-production page-responsive"><meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats"><meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors"><meta name="release" content="0830a5ede42ee318303570c36845963ff2abdd9a"><link rel="mask-icon" href="https://github.githubassets.com/assets/pinned-octocat-093da3e6fa40.svg" color="#000000"><link rel="alternate icon" class="js-site-favicon" type="image/png" href="https://github.githubassets.com/favicons/favicon-dark.png"><link rel="icon" class="js-site-favicon" type="image/svg+xml" href="https://github.githubassets.com/favicons/favicon-dark.svg" data-base-href="https://github.githubassets.com/favicons/favicon"><meta name="theme-color" content="#1e2327"><meta name="color-scheme" content="light dark"><meta name="msapplication-TileImage" content="/windows-tile.png"><meta name="msapplication-TileColor" content="#ffffff"><link rel="manifest" href="https://github.com/manifest.json" crossorigin="use-credentials"><style type="text/css" id="ms-consent-banner-theme-styles"></style><link rel="stylesheet" type="text/css" href="./Conditional Statements in Python_ Even or Odd Checker_files/app_assets_modules_react-code-view_components_blob-edit_BlobEditor_tsx-app_assets_modules_sec-3094c3.aca17a3da3b9d21d4f5e.module.css" crossorigin="anonymous"></head>

  <body class="logged-in env-production page-responsive" style="overflow-wrap: break-word; --dialog-scrollgutter: 15px;">
    <div data-turbo-body="" class="logged-in env-production page-responsive" style="word-wrap: break-word;">
      



    <div class="position-relative header-wrapper js-header-wrapper ">
      <a href="https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md#start-of-content" data-skip-target-assigned="false" class="p-3 color-bg-accent-emphasis color-fg-on-emphasis show-on-focus js-skip-to-content">Skip to content</a>

      <span data-view-component="true" class="progress-pjax-loader Progress position-fixed width-full">
    <span style="width: 0%;" data-view-component="true" class="Progress-item progress-pjax-loader-bar left-0 top-0 color-bg-accent-emphasis"></span>
</span>      
      
      <script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_ui-commands_ui-commands_ts-eeddffae9643.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/keyboard-shortcuts-dialog-59c6d1a3f8b0.js.download"></script>
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/primer-react.d2117d7623cc63123645.module.css">
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/keyboard-shortcuts-dialog.b973d595584666020636.module.css">

<react-partial partial-name="keyboard-shortcuts-dialog" data-ssr="false" data-attempted-ssr="false" data-catalyst="" class="loaded">
  
  <script type="application/json" data-target="react-partial.embeddedData">{"props":{"docsUrl":"https://docs.github.com/get-started/accessibility/keyboard-shortcuts"}}</script>
  <div data-target="react-partial.reactRoot"><div class="d-none"></div><script type="application/json" id="__PRIMER_DATA_:r6u:__">{"resolvedServerColorMode":"night"}</script></div>
</react-partial>




      

          

              <header class="AppHeader" role="banner">
  <h2 class="sr-only">Navigation Menu</h2>


    

    <div class="AppHeader-globalBar pb-2 js-global-bar">
      <div class="AppHeader-globalBar-start">
        <div class="">
            <deferred-side-panel data-url="/_side-panels/global" data-catalyst="">
  <include-fragment data-target="deferred-side-panel.fragment" data-nonce="v1:75ea35dc-9409-f3c3-903c-f1f3c0393ed3" data-view-component="true"><template shadowrootmode="open"><style>:host {display: block;}</style><slot></slot></template>
      <button aria-label="Open global navigation menu" data-action="click:deferred-side-panel#loadPanel click:deferred-side-panel#panelOpened" data-show-dialog-id="dialog-673dbe0c-37a5-44e9-8514-62d9c153eba5" id="dialog-show-dialog-673dbe0c-37a5-44e9-8514-62d9c153eba5" type="button" data-view-component="true" class="Button Button--iconOnly Button--secondary Button--medium AppHeader-button p-0 color-fg-muted">  <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-three-bars Button-visual">
    <path d="M1 2.75A.75.75 0 0 1 1.75 2h12.5a.75.75 0 0 1 0 1.5H1.75A.75.75 0 0 1 1 2.75Zm0 5A.75.75 0 0 1 1.75 7h12.5a.75.75 0 0 1 0 1.5H1.75A.75.75 0 0 1 1 7.75ZM1.75 12h12.5a.75.75 0 0 1 0 1.5H1.75a.75.75 0 0 1 0-1.5Z"></path>
</svg>
</button>

<dialog-helper>
  <dialog data-target="deferred-side-panel.panel" id="dialog-673dbe0c-37a5-44e9-8514-62d9c153eba5" aria-modal="true" aria-labelledby="dialog-673dbe0c-37a5-44e9-8514-62d9c153eba5-title" aria-describedby="dialog-673dbe0c-37a5-44e9-8514-62d9c153eba5-description" data-view-component="true" class="Overlay Overlay-whenNarrow Overlay--size-small-portrait Overlay--motion-scaleFade Overlay--placement-left SidePanel Overlay--disableScroll">
    <div styles="flex-direction: row;" data-view-component="true" class="Overlay-header">
  <div class="Overlay-headerContentWrap">
    <div class="Overlay-titleWrap">
      <h1 class="Overlay-title sr-only" id="dialog-673dbe0c-37a5-44e9-8514-62d9c153eba5-title">
        Global navigation
      </h1>
            <div data-view-component="true" class="d-flex">
      <div data-view-component="true" class="AppHeader-logo position-relative">
        <svg aria-hidden="true" height="24" viewBox="0 0 24 24" version="1.1" width="24" data-view-component="true" class="octicon octicon-mark-github">
    <path d="M12 1C5.9225 1 1 5.9225 1 12C1 16.8675 4.14875 20.9787 8.52125 22.4362C9.07125 22.5325 9.2775 22.2025 9.2775 21.9137C9.2775 21.6525 9.26375 20.7862 9.26375 19.865C6.5 20.3737 5.785 19.1912 5.565 18.5725C5.44125 18.2562 4.905 17.28 4.4375 17.0187C4.0525 16.8125 3.5025 16.3037 4.42375 16.29C5.29 16.2762 5.90875 17.0875 6.115 17.4175C7.105 19.0812 8.68625 18.6137 9.31875 18.325C9.415 17.61 9.70375 17.1287 10.02 16.8537C7.5725 16.5787 5.015 15.63 5.015 11.4225C5.015 10.2262 5.44125 9.23625 6.1425 8.46625C6.0325 8.19125 5.6475 7.06375 6.2525 5.55125C6.2525 5.55125 7.17375 5.2625 9.2775 6.67875C10.1575 6.43125 11.0925 6.3075 12.0275 6.3075C12.9625 6.3075 13.8975 6.43125 14.7775 6.67875C16.8813 5.24875 17.8025 5.55125 17.8025 5.55125C18.4075 7.06375 18.0225 8.19125 17.9125 8.46625C18.6138 9.23625 19.04 10.2125 19.04 11.4225C19.04 15.6437 16.4688 16.5787 14.0213 16.8537C14.42 17.1975 14.7638 17.8575 14.7638 18.8887C14.7638 20.36 14.75 21.5425 14.75 21.9137C14.75 22.2025 14.9563 22.5462 15.5063 22.4362C19.8513 20.9787 23 16.8537 23 12C23 5.9225 18.0775 1 12 1Z"></path>
</svg>
</div></div>
    </div>
    <div class="Overlay-actionWrap">
      <button data-close-dialog-id="dialog-673dbe0c-37a5-44e9-8514-62d9c153eba5" aria-label="Close" type="button" data-view-component="true" class="close-button Overlay-closeButton"><svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path d="M3.72 3.72a.75.75 0 0 1 1.06 0L8 6.94l3.22-3.22a.749.749 0 0 1 1.275.326.749.749 0 0 1-.215.734L9.06 8l3.22 3.22a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215L8 9.06l-3.22 3.22a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042L6.94 8 3.72 4.78a.75.75 0 0 1 0-1.06Z"></path>
</svg></button>
    </div>
  </div>
  
</div>
      <scrollable-region data-labelled-by="dialog-673dbe0c-37a5-44e9-8514-62d9c153eba5-title" data-catalyst="" style="overflow: auto;">
        <div data-view-component="true" class="Overlay-body d-flex flex-column px-2">    <div data-view-component="true" class="d-flex flex-column mb-3">
        <nav aria-label="Site navigation" data-view-component="true" class="ActionList">
  
  <nav-list data-catalyst="">
    <ul data-target="nav-list.topLevelList" data-view-component="true" class="ActionListWrap">
        
          
<li data-item-id="" data-targets="nav-list.items" data-view-component="true" class="ActionListItem">
    
    
    <a data-hotkey="g d" data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;HOME&quot;,&quot;label&quot;:null}" id="item-206a3e37-c50b-4bf9-8aa3-f00adff8b6ec" href="https://github.com/dashboard" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-home">
    <path d="M6.906.664a1.749 1.749 0 0 1 2.187 0l5.25 4.2c.415.332.657.835.657 1.367v7.019A1.75 1.75 0 0 1 13.25 15h-3.5a.75.75 0 0 1-.75-.75V9H7v5.25a.75.75 0 0 1-.75.75h-3.5A1.75 1.75 0 0 1 1 13.25V6.23c0-.531.242-1.034.657-1.366l5.25-4.2Zm1.25 1.171a.25.25 0 0 0-.312 0l-5.25 4.2a.25.25 0 0 0-.094.196v7.019c0 .138.112.25.25.25H5.5V8.25a.75.75 0 0 1 .75-.75h3.5a.75.75 0 0 1 .75.75v5.25h2.75a.25.25 0 0 0 .25-.25V6.23a.25.25 0 0 0-.094-.195Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Home
</span>      
</a>
  
</li>

        
          
<li data-item-id="" data-targets="nav-list.items" data-view-component="true" class="ActionListItem">
    
    
    <a data-hotkey="g i" data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;ISSUES&quot;,&quot;label&quot;:null}" id="item-90d938b5-736c-404b-b235-d37f6f63e29f" href="https://github.com/issues" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-issue-opened">
    <path d="M8 9.5a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Z"></path><path d="M8 0a8 8 0 1 1 0 16A8 8 0 0 1 8 0ZM1.5 8a6.5 6.5 0 1 0 13 0 6.5 6.5 0 0 0-13 0Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Issues
</span>      
</a>
  
</li>

        
          
<li data-item-id="" data-targets="nav-list.items" data-view-component="true" class="ActionListItem">
    
    
    <a data-hotkey="g p" data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;PULL_REQUESTS&quot;,&quot;label&quot;:null}" id="item-77af1fd9-6150-4cd0-8564-cf4b6fe752b2" href="https://github.com/pulls" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-git-pull-request">
    <path d="M1.5 3.25a2.25 2.25 0 1 1 3 2.122v5.256a2.251 2.251 0 1 1-1.5 0V5.372A2.25 2.25 0 0 1 1.5 3.25Zm5.677-.177L9.573.677A.25.25 0 0 1 10 .854V2.5h1A2.5 2.5 0 0 1 13.5 5v5.628a2.251 2.251 0 1 1-1.5 0V5a1 1 0 0 0-1-1h-1v1.646a.25.25 0 0 1-.427.177L7.177 3.427a.25.25 0 0 1 0-.354ZM3.75 2.5a.75.75 0 1 0 0 1.5.75.75 0 0 0 0-1.5Zm0 9.5a.75.75 0 1 0 0 1.5.75.75 0 0 0 0-1.5Zm8.25.75a.75.75 0 1 0 1.5 0 .75.75 0 0 0-1.5 0Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Pull requests
</span>      
</a>
  
</li>

        
          
<li data-item-id="" data-targets="nav-list.items" data-view-component="true" class="ActionListItem">
    
    
    <a data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;PROJECTS&quot;,&quot;label&quot;:null}" id="item-0fcf580f-c14e-44e8-9936-5651c928399d" href="https://github.com/projects" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-table">
    <path d="M0 1.75C0 .784.784 0 1.75 0h12.5C15.216 0 16 .784 16 1.75v12.5A1.75 1.75 0 0 1 14.25 16H1.75A1.75 1.75 0 0 1 0 14.25ZM6.5 6.5v8h7.75a.25.25 0 0 0 .25-.25V6.5Zm8-1.5V1.75a.25.25 0 0 0-.25-.25H6.5V5Zm-13 1.5v7.75c0 .138.112.25.25.25H5v-8ZM5 5V1.5H1.75a.25.25 0 0 0-.25.25V5Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Projects
</span>      
</a>
  
</li>

        
          
<li data-item-id="" data-targets="nav-list.items" data-view-component="true" class="ActionListItem">
    
    
    <a data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;DISCUSSIONS&quot;,&quot;label&quot;:null}" id="item-0a8c8f36-7ff1-4e23-afed-e626afd9261b" href="https://github.com/discussions" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-comment-discussion">
    <path d="M1.75 1h8.5c.966 0 1.75.784 1.75 1.75v5.5A1.75 1.75 0 0 1 10.25 10H7.061l-2.574 2.573A1.458 1.458 0 0 1 2 11.543V10h-.25A1.75 1.75 0 0 1 0 8.25v-5.5C0 1.784.784 1 1.75 1ZM1.5 2.75v5.5c0 .138.112.25.25.25h1a.75.75 0 0 1 .75.75v2.19l2.72-2.72a.749.749 0 0 1 .53-.22h3.5a.25.25 0 0 0 .25-.25v-5.5a.25.25 0 0 0-.25-.25h-8.5a.25.25 0 0 0-.25.25Zm13 2a.25.25 0 0 0-.25-.25h-.5a.75.75 0 0 1 0-1.5h.5c.966 0 1.75.784 1.75 1.75v5.5A1.75 1.75 0 0 1 14.25 12H14v1.543a1.458 1.458 0 0 1-2.487 1.03L9.22 12.28a.749.749 0 0 1 .326-1.275.749.749 0 0 1 .734.215l2.22 2.22v-2.19a.75.75 0 0 1 .75-.75h1a.25.25 0 0 0 .25-.25Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Discussions
</span>      
</a>
  
</li>

        
          
<li data-item-id="" data-targets="nav-list.items" data-view-component="true" class="ActionListItem">
    
    
    <a data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;CODESPACES&quot;,&quot;label&quot;:null}" id="item-3c1daf25-f445-4acb-8e29-6f2b9deb780b" href="https://github.com/codespaces" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-codespaces">
    <path d="M0 11.25c0-.966.784-1.75 1.75-1.75h12.5c.966 0 1.75.784 1.75 1.75v3A1.75 1.75 0 0 1 14.25 16H1.75A1.75 1.75 0 0 1 0 14.25Zm2-9.5C2 .784 2.784 0 3.75 0h8.5C13.216 0 14 .784 14 1.75v5a1.75 1.75 0 0 1-1.75 1.75h-8.5A1.75 1.75 0 0 1 2 6.75Zm1.75-.25a.25.25 0 0 0-.25.25v5c0 .138.112.25.25.25h8.5a.25.25 0 0 0 .25-.25v-5a.25.25 0 0 0-.25-.25Zm-2 9.5a.25.25 0 0 0-.25.25v3c0 .138.112.25.25.25h12.5a.25.25 0 0 0 .25-.25v-3a.25.25 0 0 0-.25-.25Z"></path><path d="M7 12.75a.75.75 0 0 1 .75-.75h4.5a.75.75 0 0 1 0 1.5h-4.5a.75.75 0 0 1-.75-.75Zm-4 0a.75.75 0 0 1 .75-.75h.5a.75.75 0 0 1 0 1.5h-.5a.75.75 0 0 1-.75-.75Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Codespaces
</span>      
</a>
  
</li>

        
          
<li data-item-id="" data-targets="nav-list.items" data-view-component="true" class="ActionListItem">
    
    
    <a data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;COPILOT&quot;,&quot;label&quot;:null}" id="item-f20c9961-b7fc-4084-9d04-5f8ac5acb45b" href="https://github.com/copilot" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copilot">
    <path d="M7.998 15.035c-4.562 0-7.873-2.914-7.998-3.749V9.338c.085-.628.677-1.686 1.588-2.065.013-.07.024-.143.036-.218.029-.183.06-.384.126-.612-.201-.508-.254-1.084-.254-1.656 0-.87.128-1.769.693-2.484.579-.733 1.494-1.124 2.724-1.261 1.206-.134 2.262.034 2.944.765.05.053.096.108.139.165.044-.057.094-.112.143-.165.682-.731 1.738-.899 2.944-.765 1.23.137 2.145.528 2.724 1.261.566.715.693 1.614.693 2.484 0 .572-.053 1.148-.254 1.656.066.228.098.429.126.612.012.076.024.148.037.218.924.385 1.522 1.471 1.591 2.095v1.872c0 .766-3.351 3.795-8.002 3.795Zm0-1.485c2.28 0 4.584-1.11 5.002-1.433V7.862l-.023-.116c-.49.21-1.075.291-1.727.291-1.146 0-2.059-.327-2.71-.991A3.222 3.222 0 0 1 8 6.303a3.24 3.24 0 0 1-.544.743c-.65.664-1.563.991-2.71.991-.652 0-1.236-.081-1.727-.291l-.023.116v4.255c.419.323 2.722 1.433 5.002 1.433ZM6.762 2.83c-.193-.206-.637-.413-1.682-.297-1.019.113-1.479.404-1.713.7-.247.312-.369.789-.369 1.554 0 .793.129 1.171.308 1.371.162.181.519.379 1.442.379.853 0 1.339-.235 1.638-.54.315-.322.527-.827.617-1.553.117-.935-.037-1.395-.241-1.614Zm4.155-.297c-1.044-.116-1.488.091-1.681.297-.204.219-.359.679-.242 1.614.091.726.303 1.231.618 1.553.299.305.784.54 1.638.54.922 0 1.28-.198 1.442-.379.179-.2.308-.578.308-1.371 0-.765-.123-1.242-.37-1.554-.233-.296-.693-.587-1.713-.7Z"></path><path d="M6.25 9.037a.75.75 0 0 1 .75.75v1.501a.75.75 0 0 1-1.5 0V9.787a.75.75 0 0 1 .75-.75Zm4.25.75v1.501a.75.75 0 0 1-1.5 0V9.787a.75.75 0 0 1 1.5 0Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Copilot
</span>      
</a>
  
</li>

        
          <li role="presentation" aria-hidden="true" data-view-component="true" class="ActionList-sectionDivider"></li>
        
          
<li data-item-id="" data-targets="nav-list.items" data-view-component="true" class="ActionListItem">
    
    
    <a data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;EXPLORE&quot;,&quot;label&quot;:null}" id="item-2aed73ed-6ce7-4415-9da6-3dee8f80b232" href="https://github.com/explore" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-telescope">
    <path d="M14.184 1.143v-.001l1.422 2.464a1.75 1.75 0 0 1-.757 2.451L3.104 11.713a1.75 1.75 0 0 1-2.275-.702l-.447-.775a1.75 1.75 0 0 1 .53-2.32L11.682.573a1.748 1.748 0 0 1 2.502.57Zm-4.709 9.32h-.001l2.644 3.863a.75.75 0 1 1-1.238.848l-1.881-2.75v2.826a.75.75 0 0 1-1.5 0v-2.826l-1.881 2.75a.75.75 0 1 1-1.238-.848l2.049-2.992a.746.746 0 0 1 .293-.253l1.809-.87a.749.749 0 0 1 .944.252ZM9.436 3.92h-.001l-4.97 3.39.942 1.63 5.42-2.61Zm3.091-2.108h.001l-1.85 1.26 1.505 2.605 2.016-.97a.247.247 0 0 0 .13-.151.247.247 0 0 0-.022-.199l-1.422-2.464a.253.253 0 0 0-.161-.119.254.254 0 0 0-.197.038ZM1.756 9.157a.25.25 0 0 0-.075.33l.447.775a.25.25 0 0 0 .325.1l1.598-.769-.83-1.436-1.465 1Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Explore
</span>      
</a>
  
</li>

        
          
<li data-item-id="" data-targets="nav-list.items" data-view-component="true" class="ActionListItem">
    
    
    <a data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;MARKETPLACE&quot;,&quot;label&quot;:null}" id="item-59bd1af2-3461-46c0-823d-c142661af2fe" href="https://github.com/marketplace" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-gift">
    <path d="M2 2.75A2.75 2.75 0 0 1 4.75 0c.983 0 1.873.42 2.57 1.232.268.318.497.668.68 1.042.183-.375.411-.725.68-1.044C9.376.42 10.266 0 11.25 0a2.75 2.75 0 0 1 2.45 4h.55c.966 0 1.75.784 1.75 1.75v2c0 .698-.409 1.301-1 1.582v4.918A1.75 1.75 0 0 1 13.25 16H2.75A1.75 1.75 0 0 1 1 14.25V9.332C.409 9.05 0 8.448 0 7.75v-2C0 4.784.784 4 1.75 4h.55c-.192-.375-.3-.8-.3-1.25ZM7.25 9.5H2.5v4.75c0 .138.112.25.25.25h4.5Zm1.5 0v5h4.5a.25.25 0 0 0 .25-.25V9.5Zm0-4V8h5.5a.25.25 0 0 0 .25-.25v-2a.25.25 0 0 0-.25-.25Zm-7 0a.25.25 0 0 0-.25.25v2c0 .138.112.25.25.25h5.5V5.5h-5.5Zm3-4a1.25 1.25 0 0 0 0 2.5h2.309c-.233-.818-.542-1.401-.878-1.793-.43-.502-.915-.707-1.431-.707ZM8.941 4h2.309a1.25 1.25 0 0 0 0-2.5c-.516 0-1 .205-1.43.707-.337.392-.646.975-.879 1.793Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Marketplace
</span>      
</a>
  
</li>

</ul>  </nav-list>
</nav>

        <div data-view-component="true" class="my-3 d-flex flex-justify-center height-full">
          <span data-view-component="true">
  <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="16" height="16" viewBox="0 0 16 16" fill="none" aria-hidden="true" data-view-component="true" class="anim-rotate">
    <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" fill="none"></circle>
    <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke"></path>
</svg>    <span class="sr-only">Loading</span>
</span>
</div>
</div>
      <div data-view-component="true" class="flex-1"></div>


      <div data-view-component="true" class="px-2">      <p class="color-fg-subtle text-small text-light">© 2025 GitHub, Inc.</p>

      <div data-view-component="true" class="d-flex flex-wrap text-small text-light">
          <a target="_blank" href="https://github.com/about" data-view-component="true" class="Link mr-2">About</a>
          <a target="_blank" href="https://github.blog/" data-view-component="true" class="Link mr-2">Blog</a>
          <a target="_blank" href="https://docs.github.com/site-policy/github-terms/github-terms-of-service" data-view-component="true" class="Link mr-2">Terms</a>
          <a target="_blank" href="https://docs.github.com/site-policy/privacy-policies/github-privacy-statement" data-view-component="true" class="Link mr-2">Privacy</a>
          <a target="_blank" href="https://github.com/security" data-view-component="true" class="Link mr-2">Security</a>
          <a target="_blank" href="https://www.githubstatus.com/" data-view-component="true" class="Link mr-3">Status</a>

</div></div>
</div>
      </scrollable-region>
      
</dialog></dialog-helper>

</include-fragment></deferred-side-panel>
        </div>

        <a class="AppHeader-logo ml-1 " href="https://github.com/" data-hotkey="g d" aria-label="Homepage " data-turbo="false" data-analytics-event="{&quot;category&quot;:&quot;Header&quot;,&quot;action&quot;:&quot;go to dashboard&quot;,&quot;label&quot;:&quot;icon:logo&quot;}">
          <svg height="32" aria-hidden="true" viewBox="0 0 24 24" version="1.1" width="32" data-view-component="true" class="octicon octicon-mark-github v-align-middle">
    <path d="M12 1C5.9225 1 1 5.9225 1 12C1 16.8675 4.14875 20.9787 8.52125 22.4362C9.07125 22.5325 9.2775 22.2025 9.2775 21.9137C9.2775 21.6525 9.26375 20.7862 9.26375 19.865C6.5 20.3737 5.785 19.1912 5.565 18.5725C5.44125 18.2562 4.905 17.28 4.4375 17.0187C4.0525 16.8125 3.5025 16.3037 4.42375 16.29C5.29 16.2762 5.90875 17.0875 6.115 17.4175C7.105 19.0812 8.68625 18.6137 9.31875 18.325C9.415 17.61 9.70375 17.1287 10.02 16.8537C7.5725 16.5787 5.015 15.63 5.015 11.4225C5.015 10.2262 5.44125 9.23625 6.1425 8.46625C6.0325 8.19125 5.6475 7.06375 6.2525 5.55125C6.2525 5.55125 7.17375 5.2625 9.2775 6.67875C10.1575 6.43125 11.0925 6.3075 12.0275 6.3075C12.9625 6.3075 13.8975 6.43125 14.7775 6.67875C16.8813 5.24875 17.8025 5.55125 17.8025 5.55125C18.4075 7.06375 18.0225 8.19125 17.9125 8.46625C18.6138 9.23625 19.04 10.2125 19.04 11.4225C19.04 15.6437 16.4688 16.5787 14.0213 16.8537C14.42 17.1975 14.7638 17.8575 14.7638 18.8887C14.7638 20.36 14.75 21.5425 14.75 21.9137C14.75 22.2025 14.9563 22.5462 15.5063 22.4362C19.8513 20.9787 23 16.8537 23 12C23 5.9225 18.0775 1 12 1Z"></path>
</svg>
        </a>

          <context-region-observer class="AppHeader-context " data-catalyst="">
    <div class="AppHeader-context-compact" data-target="context-region-observer.compactContainer">
        <button aria-expanded="false" aria-haspopup="dialog" aria-label="Page context: Kiran437228 / Module1" data-target="context-region-observer.compactContextRegion" data-show-dialog-id="context-region-dialog" id="dialog-show-context-region-dialog" type="button" data-view-component="true" class="AppHeader-context-compact-trigger Truncate Button--secondary Button--medium Button box-shadow-none">  <span class="Button-content">
    <span class="Button-label"><span class="AppHeader-context-compact-lead">
            <span class="AppHeader-context-compact-parentItem">Kiran437228</span>

            <span class="no-wrap">&nbsp;/</span>

        </span>

        <strong class="AppHeader-context-compact-mainItem d-flex flex-items-center Truncate">
  <span class="Truncate-text ">Module1</span>

</strong></span>
  </span>
</button>

<dialog-helper>
  <dialog id="context-region-dialog" aria-modal="true" aria-labelledby="context-region-dialog-title" aria-describedby="context-region-dialog-description" data-view-component="true" class="Overlay Overlay-whenNarrow Overlay--size-medium Overlay--motion-scaleFade Overlay--disableScroll">
    <div data-view-component="true" class="Overlay-header">
  <div class="Overlay-headerContentWrap">
    <div class="Overlay-titleWrap">
      <h1 class="Overlay-title " id="context-region-dialog-title">
        Navigate back to
      </h1>
        
    </div>
    <div class="Overlay-actionWrap">
      <button data-close-dialog-id="context-region-dialog" aria-label="Close" type="button" data-view-component="true" class="close-button Overlay-closeButton"><svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path d="M3.72 3.72a.75.75 0 0 1 1.06 0L8 6.94l3.22-3.22a.749.749 0 0 1 1.275.326.749.749 0 0 1-.215.734L9.06 8l3.22 3.22a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215L8 9.06l-3.22 3.22a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042L6.94 8 3.72 4.78a.75.75 0 0 1 0-1.06Z"></path>
</svg></button>
    </div>
  </div>
  
</div>
      <scrollable-region data-labelled-by="context-region-dialog-title" data-catalyst="" style="overflow: auto;">
        <div data-view-component="true" class="Overlay-body">      <ul role="list" class="list-style-none">
    <li>
      <a data-analytics-event="{&quot;category&quot;:&quot;SiteHeaderComponent&quot;,&quot;action&quot;:&quot;context_region_crumb&quot;,&quot;label&quot;:&quot;Kiran437228&quot;,&quot;screen_size&quot;:&quot;compact&quot;}" href="https://github.com/Kiran437228" data-view-component="true" class="Link--primary Truncate d-flex flex-items-center py-1">
        <span class="AppHeader-context-item-label Truncate-text ">
            <svg aria-hidden="true" height="12" viewBox="0 0 16 16" version="1.1" width="12" data-view-component="true" class="octicon octicon-person mr-1">
    <path d="M10.561 8.073a6.005 6.005 0 0 1 3.432 5.142.75.75 0 1 1-1.498.07 4.5 4.5 0 0 0-8.99 0 .75.75 0 0 1-1.498-.07 6.004 6.004 0 0 1 3.431-5.142 3.999 3.999 0 1 1 5.123 0ZM10.5 5a2.5 2.5 0 1 0-5 0 2.5 2.5 0 0 0 5 0Z"></path>
</svg>

          Kiran437228
        </span>

</a>
    </li>
    <li>
      <a data-analytics-event="{&quot;category&quot;:&quot;SiteHeaderComponent&quot;,&quot;action&quot;:&quot;context_region_crumb&quot;,&quot;label&quot;:&quot;Module1&quot;,&quot;screen_size&quot;:&quot;compact&quot;}" href="https://github.com/Kiran437228/Module1" data-view-component="true" class="Link--primary Truncate d-flex flex-items-center py-1">
        <span class="AppHeader-context-item-label Truncate-text ">
            <svg aria-hidden="true" height="12" viewBox="0 0 16 16" version="1.1" width="12" data-view-component="true" class="octicon octicon-repo mr-1">
    <path d="M2 2.5A2.5 2.5 0 0 1 4.5 0h8.75a.75.75 0 0 1 .75.75v12.5a.75.75 0 0 1-.75.75h-2.5a.75.75 0 0 1 0-1.5h1.75v-2h-8a1 1 0 0 0-.714 1.7.75.75 0 1 1-1.072 1.05A2.495 2.495 0 0 1 2 11.5Zm10.5-1h-8a1 1 0 0 0-1 1v6.708A2.486 2.486 0 0 1 4.5 9h8ZM5 12.25a.25.25 0 0 1 .25-.25h3.5a.25.25 0 0 1 .25.25v3.25a.25.25 0 0 1-.4.2l-1.45-1.087a.249.249 0 0 0-.3 0L5.4 15.7a.25.25 0 0 1-.4-.2Z"></path>
</svg>

          Module1
        </span>

</a>
    </li>
</ul>

</div>
      </scrollable-region>
      
</dialog></dialog-helper>

    </div>

  <div class="AppHeader-context-full">
    <nav role="navigation" aria-label="Page context">
        
<context-region role="list" data-action="context-region-changed:context-region-observer#crumbsChanged" data-catalyst="" data-max-items="5">
    <context-region-crumb data-targets="context-region.crumbs" data-label="Kiran437228" data-href="/Kiran437228" data-pre-rendered="" role="listitem" data-catalyst="">
      <a data-analytics-event="{&quot;category&quot;:&quot;SiteHeaderComponent&quot;,&quot;action&quot;:&quot;context_region_crumb&quot;,&quot;label&quot;:&quot;Kiran437228&quot;,&quot;screen_size&quot;:&quot;full&quot;}" data-hovercard-type="user" data-hovercard-url="/users/Kiran437228/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" data-target="context-region-crumb.link" href="https://github.com/Kiran437228" data-view-component="true" class="AppHeader-context-item">
        <span data-target="context-region-crumb.labelElement" class="AppHeader-context-item-label  ">Kiran437228</span>

</a>
        <context-region-divider data-target="context-region-crumb.dividerElement" data-pre-rendered="" data-catalyst="">
  <span class="AppHeader-context-item-separator">
    <span class="sr-only">/</span>
    <svg width="16" height="16" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
      <path d="M10.956 1.27994L6.06418 14.7201L5 14.7201L9.89181 1.27994L10.956 1.27994Z" fill="currentcolor"></path>
    </svg>
  </span>
</context-region-divider>

    </context-region-crumb>
    <context-region-crumb data-targets="context-region.crumbs" data-label="Module1" data-href="/Kiran437228/Module1" data-pre-rendered="" role="listitem" data-catalyst="">
      <a data-analytics-event="{&quot;category&quot;:&quot;SiteHeaderComponent&quot;,&quot;action&quot;:&quot;context_region_crumb&quot;,&quot;label&quot;:&quot;Module1&quot;,&quot;screen_size&quot;:&quot;full&quot;}" data-target="context-region-crumb.link" href="https://github.com/Kiran437228/Module1" data-view-component="true" class="AppHeader-context-item">
        <span data-target="context-region-crumb.labelElement" class="AppHeader-context-item-label  ">Module1</span>

</a>
        <context-region-divider data-target="context-region-crumb.dividerElement" data-pre-rendered="" data-catalyst="">
  <span class="AppHeader-context-item-separator">
    <span class="sr-only">/</span>
    <svg width="16" height="16" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
      <path d="M10.956 1.27994L6.06418 14.7201L5 14.7201L9.89181 1.27994L10.956 1.27994Z" fill="currentcolor"></path>
    </svg>
  </span>
</context-region-divider>

    </context-region-crumb>
</context-region>

    </nav>
  </div>
</context-region-observer>

      </div>
      <div class="AppHeader-globalBar-end">
          <div class="AppHeader-search">
              


<qbsearch-input class="search-input" data-scope="repo:Kiran437228/Module1" data-custom-scopes-path="/search/custom_scopes" data-delete-custom-scopes-csrf="Bfbpr6qC3fOghrAB5jJWO6Jtts9QVdW_-ytScIV7rLWgmJTNXvXDpnrXdHQN3_eowqNQfp0mjsxgmPOidZUrmA" data-max-custom-scopes="10" data-header-redesign-enabled="true" data-initial-value="" data-blackbird-suggestions-path="/search/suggestions" data-jump-to-suggestions-path="/_graphql/GetSuggestedNavigationDestinations" data-current-repository="Kiran437228/Module1" data-current-org="" data-current-owner="Kiran437228" data-logged-in="true" data-copilot-chat-enabled="false" data-nl-search-enabled="false" data-catalyst="">
  <div class="search-input-container search-with-dialog position-relative d-flex flex-row flex-items-center height-auto color-bg-transparent border-0 color-fg-subtle mx-0" data-action="click:qbsearch-input#searchInputContainerClicked">
      
            <button type="button" data-action="click:qbsearch-input#handleExpand" class="AppHeader-button AppHeader-search-whenNarrow" aria-label="Search or jump to…" aria-expanded="false" aria-haspopup="dialog">
            <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-search">
    <path d="M10.68 11.74a6 6 0 0 1-7.922-8.982 6 6 0 0 1 8.982 7.922l3.04 3.04a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215ZM11.5 7a4.499 4.499 0 1 0-8.997 0A4.499 4.499 0 0 0 11.5 7Z"></path>
</svg>
          </button>


<div class="AppHeader-search-whenRegular">
  <div class="AppHeader-search-wrap AppHeader-search-wrap--hasTrailing">
    <div class="AppHeader-search-control AppHeader-search-control-overflow">
      <label for="AppHeader-searchInput" aria-label="Search or jump to…" class="AppHeader-search-visual--leading">
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-search">
    <path d="M10.68 11.74a6 6 0 0 1-7.922-8.982 6 6 0 0 1 8.982 7.922l3.04 3.04a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215ZM11.5 7a4.499 4.499 0 1 0-8.997 0A4.499 4.499 0 0 0 11.5 7Z"></path>
</svg>
      </label>

                <button type="button" data-target="qbsearch-input.inputButton" data-action="click:qbsearch-input#handleExpand" class="AppHeader-searchButton form-control input-contrast text-left color-fg-subtle no-wrap placeholder" data-hotkey="s,/" data-analytics-event="{&quot;location&quot;:&quot;navbar&quot;,&quot;action&quot;:&quot;searchbar&quot;,&quot;context&quot;:&quot;global&quot;,&quot;tag&quot;:&quot;input&quot;,&quot;label&quot;:&quot;searchbar_input_global_navbar&quot;}" aria-describedby="search-error-message-flash">
            <div class="overflow-hidden">
              <span id="qb-input-query" data-target="qbsearch-input.inputButtonText">
                  Type <kbd class="AppHeader-search-kbd">/</kbd> to search
              </span>
            </div>
          </button>

    </div>


  </div>
</div>

    <input type="hidden" name="type" class="js-site-search-type-field">

    
<div class="Overlay--hidden " data-modal-dialog-overlay="">
  <modal-dialog data-action="close:qbsearch-input#handleClose cancel:qbsearch-input#handleClose" data-target="qbsearch-input.searchSuggestionsDialog" role="dialog" id="search-suggestions-dialog" aria-modal="true" aria-labelledby="search-suggestions-dialog-header" data-view-component="true" class="Overlay Overlay--width-medium Overlay--height-auto">
      <h1 id="search-suggestions-dialog-header" class="sr-only">Search code, repositories, users, issues, pull requests...</h1>
    <div class="Overlay-body Overlay-body--paddingNone">
      
          <div data-view-component="true">        <div class="search-suggestions position-absolute width-full color-shadow-large border color-fg-default color-bg-default overflow-hidden d-flex flex-column query-builder-container" style="border-radius: 12px;" data-target="qbsearch-input.queryBuilderContainer" hidden="">
          <!-- '"` --><!-- </textarea></xmp> --><form id="query-builder-test-form" action="https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md" accept-charset="UTF-8" method="get">
  <query-builder data-target="qbsearch-input.queryBuilder" id="query-builder-query-builder-test" data-filter-key=":" data-view-component="true" class="QueryBuilder search-query-builder" data-min-width="300" data-catalyst="">
    <div class="FormControl FormControl--fullWidth">
      <label id="query-builder-test-label" for="query-builder-test" class="FormControl-label sr-only">
        Search
      </label>
      <div class="QueryBuilder-StyledInput width-fit " data-target="query-builder.styledInput">
          <span id="query-builder-test-leadingvisual-wrap" class="FormControl-input-leadingVisualWrap QueryBuilder-leadingVisualWrap">
            <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-search FormControl-input-leadingVisual">
    <path d="M10.68 11.74a6 6 0 0 1-7.922-8.982 6 6 0 0 1 8.982 7.922l3.04 3.04a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215ZM11.5 7a4.499 4.499 0 1 0-8.997 0A4.499 4.499 0 0 0 11.5 7Z"></path>
</svg>
          </span>
        <div data-target="query-builder.styledInputContainer" class="QueryBuilder-StyledInputContainer">
          <div aria-hidden="true" class="QueryBuilder-StyledInputContent" data-target="query-builder.styledInputContent"></div>
          <div class="QueryBuilder-InputWrapper">
            <div aria-hidden="true" class="QueryBuilder-Sizer" data-target="query-builder.sizer"><span></span></div>
            <input id="query-builder-test" name="query-builder-test" value="" autocomplete="off" type="text" role="combobox" spellcheck="false" aria-expanded="false" aria-describedby="validation-c04f5b87-ff27-411b-9329-d2db08b85bcf" data-target="query-builder.input" data-action="
          input:query-builder#inputChange
          blur:query-builder#inputBlur
          keydown:query-builder#inputKeydown
          focus:query-builder#inputFocus
        " data-view-component="true" class="FormControl-input QueryBuilder-Input FormControl-medium" aria-controls="query-builder-test-results" aria-autocomplete="list" aria-haspopup="listbox" style="width: 300px;">
          </div>
        </div>
          <span class="sr-only" id="query-builder-test-clear">Clear</span>
          <button role="button" id="query-builder-test-clear-button" aria-labelledby="query-builder-test-clear query-builder-test-label" data-target="query-builder.clearButton" data-action="
                click:query-builder#clear
                focus:query-builder#clearButtonFocus
                blur:query-builder#clearButtonBlur
              " variant="small" hidden="" type="button" data-view-component="true" class="Button Button--iconOnly Button--invisible Button--medium mr-1 px-2 py-0 d-flex flex-items-center rounded-1 color-fg-muted">  <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x-circle-fill Button-visual">
    <path d="M2.343 13.657A8 8 0 1 1 13.658 2.343 8 8 0 0 1 2.343 13.657ZM6.03 4.97a.751.751 0 0 0-1.042.018.751.751 0 0 0-.018 1.042L6.94 8 4.97 9.97a.749.749 0 0 0 .326 1.275.749.749 0 0 0 .734-.215L8 9.06l1.97 1.97a.749.749 0 0 0 1.275-.326.749.749 0 0 0-.215-.734L9.06 8l1.97-1.97a.749.749 0 0 0-.326-1.275.749.749 0 0 0-.734.215L8 6.94Z"></path>
</svg>
</button>

      </div>
      <template id="search-icon"></template>

<template id="code-icon"></template>

<template id="file-code-icon"></template>

<template id="history-icon"></template>

<template id="repo-icon"></template>

<template id="bookmark-icon"></template>

<template id="plus-circle-icon"></template>

<template id="circle-icon"></template>

<template id="trash-icon"></template>

<template id="team-icon"></template>

<template id="project-icon"></template>

<template id="pencil-icon"></template>

<template id="copilot-icon"></template>

<template id="copilot-error-icon"></template>

<template id="workflow-icon"></template>

<template id="book-icon"></template>

<template id="code-review-icon"></template>

<template id="codespaces-icon"></template>

<template id="comment-icon"></template>

<template id="comment-discussion-icon"></template>

<template id="organization-icon"></template>

<template id="rocket-icon"></template>

<template id="shield-check-icon"></template>

<template id="heart-icon"></template>

<template id="server-icon"></template>

<template id="globe-icon"></template>

<template id="issue-opened-icon"></template>

<template id="device-mobile-icon"></template>

<template id="package-icon"></template>

<template id="credit-card-icon"></template>

<template id="play-icon"></template>

<template id="gift-icon"></template>

<template id="code-square-icon"></template>

<template id="device-desktop-icon"></template>

        <div class="position-relative">
                <ul role="listbox" class="ActionListWrap QueryBuilder-ListWrap" aria-label="Suggestions" data-action="
                    combobox-commit:query-builder#comboboxCommit
                    mousedown:query-builder#resultsMousedown
                  " data-target="query-builder.resultsList" data-persist-list="false" id="query-builder-test-results"></ul>
        </div>
      <div class="FormControl-inlineValidation" id="validation-c04f5b87-ff27-411b-9329-d2db08b85bcf" hidden="hidden">
        <span class="FormControl-inlineValidation--visual">
          <svg aria-hidden="true" height="12" viewBox="0 0 12 12" version="1.1" width="12" data-view-component="true" class="octicon octicon-alert-fill">
    <path d="M4.855.708c.5-.896 1.79-.896 2.29 0l4.675 8.351a1.312 1.312 0 0 1-1.146 1.954H1.33A1.313 1.313 0 0 1 .183 9.058ZM7 7V3H5v4Zm-1 3a1 1 0 1 0 0-2 1 1 0 0 0 0 2Z"></path>
</svg>
        </span>
        <span></span>
</div>    </div>
    <div data-target="query-builder.screenReaderFeedback" aria-live="polite" aria-atomic="true" class="sr-only">0 suggestions.</div>
</query-builder></form>
          <div class="d-flex flex-row color-fg-muted px-3 text-small color-bg-default search-feedback-prompt">
            <a target="_blank" href="https://docs.github.com/search-github/github-code-search/understanding-github-code-search-syntax" data-view-component="true" class="Link color-fg-accent text-normal ml-2">Search syntax tips</a>            <div class="d-flex flex-1"></div>
              <button data-action="click:qbsearch-input#showFeedbackDialog" type="button" data-view-component="true" class="Button--link Button--medium Button color-fg-accent text-normal ml-2">  <span class="Button-content">
    <span class="Button-label">Give feedback</span>
  </span>
</button>
          </div>
        </div>
</div>

    </div>
</modal-dialog></div>
  </div>
  <div data-action="click:qbsearch-input#retract" class="dark-backdrop position-fixed" hidden="" data-target="qbsearch-input.darkBackdrop"></div>
  <div class="color-fg-default">
    
<dialog-helper>
  <dialog data-target="qbsearch-input.feedbackDialog" data-action="close:qbsearch-input#handleDialogClose cancel:qbsearch-input#handleDialogClose" id="feedback-dialog" aria-modal="true" aria-labelledby="feedback-dialog-title" aria-describedby="feedback-dialog-description" data-view-component="true" class="Overlay Overlay-whenNarrow Overlay--size-medium Overlay--motion-scaleFade Overlay--disableScroll">
    <div data-view-component="true" class="Overlay-header">
  <div class="Overlay-headerContentWrap">
    <div class="Overlay-titleWrap">
      <h1 class="Overlay-title " id="feedback-dialog-title">
        Provide feedback
      </h1>
        
    </div>
    <div class="Overlay-actionWrap">
      <button data-close-dialog-id="feedback-dialog" aria-label="Close" type="button" data-view-component="true" class="close-button Overlay-closeButton"><svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path d="M3.72 3.72a.75.75 0 0 1 1.06 0L8 6.94l3.22-3.22a.749.749 0 0 1 1.275.326.749.749 0 0 1-.215.734L9.06 8l3.22 3.22a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215L8 9.06l-3.22 3.22a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042L6.94 8 3.72 4.78a.75.75 0 0 1 0-1.06Z"></path>
</svg></button>
    </div>
  </div>
  
</div>
      <scrollable-region data-labelled-by="feedback-dialog-title" data-catalyst="" style="overflow: auto;">
        <div data-view-component="true" class="Overlay-body">        <!-- '"` --><!-- </textarea></xmp> --><form id="code-search-feedback-form" data-turbo="false" action="https://github.com/search/feedback" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="pkOyrrCMy1D9699NavkjvXxeVefeiogq54QNoZhskEa_gqZNoDsnaoJRs76DDusJtvj1avadigdCH9JcW5Gxng">
          <p>We read every piece of feedback, and take your input very seriously.</p>
          <textarea name="feedback" class="form-control width-full mb-2" style="height: 120px" id="feedback"></textarea>
          <input name="include_email" id="include_email" aria-label="Include my email address so I can be contacted" class="form-control mr-2" type="checkbox">
          <label for="include_email" style="font-weight: normal">Include my email address so I can be contacted</label>
</form></div>
      </scrollable-region>
      <div data-view-component="true" class="Overlay-footer Overlay-footer--alignEnd">          <button data-close-dialog-id="feedback-dialog" type="button" data-view-component="true" class="btn">    Cancel
</button>
          <button form="code-search-feedback-form" data-action="click:qbsearch-input#submitFeedback" type="submit" data-view-component="true" class="btn-primary btn">    Submit feedback
</button>
</div>
</dialog></dialog-helper>

    <custom-scopes data-target="qbsearch-input.customScopesManager" data-catalyst="">
    
<dialog-helper>
  <dialog data-target="custom-scopes.customScopesModalDialog" data-action="close:qbsearch-input#handleDialogClose cancel:qbsearch-input#handleDialogClose" id="custom-scopes-dialog" aria-modal="true" aria-labelledby="custom-scopes-dialog-title" aria-describedby="custom-scopes-dialog-description" data-view-component="true" class="Overlay Overlay-whenNarrow Overlay--size-medium Overlay--motion-scaleFade Overlay--disableScroll">
    <div data-view-component="true" class="Overlay-header Overlay-header--divided">
  <div class="Overlay-headerContentWrap">
    <div class="Overlay-titleWrap">
      <h1 class="Overlay-title " id="custom-scopes-dialog-title">
        Saved searches
      </h1>
        <h2 id="custom-scopes-dialog-description" class="Overlay-description">Use saved searches to filter your results more quickly</h2>
    </div>
    <div class="Overlay-actionWrap">
      <button data-close-dialog-id="custom-scopes-dialog" aria-label="Close" type="button" data-view-component="true" class="close-button Overlay-closeButton"><svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path d="M3.72 3.72a.75.75 0 0 1 1.06 0L8 6.94l3.22-3.22a.749.749 0 0 1 1.275.326.749.749 0 0 1-.215.734L9.06 8l3.22 3.22a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215L8 9.06l-3.22 3.22a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042L6.94 8 3.72 4.78a.75.75 0 0 1 0-1.06Z"></path>
</svg></button>
    </div>
  </div>
  
</div>
      <scrollable-region data-labelled-by="custom-scopes-dialog-title" data-catalyst="" style="overflow: auto;">
        <div data-view-component="true" class="Overlay-body">        <div data-target="custom-scopes.customScopesModalDialogFlash"></div>

        <div hidden="" class="create-custom-scope-form" data-target="custom-scopes.createCustomScopeForm">
        <!-- '"` --><!-- </textarea></xmp> --><form id="custom-scopes-dialog-form" data-turbo="false" action="https://github.com/search/custom_scopes" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="2MQD-ldMdIPKudB-3tui0pA-WiiLbTP4Wro8dCuAP1Hlpw6Wtt4wEBPby2eYNacAl8NuCxGFKLYclEqt-upa6g">
          <div data-target="custom-scopes.customScopesModalDialogFlash"></div>

          <input type="hidden" id="custom_scope_id" name="custom_scope_id" data-target="custom-scopes.customScopesIdField">

          <div class="form-group">
            <label for="custom_scope_name">Name</label>
            <auto-check src="/search/custom_scopes/check_name" required="">
              <input type="text" name="custom_scope_name" id="custom_scope_name" data-target="custom-scopes.customScopesNameField" class="form-control" autocomplete="off" placeholder="github-ruby" required="" maxlength="50" spellcheck="false">
              <input type="hidden" value="nEI-NZGz5LLnSvqnZdAPIUKbo0hpjbKc2hs86kdBCKlKwXofIaTzUTmtZkhii1JqK0T9JdlPkiA65uHviAXB0Q" data-csrf="true">
            </auto-check>
          </div>

          <div class="form-group">
            <label for="custom_scope_query">Query</label>
            <input type="text" name="custom_scope_query" id="custom_scope_query" data-target="custom-scopes.customScopesQueryField" class="form-control" autocomplete="off" placeholder="(repo:mona/a OR repo:mona/b) AND lang:python" required="" maxlength="500">
          </div>

          <p class="text-small color-fg-muted">
            To see all available qualifiers, see our <a class="Link--inTextBlock" href="https://docs.github.com/search-github/github-code-search/understanding-github-code-search-syntax">documentation</a>.
          </p>
</form>        </div>

        <div data-target="custom-scopes.manageCustomScopesForm">
          <div data-target="custom-scopes.list"></div>
        </div>

</div>
      </scrollable-region>
      <div data-view-component="true" class="Overlay-footer Overlay-footer--alignEnd Overlay-footer--divided">          <button data-action="click:custom-scopes#customScopesCancel" type="button" data-view-component="true" class="btn">    Cancel
</button>
          <button form="custom-scopes-dialog-form" data-action="click:custom-scopes#customScopesSubmit" data-target="custom-scopes.customScopesSubmitButton" type="submit" data-view-component="true" class="btn-primary btn">    Create saved search
</button>
</div>
</dialog></dialog-helper>
    </custom-scopes>
  </div>
</qbsearch-input>  <input type="hidden" value="PU3ED0WjkA4tImxufQmSoizO10g1bgxeAu7ommJ585Mkeqcu4OtKyxg09hERIUAihiESPTMjTHrFswM44YDfgQ" data-csrf="true" class="js-data-jump-to-suggestions-path-csrf">


          </div>

        
          <div class="AppHeader-CopilotChat hide-sm hide-md">
  <react-partial-anchor data-catalyst="">
      <a href="https://github.com/copilot" data-target="react-partial-anchor.anchor" id="copilot-chat-header-button" aria-expanded="false" aria-controls="copilot-chat-panel" aria-labelledby="tooltip-e5a6e82d-b8b0-4a5d-96fa-b496f26ec4ff" data-view-component="true" class="Button Button--iconOnly Button--secondary Button--medium AppHeader-button AppHeader-buttonLeft">  <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copilot Button-visual">
    <path d="M7.998 15.035c-4.562 0-7.873-2.914-7.998-3.749V9.338c.085-.628.677-1.686 1.588-2.065.013-.07.024-.143.036-.218.029-.183.06-.384.126-.612-.201-.508-.254-1.084-.254-1.656 0-.87.128-1.769.693-2.484.579-.733 1.494-1.124 2.724-1.261 1.206-.134 2.262.034 2.944.765.05.053.096.108.139.165.044-.057.094-.112.143-.165.682-.731 1.738-.899 2.944-.765 1.23.137 2.145.528 2.724 1.261.566.715.693 1.614.693 2.484 0 .572-.053 1.148-.254 1.656.066.228.098.429.126.612.012.076.024.148.037.218.924.385 1.522 1.471 1.591 2.095v1.872c0 .766-3.351 3.795-8.002 3.795Zm0-1.485c2.28 0 4.584-1.11 5.002-1.433V7.862l-.023-.116c-.49.21-1.075.291-1.727.291-1.146 0-2.059-.327-2.71-.991A3.222 3.222 0 0 1 8 6.303a3.24 3.24 0 0 1-.544.743c-.65.664-1.563.991-2.71.991-.652 0-1.236-.081-1.727-.291l-.023.116v4.255c.419.323 2.722 1.433 5.002 1.433ZM6.762 2.83c-.193-.206-.637-.413-1.682-.297-1.019.113-1.479.404-1.713.7-.247.312-.369.789-.369 1.554 0 .793.129 1.171.308 1.371.162.181.519.379 1.442.379.853 0 1.339-.235 1.638-.54.315-.322.527-.827.617-1.553.117-.935-.037-1.395-.241-1.614Zm4.155-.297c-1.044-.116-1.488.091-1.681.297-.204.219-.359.679-.242 1.614.091.726.303 1.231.618 1.553.299.305.784.54 1.638.54.922 0 1.28-.198 1.442-.379.179-.2.308-.578.308-1.371 0-.765-.123-1.242-.37-1.554-.233-.296-.693-.587-1.713-.7Z"></path><path d="M6.25 9.037a.75.75 0 0 1 .75.75v1.501a.75.75 0 0 1-1.5 0V9.787a.75.75 0 0 1 .75-.75Zm4.25.75v1.501a.75.75 0 0 1-1.5 0V9.787a.75.75 0 0 1 1.5 0Z"></path>
</svg>
</a><tool-tip id="tooltip-e5a6e82d-b8b0-4a5d-96fa-b496f26ec4ff" for="copilot-chat-header-button" popover="manual" data-direction="s" data-type="label" data-view-component="true" class="sr-only position-absolute" aria-hidden="true" role="tooltip"><template shadowrootmode="open"><style>
      :host {
        --tooltip-top: var(--tool-tip-position-top, 0);
        --tooltip-left: var(--tool-tip-position-left, 0);
        padding: var(--overlay-paddingBlock-condensed) var(--overlay-padding-condensed) !important;
        font: var(--text-body-shorthand-small);
        color: var(--tooltip-fgColor, var(--fgColor-onEmphasis)) !important;
        text-align: center;
        text-decoration: none;
        text-shadow: none;
        text-transform: none;
        letter-spacing: normal;
        word-wrap: break-word;
        white-space: pre;
        background: var(--tooltip-bgColor, var(--bgColor-emphasis)) !important;
        border-radius: var(--borderRadius-medium);
        border: 0 !important;
        opacity: 0;
        max-width: var(--overlay-width-small);
        word-wrap: break-word;
        white-space: normal;
        width: max-content !important;
        inset: var(--tooltip-top) auto auto var(--tooltip-left) !important;
        overflow: visible !important;
        text-wrap: balance;
      }

      :host(:is(.tooltip-n, .tooltip-nw, .tooltip-ne)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) - var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(:is(.tooltip-s, .tooltip-sw, .tooltip-se)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) + var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(.tooltip-w) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) - var(--overlay-offset, 0.25rem));
      }

      :host(.tooltip-e) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) + var(--overlay-offset, 0.25rem));
      }

      :host:after{
        position: absolute;
        display: block;
        right: 0;
        left: 0;
        height: var(--overlay-offset, 0.25rem);
        content: "";
      }

      :host(.tooltip-s):after,
      :host(.tooltip-se):after,
      :host(.tooltip-sw):after {
        bottom: 100%
      }

      :host(.tooltip-n):after,
      :host(.tooltip-ne):after,
      :host(.tooltip-nw):after {
        top: 100%;
      }

      @keyframes tooltip-appear {
        from {
          opacity: 0;
        }
        to {
          opacity: 1;
        }
      }

      :host(:popover-open),
      :host(:popover-open):before {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      :host(.\:popover-open) {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      @media (forced-colors: active) {
        :host {
          outline: solid 1px transparent;
        }

        :host:before {
          display: none;
        }
      }
    </style><slot></slot></template>Chat with Copilot</tool-tip>

    
  
      <script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_tanstack_query-core_build_modern_queryObserver_js-node_modules_tanstack_-defd52-4fadb0b8d069.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_react-relay_index_js-9b3ae543a201.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_remark-gfm_lib_index_js-node_modules_remark-parse_lib_index_js-node_modu-44d0fc-eab34ca54a6e.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_highlight_js_es_core_js-node_modules_lowlight_lib_all_js-bdeb65237214.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_hastscript_lib_index_js-node_modules_react-markdown_lib_index_js-node_mo-68849e-79c2674e8a89.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_mini-throttle_dist_decorators_js-node_modules_accname_dist_access-690142-ee71f0becd82.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_combobox-nav_dist_index_js-node_modules_github_hotkey_dist_index_-9adaba-089d939a2d17.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_item-picker_components_RepositoryPicker_tsx-8698dae1910d.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_copilot-chat_utils_copilot-chat-helpers_ts-c1c42c1d11d6.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_copilot-markdown_MarkdownRenderer_tsx-d333d1cf771a.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_copilot-chat_utils_CopilotChatContext_tsx-b4c1810beefe.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_copilot-chat_components_CopilotIconAnimation_tsx-ui_packages_copilot-chat_compone-8be2e4-973264da89a2.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/copilot-chat-411b269e576f.js.download"></script>
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/primer-react.d2117d7623cc63123645.module.css">
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/copilot-chat.75b492a7f7731689f5ea.module.css">
      <link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/copilot-markdown-rendering-f6845e8f5d6b.css">
      <script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/primer-react-cf8d019de009.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/react-core-2e45a8c586a0.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/react-lib-248ff5a58e4e.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/octicons-react-9fd6ca6872cc.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_emotion_is-prop-valid_dist_emotion-is-prop-valid_esm_js-node_modules_emo-b1c483-9589ee80fc4f.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_catalyst_lib_index_js-node_modules_primer_live-region-element_dis-b2aea6-980db0e5dd58.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_dompurify_dist_purify_es_mjs-d13e3af1f7a5.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_tanstack_query-core_build_modern_queryObserver_js-node_modules_tanstack_-defd52-4fadb0b8d069.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_react-relay_index_js-9b3ae543a201.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_remark-gfm_lib_index_js-node_modules_remark-parse_lib_index_js-node_modu-44d0fc-eab34ca54a6e.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_highlight_js_es_core_js-node_modules_lowlight_lib_all_js-bdeb65237214.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_hastscript_lib_index_js-node_modules_react-markdown_lib_index_js-node_mo-68849e-79c2674e8a89.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_mini-throttle_dist_decorators_js-node_modules_accname_dist_access-690142-ee71f0becd82.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_focus-visible_dist_focus-visible_js-node_modules_github_hydro-analytics--e21ffd-34e19bb44764.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/vendors-node_modules_github_combobox-nav_dist_index_js-node_modules_github_hotkey_dist_index_-9adaba-089d939a2d17.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_paths_index_ts-08fcbb3f0e88.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_ui-commands_ui-commands_ts-eeddffae9643.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_item-picker_components_RepositoryPicker_tsx-8698dae1910d.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_copilot-chat_utils_copilot-chat-helpers_ts-c1c42c1d11d6.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_copilot-markdown_MarkdownRenderer_tsx-d333d1cf771a.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_copilot-chat_utils_CopilotChatContext_tsx-b4c1810beefe.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_copilot-chat_components_CopilotIconAnimation_tsx-ui_packages_copilot-chat_compone-8be2e4-973264da89a2.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/copilot-chat-411b269e576f.js.download"></script>
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/primer-react.d2117d7623cc63123645.module.css">
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/copilot-chat.75b492a7f7731689f5ea.module.css">

<react-partial partial-name="copilot-chat" data-ssr="false" data-attempted-ssr="false" data-catalyst="" class="loaded">
  
  <script type="application/json" data-target="react-partial.embeddedData">{"props":{"currentTopic":{"id":974415414,"name":"Module1","ownerLogin":"Kiran437228","ownerType":"User","readmePath":null,"description":null,"commitOID":"cd56a190f392faafdd7928aa78289c2d76b2abb8","ref":"refs/heads/main","refInfo":{"name":"main","type":"branch"},"visibility":"public","languages":[],"customInstructions":[]},"findFileWorkerPath":"/assets-cdn/worker/find-file-worker-263cab1760dd.js","renderPopover":false,"renderBetaLabel":false,"chatIsVisible":true,"chatVisibleSettingPath":"/users/dhashvanth21/copilot_chat/settings/copilot_chat_visibility","ssoOrganizations":[],"apiVersion":null,"agentsPath":"/github-copilot/chat/agents","apiURL":"https://api.individual.githubcopilot.com","currentUserLogin":"dhashvanth21","customInstructions":null,"renderKnowledgeBases":false,"optedInToPreviewFeatures":false,"optedInToUserFeedback":false,"renderAttachKnowledgeBaseHerePopover":true,"renderKnowledgeBaseAttachedToChatPopover":true,"personalInstructions":null,"reviewLab":false,"realIp":null,"scrollToTop":false,"hasCEorCBAccess":false,"licenseType":"unlicensed","plan":null,"quotas":null,"icebreakers":[{"type":"functional","data":[{"id":"open-issues-in-react","message":"Get a list of the latest open issues in the facebook/react repository, including all their labels.","titleHtml":"Open issues in \u003cspan class=\"fgColor-muted\"\u003efacebook/react\u003c/span\u003e","icon":"issue-opened","color":"var(--display-green-fgColor)"},{"id":"pulls-in-vscode","message":"Retrieve pull requests in microsoft/vscode.","titleHtml":"Pull requests in \u003cspan class=\"fgColor-muted\"\u003emicrosoft/vscode\u003c/span\u003e","icon":"git-pull-request","color":"var(--display-green-fgColor)"},{"id":"commits-in-linux","message":"Show recent commits in torvalds/linux.","titleHtml":"Recent commits in \u003cspan class=\"fgColor-muted\"\u003etorvalds/linux\u003c/span\u003e","icon":"git-commit","color":"var(--display-blue-fgColor)"},{"id":"my-latest-issues","message":"Find the five latest issues assigned to me.","titleHtml":"Find issues assigned to me","icon":"issue-opened","color":"var(--display-green-fgColor)"},{"id":"latest-node-release","message":"Fetch the latest release of nodejs/node and highlight the changes.","titleHtml":"Latest \u003cspan class=\"fgColor-muted\"\u003enodejs/node\u003c/span\u003e release","icon":"tag","color":"var(--display-purple-fgColor)"},{"id":"create-profile-readme","message":"Create a profile README for $$USERNAME$$.","titleHtml":"Create a profile README for me","icon":"rocket","color":"var(--display-pink-fgColor)"},{"id":"bugs-in-primer","message":"Show recent bugs in primer/react.","titleHtml":"Recent bugs in \u003cspan class=\"fgColor-muted\"\u003eprimer/react\u003c/span\u003e","icon":"bug","color":"var(--display-purple-fgColor)"},{"id":"my-open-pulls","message":"Find my open pull requests.","titleHtml":"My open pull requests","icon":"git-pull-request","color":"var(--display-green-fgColor)"},{"id":"generate-html-calculator","message":"Generate a simple calculator using HTML, CSS, and JavaScript.","titleHtml":"Generate an HTML/JS calculator","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"python-strong-password-endpoint","message":"Generate a Python endpoint for signing up that only allows strong passwords.","titleHtml":"Python password endpoint","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"rails-auth-endpoint","message":"Generate a Rails endpoint for authenticating with email and password.","titleHtml":"Rails authentication endpoint","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"python-pandas-data-analysis","message":"Write a Python script that analyzes a dataset using Pandas.","titleHtml":"Python Panda data analysis","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"explain-restful-basics","message":"Explain REST architectural principles and how to implement RESTful web services.","titleHtml":"Explain RESTful basics","icon":"book","color":"var(--display-blue-fgColor)"},{"id":"compare-http-post-vs-put","message":"Compare HTTP POST and PUT methods, explaining their proper usage in RESTful APIs.","titleHtml":"Compare HTTP POST vs PUT","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"explain-json-content-types","message":"Explain proper JSON MIME types and content-type headers for different scenarios and platforms.","titleHtml":"Explain JSON content types","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"compare-dates-and-times","message":"Explain strategies for accurately comparing dates and times across different timezones and formats.","titleHtml":"Compare dates and times","icon":"clock","color":"var(--display-blue-fgColor)"},{"id":"compare-json-comment-options","message":"Explain JSON syntax limitations regarding comments and alternative approaches for documentation.","titleHtml":"Compare JSON comment options","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"explain-stack-and-heap-memory","message":"Compare stack and heap memory allocation, their characteristics, and use cases in programming.","titleHtml":"Explain stack and heap memory","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"compare-api-version-strategies","message":"Explain different approaches to API versioning including URL, header, and content negotiation.","titleHtml":"Compare API version strategies","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"how-to-fix-git-submodules","message":"Troubleshoot and resolve issues with uninitialized Git submodules, explaining initialization commands and common pitfalls.","titleHtml":"How to fix Git submodules","icon":"git-merge","color":"var(--display-green-fgColor)"},{"id":"compare-git-fork-and-clone","message":"Compare and contrast Git clones versus forks, explaining their technical differences, use cases, and relationship to original repositories.","titleHtml":"Compare Git fork and clone","icon":"git-branch","color":"var(--display-green-fgColor)"},{"id":"explain-pull-request-basics","message":"Walk through the complete process of creating, submitting, and managing pull requests on GitHub, from forking to merging.","titleHtml":"Explain pull request basics","icon":"git-pull-request","color":"var(--display-green-fgColor)"},{"id":"git-history-cleanup-guide","message":"Provide a complete guide to permanently removing files from Git history, including BFG and filter-repo approaches with safety considerations.","titleHtml":"Git history cleanup guide","icon":"trash","color":"var(--display-blue-fgColor)"},{"id":"git-credential-management","message":"Explain the different methods for caching HTTPS credentials when pushing Git commits, including credential helpers, personal access tokens, and their security implications.","titleHtml":"Git credential management","icon":"key","color":"var(--display-purple-fgColor)"},{"id":"compare-origin-and-upstream","message":"Explain the conceptual and functional differences between origin and upstream remote repositories in Git, with examples of how they're used in workflow.","titleHtml":"Compare origin and upstream","icon":"git-branch","color":"var(--display-green-fgColor)"},{"id":"how-to-download-github-folders","message":"Describe various methods to download specific folders from GitHub repositories without cloning the entire project.","titleHtml":"How to download GitHub folders","icon":"download","color":"var(--display-blue-fgColor)"},{"id":"git-path-configurations","message":"Provide cross-platform instructions for properly configuring GitHub Desktop to include Git in the system PATH, enabling command-line Git operations alongside the GUI client on Windows, macOS, and Linux systems.","titleHtml":"Git PATH configurations","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"explain-fork-sync-process","message":"Provide step-by-step instructions for synchronizing a forked GitHub repository with its original upstream repository, including both command line methods and GitHub interface options.","titleHtml":"Explain fork sync process","icon":"git-merge","color":"var(--display-green-fgColor)"},{"id":"list-git-history-danger-zones","message":"List and explain potentially dangerous Git commands that can alter repository history, with guidelines on when and how to use them safely.","titleHtml":"List Git history danger zones","icon":"history","color":"var(--display-blue-fgColor)"},{"id":"explain-cli-repository-setup","message":"Explain methods for creating GitHub repositories entirely from the command line using GitHub CLI, API tokens, and other headless approaches.","titleHtml":"Explain CLI repository setup","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"how-to-migrate-git-remote","message":"Detail the process of migrating an existing Git repository to a different remote server while preserving history, branches, and tags, with command examples.","titleHtml":"How to migrate Git remote","icon":"git-commit","color":"var(--display-blue-fgColor)"},{"id":"compare-git-and-github","message":"Explain the fundamental differences between Git (the distributed version control system) and GitHub (the web-based hosting service), clarifying their relationship, unique features, and how they complement each other in modern development workflows.","titleHtml":"Compare Git and GitHub","icon":"git-branch","color":"var(--display-green-fgColor)"},{"id":"learn-git-multi-remote-setup","message":"Explain the process of configuring a Git repository to push commits simultaneously to multiple remote repositories, including setting up multiple remotes and creating automated push workflows.","titleHtml":"Learn Git multi remote setup","icon":"git-commit","color":"var(--display-blue-fgColor)"},{"id":"convert-single-branch-clone","message":"Explain methods for converting a single-branch Git clone into a full repository clone with access to all remote branches, including fetch commands and configuration changes.","titleHtml":"Convert single branch clone","icon":"git-branch","color":"var(--display-green-fgColor)"},{"id":"multiple-github-account-guide","message":"Provide step-by-step instructions for configuring and managing multiple GitHub accounts on a single computer, including SSH key setup and Git configuration.","titleHtml":"Multiple GitHub account guide","icon":"mark-github","color":"var(--display-purple-fgColor)"},{"id":"explore-java-map-iterations","message":"Compare different methods for efficiently iterating over Map entries in Java.","titleHtml":"Explore Java Map Iterations","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"understand-java-access-levels","message":"Explain differences between Java's access modifiers with practical examples.","titleHtml":"Understand Java access levels","icon":"lock","color":"var(--display-purple-fgColor)"},{"id":"compare-java-password-types","message":"Compare char[] vs String for password storage in Java with security implications.","titleHtml":"Compare Java password types","icon":"key","color":"var(--display-purple-fgColor)"},{"id":"compare-java-hashmap-hashtable","message":"Compare HashMap and Hashtable in Java, explaining their key differences including thread safety, null handling, synchronization overhead, and performance characteristics with practical examples.","titleHtml":"Compare Java HashMap/Hashtable","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"learn-java-array-sorting-perf","message":"Explain how CPU branch prediction and cache optimization affect Java array processing performance, demonstrating the speed difference between sorted and unsorted arrays with examples.","titleHtml":"Learn Java array sorting perf","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"java-operator-casting-basics","message":"Explain why compound assignment operators in Java don't require explicit casting.","titleHtml":"Java operator casting basics","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"explain-java-char-for-password","message":"Explain why char[] is preferred over String for passwords in Java, including security implications.","titleHtml":"Explain Java char[] for password","icon":"key","color":"var(--display-purple-fgColor)"},{"id":"compare-java-pass-by-value-ref","message":"Explain whether Java is pass-by-reference or pass-by-value with examples.","titleHtml":"Compare Java pass by value/ref","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"learn-js-import-patterns","message":"Explain different approaches to importing JavaScript files, including modern ES6 modules.","titleHtml":"Learn JS import patterns","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"explore-js-array-loops","message":"Compare different methods for iterating over arrays in JavaScript with use cases.","titleHtml":"Explore JS array loops","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"understand-js-strict-mode-usage","message":"Explain the purpose and benefits of strict mode in JavaScript, including common pitfalls it prevents.","titleHtml":"Understand JS strict mode usage","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"learn-js-closures","message":"Explain JavaScript closure concept with practical examples showing scope and data privacy.","titleHtml":"Learn JS closures","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"compare-js-equality-operators","message":"Compare the behavior and use cases of == and === operators in JavaScript, explaining type coercion and best practices.","titleHtml":"Compare JS equality operators","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"learn-js-sleep-function","message":"Explain how to implement delay/sleep functionality in JavaScript using promises and async/await.","titleHtml":"Learn JS sleep function","icon":"clock","color":"var(--display-blue-fgColor)"},{"id":"compare-js-substring-checks","message":"Compare methods for checking substrings in JavaScript strings, with performance considerations.","titleHtml":"Compare JS substring checks","icon":"search","color":"var(--display-blue-fgColor)"},{"id":"how-to-handle-js-async-response","message":"Explain handling asynchronous operations in JavaScript using promises, async/await, and callbacks.","titleHtml":"How to handle JS async response","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"python-slice-syntax","message":"Explain Python's list slicing syntax, including step values and negative indices.","titleHtml":"Python slice syntax","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"how-to-flatten-lists-in-python","message":"Compare methods for flattening nested lists in Python, from simple to complex cases.","titleHtml":"How to flatten lists in Python","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"learn-python-main-check","message":"Explain the purpose and usage of if name == \"main\" in Python, including module behavior and best practices.","titleHtml":"Learn Python main check","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"python-env-variables-guide","message":"Explain how to access and manage environment variables in Python applications.","titleHtml":"Python env variables guide","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"learn-python-star-operators","message":"Explain the difference between single and double asterisk operators in Python for parameter packing and unpacking.","titleHtml":"Learn Python star operators","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"explain-python-yield","message":"Explain Python generators and the yield keyword with examples of memory-efficient iteration.","titleHtml":"Explain Python yield","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"python-variable-passing-guide","message":"Explain Python's pass-by-object-reference behavior with examples of mutable and immutable objects.","titleHtml":"Python variable passing guide","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"generate-curl-json-post","message":"Demonstrate how to send JSON data using cURL, including headers and authentication.","titleHtml":"Generate cURL JSON POST","icon":"terminal","color":"var(--display-gray-fgColor)"},{"id":"show-linux-text-search","message":"Demonstrate commands and techniques for searching text within files on Linux systems.","titleHtml":"Show Linux text search","icon":"search","color":"var(--display-blue-fgColor)"},{"id":"learn-to-check-visibility-in-js","message":"Demonstrate methods for detecting hidden elements in JavaScript, including various visibility states.","titleHtml":"Learn to check visibility in JS","icon":"eye","color":"var(--display-purple-fgColor)"},{"id":"find-bash-script-location","message":"Show methods for determining a Bash script's directory location during execution.","titleHtml":"Find Bash script location","icon":"terminal","color":"var(--display-gray-fgColor)"},{"id":"explain-special-char-escape","message":"Demonstrate different methods for escaping special characters in various programming contexts.","titleHtml":"Explain special char escape","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"show-directory-exists","message":"Show different methods for checking directory existence in Bash with error handling.","titleHtml":"Show directory exists","icon":"terminal","color":"var(--display-gray-fgColor)"},{"id":"webpage-redirect-methods","message":"Show different techniques for implementing webpage redirects using HTML, JavaScript and server-side approaches.","titleHtml":"Webpage redirect methods","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"branch-sync-patterns","message":"Demonstrate Git commands for synchronizing branches, including reset, rebase, and merge techniques with their implications.","titleHtml":"Branch sync patterns","icon":"git-merge","color":"var(--display-green-fgColor)"},{"id":"how-to-recover-deleted-git-files","message":"Demonstrate techniques for locating and recovering files that were deleted in previous commits, including Git log commands, filtering options, and restoration methods.","titleHtml":"How to recover deleted Git files","icon":"history","color":"var(--display-blue-fgColor)"},{"id":"how-to-load-remote-js-script","message":"Provide code examples and best practices for linking to and executing JavaScript files hosted on GitHub in web applications.","titleHtml":"How to load remote JS script","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"how-to-npm-install-from-github","message":"Demonstrate different methods for installing npm packages directly from GitHub repositories, including syntax examples and troubleshooting tips.","titleHtml":"How to npm install from GitHub","icon":"package","color":"var(--display-blue-fgColor)"},{"id":"demo-java-linkedlist-arraylist","message":"Show different methods for initializing ArrayLists in Java in a single line.","titleHtml":"Demo Java LinkedList/ArrayList","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"learn-java-memory-issues","message":"Demonstrate common causes of memory leaks in Java and how to prevent them.","titleHtml":"Learn Java memory issues","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"learn-java-stream-conversion","message":"Show different methods for converting an InputStream to a String in Java, comparing performance.","titleHtml":"Learn Java stream conversion","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"java-null-handling-patterns","message":"Demonstrate best practices for handling null values in Java using Optional and other patterns.","titleHtml":"Java null handling patterns","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"java-list-conversion-guide","message":"Show different approaches to convert arrays to ArrayLists in Java with examples.","titleHtml":"Java List conversion guide","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"js-email-validation-guide","message":"Demonstrate robust email validation techniques in JavaScript, from regex patterns to validation APIs.","titleHtml":"JS email validation guide","icon":"mail","color":"var(--display-blue-fgColor)"},{"id":"prototype-js-array-iteration","message":"Demonstrate methods for removing specific items from JavaScript arrays with examples.","titleHtml":"Prototype JS array iteration","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"explore-js-object-checks","message":"Show different methods for detecting empty objects in JavaScript, considering various edge cases.","titleHtml":"Explore JS object checks","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"how-to-js-remove-object-props","message":"Demonstrate different methods for removing properties from JavaScript objects and their implications.","titleHtml":"How to JS remove object props","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"how-to-merge-python-dicts","message":"Show different methods for merging Python dictionaries, including dictionary unpacking and update methods.","titleHtml":"How to merge Python dicts","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"explore-python-ternary-syntax","message":"Demonstrate Python's ternary conditional operator with examples comparing it to traditional if-else statements.","titleHtml":"Explore Python ternary syntax","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"demo-python-loop-with-index","message":"Demonstrate different ways to access index values in Python for loops using enumerate and range.","titleHtml":"Demo Python loop with index","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"demo-sorting-python-dictionary","message":"Demonstrate methods for sorting Python dictionaries by values using different approaches and sorting criteria.","titleHtml":"Demo sorting Python dictionary","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"learn-python-file-checks","message":"Show methods for checking file existence in Python without raising exceptions.","titleHtml":"Learn Python file checks","icon":"file","color":"var(--display-blue-fgColor)"},{"id":"demo-python-run-system-command","message":"Demonstrate various methods for executing system commands in Python using subprocess and other modules.","titleHtml":"Demo Python run system command","icon":"terminal","color":"var(--display-gray-fgColor)"},{"id":"compare-python-method-decorators","message":"Compare @staticmethod and @classmethod decorators in Python, explaining their use cases.","titleHtml":"Compare Python method decorators","icon":"code","color":"var(--display-gray-fgColor)"}]},{"type":"instructional","data":[{"id":"what-can-i-do-with-github-copilot-chat","message":"What can I do with GitHub Copilot Chat?","titleHtml":"What can I do here?","icon":"light-bulb","color":"var(--display-purple-fgColor)"}]},{"type":"interactional","data":[{"id":"to-do-app-local-storage","message":"Create a to-do list application with local storage functionality.","titleHtml":"To-do list with local storage","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"digital-clock-time-zones","message":"Create a digital clock that displays the current time in different time zones.","titleHtml":"A digital time zone clock","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"weather-dashboard-app","message":"Develop a weather dashboard that fetches data from a public weather API.","titleHtml":"Develop a weather dashboard","icon":"code","color":"var(--display-gray-fgColor)"},{"id":"create-joke-generator","message":"Create a random joke generator using an external API.","titleHtml":"Create a joke generator","icon":"code","color":"var(--display-gray-fgColor)"}]}],"canShareThread":true}}</script>
  <div data-target="react-partial.reactRoot"><div class="Box-sc-g0xbh4-0 bpDFns"></div><div class="Box-sc-g0xbh4-0 hmHhrt"></div><script type="application/json" id="__PRIMER_DATA_:r7o:__">{"resolvedServerColorMode":"night"}</script></div>
</react-partial>


    </react-partial-anchor>
  <react-partial-anchor data-catalyst="">
    <button id="global-copilot-menu-button" data-target="react-partial-anchor.anchor" aria-expanded="false" aria-labelledby="tooltip-ab340ecd-a5e2-4a75-ac79-b9305ebcc08f" type="button" data-view-component="true" class="Button Button--iconOnly Button--secondary Button--medium AppHeader-button AppHeader-buttonRight" aria-haspopup="true">  <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-triangle-down Button-visual">
    <path d="m4.427 7.427 3.396 3.396a.25.25 0 0 0 .354 0l3.396-3.396A.25.25 0 0 0 11.396 7H4.604a.25.25 0 0 0-.177.427Z"></path>
</svg>
</button><tool-tip id="tooltip-ab340ecd-a5e2-4a75-ac79-b9305ebcc08f" for="global-copilot-menu-button" popover="manual" data-direction="s" data-type="label" data-view-component="true" class="sr-only position-absolute" aria-hidden="true" role="tooltip"><template shadowrootmode="open"><style>
      :host {
        --tooltip-top: var(--tool-tip-position-top, 0);
        --tooltip-left: var(--tool-tip-position-left, 0);
        padding: var(--overlay-paddingBlock-condensed) var(--overlay-padding-condensed) !important;
        font: var(--text-body-shorthand-small);
        color: var(--tooltip-fgColor, var(--fgColor-onEmphasis)) !important;
        text-align: center;
        text-decoration: none;
        text-shadow: none;
        text-transform: none;
        letter-spacing: normal;
        word-wrap: break-word;
        white-space: pre;
        background: var(--tooltip-bgColor, var(--bgColor-emphasis)) !important;
        border-radius: var(--borderRadius-medium);
        border: 0 !important;
        opacity: 0;
        max-width: var(--overlay-width-small);
        word-wrap: break-word;
        white-space: normal;
        width: max-content !important;
        inset: var(--tooltip-top) auto auto var(--tooltip-left) !important;
        overflow: visible !important;
        text-wrap: balance;
      }

      :host(:is(.tooltip-n, .tooltip-nw, .tooltip-ne)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) - var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(:is(.tooltip-s, .tooltip-sw, .tooltip-se)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) + var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(.tooltip-w) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) - var(--overlay-offset, 0.25rem));
      }

      :host(.tooltip-e) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) + var(--overlay-offset, 0.25rem));
      }

      :host:after{
        position: absolute;
        display: block;
        right: 0;
        left: 0;
        height: var(--overlay-offset, 0.25rem);
        content: "";
      }

      :host(.tooltip-s):after,
      :host(.tooltip-se):after,
      :host(.tooltip-sw):after {
        bottom: 100%
      }

      :host(.tooltip-n):after,
      :host(.tooltip-ne):after,
      :host(.tooltip-nw):after {
        top: 100%;
      }

      @keyframes tooltip-appear {
        from {
          opacity: 0;
        }
        to {
          opacity: 1;
        }
      }

      :host(:popover-open),
      :host(:popover-open):before {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      :host(.\:popover-open) {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      @media (forced-colors: active) {
        :host {
          outline: solid 1px transparent;
        }

        :host:before {
          display: none;
        }
      }
    </style><slot></slot></template>Open Copilot…</tool-tip>

    
  
      <script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/global-copilot-menu-4d8af0507df1.js.download"></script>
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/primer-react.d2117d7623cc63123645.module.css">
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/global-copilot-menu.b973d595584666020636.module.css">

<react-partial partial-name="global-copilot-menu" data-ssr="false" data-attempted-ssr="false" data-catalyst="" class="loaded">
  
  <script type="application/json" data-target="react-partial.embeddedData">{"props":{}}</script>
  <div data-target="react-partial.reactRoot"><div class="d-none"></div><script type="application/json" id="__PRIMER_DATA_:r7f:__">{"resolvedServerColorMode":"night"}</script></div>
</react-partial>

    </react-partial-anchor>
</div>


        <div class="AppHeader-actions position-relative">
             <react-partial-anchor data-catalyst="">
      <button id="global-create-menu-anchor" aria-label="Create something new" data-target="react-partial-anchor.anchor" type="button" data-view-component="true" class="AppHeader-button global-create-button Button--secondary Button--medium Button width-auto color-fg-muted" aria-describedby="tooltip-d3186c9f-411d-4122-983c-777e668d084d" aria-expanded="false" aria-haspopup="true">  <span class="Button-content">
      <span class="Button-visual Button-leadingVisual">
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-plus">
    <path d="M7.75 2a.75.75 0 0 1 .75.75V7h4.25a.75.75 0 0 1 0 1.5H8.5v4.25a.75.75 0 0 1-1.5 0V8.5H2.75a.75.75 0 0 1 0-1.5H7V2.75A.75.75 0 0 1 7.75 2Z"></path>
</svg>
      </span>
    <span class="Button-label"><svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-triangle-down">
    <path d="m4.427 7.427 3.396 3.396a.25.25 0 0 0 .354 0l3.396-3.396A.25.25 0 0 0 11.396 7H4.604a.25.25 0 0 0-.177.427Z"></path>
</svg></span>
  </span>
</button><tool-tip id="tooltip-d3186c9f-411d-4122-983c-777e668d084d" for="global-create-menu-anchor" popover="manual" data-direction="s" data-type="description" data-view-component="true" class="sr-only position-absolute" role="tooltip"><template shadowrootmode="open"><style>
      :host {
        --tooltip-top: var(--tool-tip-position-top, 0);
        --tooltip-left: var(--tool-tip-position-left, 0);
        padding: var(--overlay-paddingBlock-condensed) var(--overlay-padding-condensed) !important;
        font: var(--text-body-shorthand-small);
        color: var(--tooltip-fgColor, var(--fgColor-onEmphasis)) !important;
        text-align: center;
        text-decoration: none;
        text-shadow: none;
        text-transform: none;
        letter-spacing: normal;
        word-wrap: break-word;
        white-space: pre;
        background: var(--tooltip-bgColor, var(--bgColor-emphasis)) !important;
        border-radius: var(--borderRadius-medium);
        border: 0 !important;
        opacity: 0;
        max-width: var(--overlay-width-small);
        word-wrap: break-word;
        white-space: normal;
        width: max-content !important;
        inset: var(--tooltip-top) auto auto var(--tooltip-left) !important;
        overflow: visible !important;
        text-wrap: balance;
      }

      :host(:is(.tooltip-n, .tooltip-nw, .tooltip-ne)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) - var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(:is(.tooltip-s, .tooltip-sw, .tooltip-se)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) + var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(.tooltip-w) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) - var(--overlay-offset, 0.25rem));
      }

      :host(.tooltip-e) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) + var(--overlay-offset, 0.25rem));
      }

      :host:after{
        position: absolute;
        display: block;
        right: 0;
        left: 0;
        height: var(--overlay-offset, 0.25rem);
        content: "";
      }

      :host(.tooltip-s):after,
      :host(.tooltip-se):after,
      :host(.tooltip-sw):after {
        bottom: 100%
      }

      :host(.tooltip-n):after,
      :host(.tooltip-ne):after,
      :host(.tooltip-nw):after {
        top: 100%;
      }

      @keyframes tooltip-appear {
        from {
          opacity: 0;
        }
        to {
          opacity: 1;
        }
      }

      :host(:popover-open),
      :host(:popover-open):before {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      :host(.\:popover-open) {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      @media (forced-colors: active) {
        :host {
          outline: solid 1px transparent;
        }

        :host:before {
          display: none;
        }
      }
    </style><slot></slot></template>Create new...</tool-tip>

      
    
        <script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/ui_packages_document-metadata_document-metadata_ts-ui_packages_promise-with-resolvers-polyfil-b81d9e-a079b289fa52.js.download"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/global-create-menu-c0e8b2269991.js.download"></script>
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/primer-react.d2117d7623cc63123645.module.css">
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/global-create-menu.b1ee6a6bae56a89148b1.module.css">

<react-partial partial-name="global-create-menu" data-ssr="false" data-attempted-ssr="false" data-catalyst="" class="loaded">
  
  <script type="application/json" data-target="react-partial.embeddedData">{"props":{"createRepo":true,"importRepo":true,"codespaces":true,"spark":false,"gist":true,"createOrg":true,"createProject":false,"createProjectUrl":"/dhashvanth21?tab=projects","createLegacyProject":false,"createIssue":false,"org":null,"owner":"Kiran437228","repo":"Module1"}}</script>
  <div data-target="react-partial.reactRoot"><script type="application/json" id="__PRIMER_DATA_:r7j:__">{"resolvedServerColorMode":"night"}</script></div>
</react-partial>

      </react-partial-anchor>


            <a href="https://github.com/issues" data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;ISSUES_HEADER&quot;,&quot;label&quot;:null}" id="icon-button-a9303f1b-c93d-44ca-aa7b-513d293c34ad" aria-labelledby="tooltip-1e82e8d7-242a-4142-ae61-8e0ee67ac124" data-view-component="true" class="Button Button--iconOnly Button--secondary Button--medium AppHeader-button color-fg-muted">  <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-issue-opened Button-visual">
    <path d="M8 9.5a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Z"></path><path d="M8 0a8 8 0 1 1 0 16A8 8 0 0 1 8 0ZM1.5 8a6.5 6.5 0 1 0 13 0 6.5 6.5 0 0 0-13 0Z"></path>
</svg>
</a><tool-tip id="tooltip-1e82e8d7-242a-4142-ae61-8e0ee67ac124" for="icon-button-a9303f1b-c93d-44ca-aa7b-513d293c34ad" popover="manual" data-direction="s" data-type="label" data-view-component="true" class="sr-only position-absolute" aria-hidden="true" role="tooltip"><template shadowrootmode="open"><style>
      :host {
        --tooltip-top: var(--tool-tip-position-top, 0);
        --tooltip-left: var(--tool-tip-position-left, 0);
        padding: var(--overlay-paddingBlock-condensed) var(--overlay-padding-condensed) !important;
        font: var(--text-body-shorthand-small);
        color: var(--tooltip-fgColor, var(--fgColor-onEmphasis)) !important;
        text-align: center;
        text-decoration: none;
        text-shadow: none;
        text-transform: none;
        letter-spacing: normal;
        word-wrap: break-word;
        white-space: pre;
        background: var(--tooltip-bgColor, var(--bgColor-emphasis)) !important;
        border-radius: var(--borderRadius-medium);
        border: 0 !important;
        opacity: 0;
        max-width: var(--overlay-width-small);
        word-wrap: break-word;
        white-space: normal;
        width: max-content !important;
        inset: var(--tooltip-top) auto auto var(--tooltip-left) !important;
        overflow: visible !important;
        text-wrap: balance;
      }

      :host(:is(.tooltip-n, .tooltip-nw, .tooltip-ne)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) - var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(:is(.tooltip-s, .tooltip-sw, .tooltip-se)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) + var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(.tooltip-w) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) - var(--overlay-offset, 0.25rem));
      }

      :host(.tooltip-e) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) + var(--overlay-offset, 0.25rem));
      }

      :host:after{
        position: absolute;
        display: block;
        right: 0;
        left: 0;
        height: var(--overlay-offset, 0.25rem);
        content: "";
      }

      :host(.tooltip-s):after,
      :host(.tooltip-se):after,
      :host(.tooltip-sw):after {
        bottom: 100%
      }

      :host(.tooltip-n):after,
      :host(.tooltip-ne):after,
      :host(.tooltip-nw):after {
        top: 100%;
      }

      @keyframes tooltip-appear {
        from {
          opacity: 0;
        }
        to {
          opacity: 1;
        }
      }

      :host(:popover-open),
      :host(:popover-open):before {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      :host(.\:popover-open) {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      @media (forced-colors: active) {
        :host {
          outline: solid 1px transparent;
        }

        :host:before {
          display: none;
        }
      }
    </style><slot></slot></template>Your issues</tool-tip>

            <a href="https://github.com/pulls" data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;PULL_REQUESTS_HEADER&quot;,&quot;label&quot;:null}" id="icon-button-ece11e0b-f663-45bb-984b-657227cba57d" aria-labelledby="tooltip-7a80b61b-506d-4785-a34f-63b68160b655" data-view-component="true" class="Button Button--iconOnly Button--secondary Button--medium AppHeader-button color-fg-muted">  <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-git-pull-request Button-visual">
    <path d="M1.5 3.25a2.25 2.25 0 1 1 3 2.122v5.256a2.251 2.251 0 1 1-1.5 0V5.372A2.25 2.25 0 0 1 1.5 3.25Zm5.677-.177L9.573.677A.25.25 0 0 1 10 .854V2.5h1A2.5 2.5 0 0 1 13.5 5v5.628a2.251 2.251 0 1 1-1.5 0V5a1 1 0 0 0-1-1h-1v1.646a.25.25 0 0 1-.427.177L7.177 3.427a.25.25 0 0 1 0-.354ZM3.75 2.5a.75.75 0 1 0 0 1.5.75.75 0 0 0 0-1.5Zm0 9.5a.75.75 0 1 0 0 1.5.75.75 0 0 0 0-1.5Zm8.25.75a.75.75 0 1 0 1.5 0 .75.75 0 0 0-1.5 0Z"></path>
</svg>
</a><tool-tip id="tooltip-7a80b61b-506d-4785-a34f-63b68160b655" for="icon-button-ece11e0b-f663-45bb-984b-657227cba57d" popover="manual" data-direction="s" data-type="label" data-view-component="true" class="sr-only position-absolute" aria-hidden="true" role="tooltip"><template shadowrootmode="open"><style>
      :host {
        --tooltip-top: var(--tool-tip-position-top, 0);
        --tooltip-left: var(--tool-tip-position-left, 0);
        padding: var(--overlay-paddingBlock-condensed) var(--overlay-padding-condensed) !important;
        font: var(--text-body-shorthand-small);
        color: var(--tooltip-fgColor, var(--fgColor-onEmphasis)) !important;
        text-align: center;
        text-decoration: none;
        text-shadow: none;
        text-transform: none;
        letter-spacing: normal;
        word-wrap: break-word;
        white-space: pre;
        background: var(--tooltip-bgColor, var(--bgColor-emphasis)) !important;
        border-radius: var(--borderRadius-medium);
        border: 0 !important;
        opacity: 0;
        max-width: var(--overlay-width-small);
        word-wrap: break-word;
        white-space: normal;
        width: max-content !important;
        inset: var(--tooltip-top) auto auto var(--tooltip-left) !important;
        overflow: visible !important;
        text-wrap: balance;
      }

      :host(:is(.tooltip-n, .tooltip-nw, .tooltip-ne)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) - var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(:is(.tooltip-s, .tooltip-sw, .tooltip-se)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) + var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(.tooltip-w) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) - var(--overlay-offset, 0.25rem));
      }

      :host(.tooltip-e) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) + var(--overlay-offset, 0.25rem));
      }

      :host:after{
        position: absolute;
        display: block;
        right: 0;
        left: 0;
        height: var(--overlay-offset, 0.25rem);
        content: "";
      }

      :host(.tooltip-s):after,
      :host(.tooltip-se):after,
      :host(.tooltip-sw):after {
        bottom: 100%
      }

      :host(.tooltip-n):after,
      :host(.tooltip-ne):after,
      :host(.tooltip-nw):after {
        top: 100%;
      }

      @keyframes tooltip-appear {
        from {
          opacity: 0;
        }
        to {
          opacity: 1;
        }
      }

      :host(:popover-open),
      :host(:popover-open):before {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      :host(.\:popover-open) {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      @media (forced-colors: active) {
        :host {
          outline: solid 1px transparent;
        }

        :host:before {
          display: none;
        }
      }
    </style><slot></slot></template>Your pull requests</tool-tip>

        </div>

          <notification-indicator data-channel="eyJjIjoibm90aWZpY2F0aW9uLWNoYW5nZWQ6MTgyMzM4MDMzIiwidCI6MTc0NzI0OTI2NX0=--2445a9b5203abc7c23e3192db827c194184a371a572692610fd0ba0eb9727b2a" data-indicator-mode="none" data-tooltip-global="You have unread notifications" data-tooltip-unavailable="Notifications are unavailable at the moment." data-tooltip-none="You have no unread notifications" data-header-redesign-enabled="true" data-fetch-indicator-src="/notifications/indicator" data-fetch-indicator-enabled="true" data-view-component="true" class="js-socket-channel" data-fetch-retry-delay-time="500" data-catalyst="">
    <a id="AppHeader-notifications-button" href="https://github.com/notifications" aria-labelledby="notification-indicator-tooltip" data-hotkey="g n" data-target="notification-indicator.link" data-analytics-event="{&quot;category&quot;:&quot;Global navigation&quot;,&quot;action&quot;:&quot;NOTIFICATIONS_HEADER&quot;,&quot;label&quot;:&quot;icon:read&quot;}" data-view-component="true" class="Button Button--iconOnly Button--secondary Button--medium AppHeader-button color-fg-muted">  <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-inbox Button-visual">
    <path d="M2.8 2.06A1.75 1.75 0 0 1 4.41 1h7.18c.7 0 1.333.417 1.61 1.06l2.74 6.395c.04.093.06.194.06.295v4.5A1.75 1.75 0 0 1 14.25 15H1.75A1.75 1.75 0 0 1 0 13.25v-4.5c0-.101.02-.202.06-.295Zm1.61.44a.25.25 0 0 0-.23.152L1.887 8H4.75a.75.75 0 0 1 .6.3L6.625 10h2.75l1.275-1.7a.75.75 0 0 1 .6-.3h2.863L11.82 2.652a.25.25 0 0 0-.23-.152Zm10.09 7h-2.875l-1.275 1.7a.75.75 0 0 1-.6.3h-3.5a.75.75 0 0 1-.6-.3L4.375 9.5H1.5v3.75c0 .138.112.25.25.25h12.5a.25.25 0 0 0 .25-.25Z"></path>
</svg>
</a>

    <tool-tip id="notification-indicator-tooltip" data-target="notification-indicator.tooltip" for="AppHeader-notifications-button" popover="manual" data-direction="s" data-type="label" data-view-component="true" class="sr-only position-absolute" aria-hidden="true" role="tooltip"><template shadowrootmode="open"><style>
      :host {
        --tooltip-top: var(--tool-tip-position-top, 0);
        --tooltip-left: var(--tool-tip-position-left, 0);
        padding: var(--overlay-paddingBlock-condensed) var(--overlay-padding-condensed) !important;
        font: var(--text-body-shorthand-small);
        color: var(--tooltip-fgColor, var(--fgColor-onEmphasis)) !important;
        text-align: center;
        text-decoration: none;
        text-shadow: none;
        text-transform: none;
        letter-spacing: normal;
        word-wrap: break-word;
        white-space: pre;
        background: var(--tooltip-bgColor, var(--bgColor-emphasis)) !important;
        border-radius: var(--borderRadius-medium);
        border: 0 !important;
        opacity: 0;
        max-width: var(--overlay-width-small);
        word-wrap: break-word;
        white-space: normal;
        width: max-content !important;
        inset: var(--tooltip-top) auto auto var(--tooltip-left) !important;
        overflow: visible !important;
        text-wrap: balance;
      }

      :host(:is(.tooltip-n, .tooltip-nw, .tooltip-ne)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) - var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(:is(.tooltip-s, .tooltip-sw, .tooltip-se)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) + var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(.tooltip-w) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) - var(--overlay-offset, 0.25rem));
      }

      :host(.tooltip-e) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) + var(--overlay-offset, 0.25rem));
      }

      :host:after{
        position: absolute;
        display: block;
        right: 0;
        left: 0;
        height: var(--overlay-offset, 0.25rem);
        content: "";
      }

      :host(.tooltip-s):after,
      :host(.tooltip-se):after,
      :host(.tooltip-sw):after {
        bottom: 100%
      }

      :host(.tooltip-n):after,
      :host(.tooltip-ne):after,
      :host(.tooltip-nw):after {
        top: 100%;
      }

      @keyframes tooltip-appear {
        from {
          opacity: 0;
        }
        to {
          opacity: 1;
        }
      }

      :host(:popover-open),
      :host(:popover-open):before {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      :host(.\:popover-open) {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      @media (forced-colors: active) {
        :host {
          outline: solid 1px transparent;
        }

        :host:before {
          display: none;
        }
      }
    </style><slot></slot></template>You have no unread notifications</tool-tip>
</notification-indicator>

        <div class="AppHeader-user">
          <deferred-side-panel data-url="/_side-panels/user?repository_id=974415414" data-catalyst="">
  <include-fragment data-target="deferred-side-panel.fragment" data-nonce="v1:75ea35dc-9409-f3c3-903c-f1f3c0393ed3" data-view-component="true"><template shadowrootmode="open"><style>:host {display: block;}</style><slot></slot></template>
    <react-partial-anchor data-catalyst="">
  <button data-target="react-partial-anchor.anchor" data-login="dhashvanth21" aria-label="Open user navigation menu" type="button" data-view-component="true" class="Button--invisible Button--medium Button Button--invisible-noVisuals color-bg-transparent p-0" aria-expanded="false" aria-haspopup="true">  <span class="Button-content">
    <span class="Button-label"><img src="./Conditional Statements in Python_ Even or Odd Checker_files/182338033" alt="" size="32" height="32" width="32" data-view-component="true" class="avatar circle"></span>
  </span>
</button>
  

    <script crossorigin="anonymous" defer="defer" type="application/javascript" src="./Conditional Statements in Python_ Even or Odd Checker_files/global-user-nav-drawer-29a5cd3eebf2.js.download"></script>
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/primer-react.d2117d7623cc63123645.module.css">
<link crossorigin="anonymous" media="all" rel="stylesheet" href="./Conditional Statements in Python_ Even or Odd Checker_files/global-user-nav-drawer.eeb7d39a21c5b49acbe0.module.css">

<react-partial partial-name="global-user-nav-drawer" data-ssr="false" data-attempted-ssr="false" data-catalyst="" class="loaded">
  
  <script type="application/json" data-target="react-partial.embeddedData">{"props":{"owner":{"login":"dhashvanth21","name":null,"avatarUrl":"https://avatars.githubusercontent.com/u/182338033?v=4"},"drawerId":"global-user-nav-drawer","lazyLoadItemDataFetchUrl":"/_side-panels/user.json","canAddAccount":true,"addAccountPath":"/login?add_account=1\u0026return_to=https%3A%2F%2Fgithub.com%2FKiran437228%2FModule1%2Fblob%2Fmain%2FConditional%2520Statements%2520in%2520Python%253A%2520Even%2520or%2520Odd%2520Checker.md","switchAccountPath":"/switch_account","loginAccountPath":"/login?add_account=1","projectsPath":"/dhashvanth21?tab=projects","gistsUrl":"https://gist.github.com/mine","docsUrl":"https://docs.github.com","yourEnterpriseUrl":null,"enterpriseSettingsUrl":null,"supportUrl":"https://support.github.com","showAccountSwitcher":true,"showCopilot":true,"showEnterprises":true,"showEnterprise":false,"showGists":true,"showOrganizations":true,"showSponsors":true,"showUpgrade":true,"showFeaturesPreviews":true,"showEnterpriseSettings":false,"createMenuProps":{"createRepo":true,"importRepo":true,"codespaces":true,"spark":false,"gist":true,"createOrg":true,"createProject":false,"createProjectUrl":"/dhashvanth21?tab=projects","createLegacyProject":false,"createIssue":false,"org":null,"owner":"Kiran437228","repo":"Module1"}}}</script>
  <div data-target="react-partial.reactRoot"><script type="application/json" id="__PRIMER_DATA_:r7m:__">{"resolvedServerColorMode":"night"}</script></div>
</react-partial>

  </react-partial-anchor>

</include-fragment></deferred-side-panel>
        </div>

        <div class="position-absolute mt-2">
            
<site-header-logged-in-user-menu data-catalyst="">

</site-header-logged-in-user-menu>

        </div>
      </div>
    </div>


    
        <div class="AppHeader-localBar">
          <nav data-pjax="#js-repo-pjax-container" aria-label="Repository" data-view-component="true" class="js-repo-nav js-sidenav-container-pjax js-responsive-underlinenav overflow-hidden UnderlineNav">

  <ul data-view-component="true" class="UnderlineNav-body list-style-none">
      <li data-view-component="true" class="d-inline-flex">
  <a id="code-tab" href="https://github.com/Kiran437228/Module1" data-tab-item="i0code-tab" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches repo_packages repo_deployments repo_attestations /Kiran437228/Module1" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-hotkey="g c" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Code&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item selected" aria-current="page">
    
              <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-code UnderlineNav-octicon d-none d-sm-inline">
    <path d="m11.28 3.22 4.25 4.25a.75.75 0 0 1 0 1.06l-4.25 4.25a.749.749 0 0 1-1.275-.326.749.749 0 0 1 .215-.734L13.94 8l-3.72-3.72a.749.749 0 0 1 .326-1.275.749.749 0 0 1 .734.215Zm-6.56 0a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042L2.06 8l3.72 3.72a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215L.47 8.53a.75.75 0 0 1 0-1.06Z"></path>
</svg>
        <span data-content="Code">Code</span>
          <span id="code-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="Not available" data-view-component="true" class="Counter"></span>


    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="pull-requests-tab" href="https://github.com/Kiran437228/Module1/pulls" data-tab-item="i1pull-requests-tab" data-selected-links="repo_pulls checks /Kiran437228/Module1/pulls" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-hotkey="g p" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Pull requests&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
              <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-git-pull-request UnderlineNav-octicon d-none d-sm-inline">
    <path d="M1.5 3.25a2.25 2.25 0 1 1 3 2.122v5.256a2.251 2.251 0 1 1-1.5 0V5.372A2.25 2.25 0 0 1 1.5 3.25Zm5.677-.177L9.573.677A.25.25 0 0 1 10 .854V2.5h1A2.5 2.5 0 0 1 13.5 5v5.628a2.251 2.251 0 1 1-1.5 0V5a1 1 0 0 0-1-1h-1v1.646a.25.25 0 0 1-.427.177L7.177 3.427a.25.25 0 0 1 0-.354ZM3.75 2.5a.75.75 0 1 0 0 1.5.75.75 0 0 0 0-1.5Zm0 9.5a.75.75 0 1 0 0 1.5.75.75 0 0 0 0-1.5Zm8.25.75a.75.75 0 1 0 1.5 0 .75.75 0 0 0-1.5 0Z"></path>
</svg>
        <span data-content="Pull requests">Pull requests</span>
          <span id="pull-requests-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="0" hidden="hidden" data-view-component="true" class="Counter">0</span>


    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="actions-tab" href="https://github.com/Kiran437228/Module1/actions" data-tab-item="i2actions-tab" data-selected-links="repo_actions /Kiran437228/Module1/actions" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-hotkey="g a" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Actions&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
              <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-play UnderlineNav-octicon d-none d-sm-inline">
    <path d="M8 0a8 8 0 1 1 0 16A8 8 0 0 1 8 0ZM1.5 8a6.5 6.5 0 1 0 13 0 6.5 6.5 0 0 0-13 0Zm4.879-2.773 4.264 2.559a.25.25 0 0 1 0 .428l-4.264 2.559A.25.25 0 0 1 6 10.559V5.442a.25.25 0 0 1 .379-.215Z"></path>
</svg>
        <span data-content="Actions">Actions</span>
          <span id="actions-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="Not available" data-view-component="true" class="Counter"></span>


    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="projects-tab" href="https://github.com/Kiran437228/Module1/projects" data-tab-item="i3projects-tab" data-selected-links="repo_projects new_repo_project repo_project /Kiran437228/Module1/projects" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-hotkey="g b" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Projects&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
              <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-table UnderlineNav-octicon d-none d-sm-inline">
    <path d="M0 1.75C0 .784.784 0 1.75 0h12.5C15.216 0 16 .784 16 1.75v12.5A1.75 1.75 0 0 1 14.25 16H1.75A1.75 1.75 0 0 1 0 14.25ZM6.5 6.5v8h7.75a.25.25 0 0 0 .25-.25V6.5Zm8-1.5V1.75a.25.25 0 0 0-.25-.25H6.5V5Zm-13 1.5v7.75c0 .138.112.25.25.25H5v-8ZM5 5V1.5H1.75a.25.25 0 0 0-.25.25V5Z"></path>
</svg>
        <span data-content="Projects">Projects</span>
          <span id="projects-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="0" hidden="hidden" data-view-component="true" class="Counter">0</span>


    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="security-tab" href="https://github.com/Kiran437228/Module1/security" data-tab-item="i4security-tab" data-selected-links="security overview alerts policy token_scanning code_scanning /Kiran437228/Module1/security" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-hotkey="g s" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Security&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
              <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-shield UnderlineNav-octicon d-none d-sm-inline">
    <path d="M7.467.133a1.748 1.748 0 0 1 1.066 0l5.25 1.68A1.75 1.75 0 0 1 15 3.48V7c0 1.566-.32 3.182-1.303 4.682-.983 1.498-2.585 2.813-5.032 3.855a1.697 1.697 0 0 1-1.33 0c-2.447-1.042-4.049-2.357-5.032-3.855C1.32 10.182 1 8.566 1 7V3.48a1.75 1.75 0 0 1 1.217-1.667Zm.61 1.429a.25.25 0 0 0-.153 0l-5.25 1.68a.25.25 0 0 0-.174.238V7c0 1.358.275 2.666 1.057 3.86.784 1.194 2.121 2.34 4.366 3.297a.196.196 0 0 0 .154 0c2.245-.956 3.582-2.104 4.366-3.298C13.225 9.666 13.5 8.36 13.5 7V3.48a.251.251 0 0 0-.174-.237l-5.25-1.68ZM8.75 4.75v3a.75.75 0 0 1-1.5 0v-3a.75.75 0 0 1 1.5 0ZM9 10.5a1 1 0 1 1-2 0 1 1 0 0 1 2 0Z"></path>
</svg>
        <span data-content="Security">Security</span>
          

    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="insights-tab" href="https://github.com/Kiran437228/Module1/pulse" data-tab-item="i5insights-tab" data-selected-links="repo_graphs repo_contributors dependency_graph dependabot_updates pulse people community /Kiran437228/Module1/pulse" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Insights&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
              <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-graph UnderlineNav-octicon d-none d-sm-inline">
    <path d="M1.5 1.75V13.5h13.75a.75.75 0 0 1 0 1.5H.75a.75.75 0 0 1-.75-.75V1.75a.75.75 0 0 1 1.5 0Zm14.28 2.53-5.25 5.25a.75.75 0 0 1-1.06 0L7 7.06 4.28 9.78a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042l3.25-3.25a.75.75 0 0 1 1.06 0L10 7.94l4.72-4.72a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042Z"></path>
</svg>
        <span data-content="Insights">Insights</span>
          <span id="insights-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="Not available" data-view-component="true" class="Counter"></span>


    
</a></li>
</ul>
    <div style="visibility:hidden;" data-view-component="true" class="UnderlineNav-actions js-responsive-underlinenav-overflow position-absolute pr-3 pr-md-4 pr-lg-5 right-0">      <action-menu data-select-variant="none" data-view-component="true" data-catalyst="" data-ready="true">
  <focus-group direction="vertical" mnemonics="" retain="">
    <button id="action-menu-28515277-00a4-43a4-9f1b-2477365d3605-button" popovertarget="action-menu-28515277-00a4-43a4-9f1b-2477365d3605-overlay" aria-controls="action-menu-28515277-00a4-43a4-9f1b-2477365d3605-list" aria-haspopup="true" aria-labelledby="tooltip-e9fe8a86-8701-4260-8abe-0761ee35b956" type="button" data-view-component="true" class="Button Button--iconOnly Button--secondary Button--medium UnderlineNav-item">  <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-kebab-horizontal Button-visual">
    <path d="M8 9a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3ZM1.5 9a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Zm13 0a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Z"></path>
</svg>
</button><tool-tip id="tooltip-e9fe8a86-8701-4260-8abe-0761ee35b956" for="action-menu-28515277-00a4-43a4-9f1b-2477365d3605-button" popover="manual" data-direction="s" data-type="label" data-view-component="true" class="sr-only position-absolute" aria-hidden="true" role="tooltip"><template shadowrootmode="open"><style>
      :host {
        --tooltip-top: var(--tool-tip-position-top, 0);
        --tooltip-left: var(--tool-tip-position-left, 0);
        padding: var(--overlay-paddingBlock-condensed) var(--overlay-padding-condensed) !important;
        font: var(--text-body-shorthand-small);
        color: var(--tooltip-fgColor, var(--fgColor-onEmphasis)) !important;
        text-align: center;
        text-decoration: none;
        text-shadow: none;
        text-transform: none;
        letter-spacing: normal;
        word-wrap: break-word;
        white-space: pre;
        background: var(--tooltip-bgColor, var(--bgColor-emphasis)) !important;
        border-radius: var(--borderRadius-medium);
        border: 0 !important;
        opacity: 0;
        max-width: var(--overlay-width-small);
        word-wrap: break-word;
        white-space: normal;
        width: max-content !important;
        inset: var(--tooltip-top) auto auto var(--tooltip-left) !important;
        overflow: visible !important;
        text-wrap: balance;
      }

      :host(:is(.tooltip-n, .tooltip-nw, .tooltip-ne)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) - var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(:is(.tooltip-s, .tooltip-sw, .tooltip-se)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) + var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(.tooltip-w) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) - var(--overlay-offset, 0.25rem));
      }

      :host(.tooltip-e) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) + var(--overlay-offset, 0.25rem));
      }

      :host:after{
        position: absolute;
        display: block;
        right: 0;
        left: 0;
        height: var(--overlay-offset, 0.25rem);
        content: "";
      }

      :host(.tooltip-s):after,
      :host(.tooltip-se):after,
      :host(.tooltip-sw):after {
        bottom: 100%
      }

      :host(.tooltip-n):after,
      :host(.tooltip-ne):after,
      :host(.tooltip-nw):after {
        top: 100%;
      }

      @keyframes tooltip-appear {
        from {
          opacity: 0;
        }
        to {
          opacity: 1;
        }
      }

      :host(:popover-open),
      :host(:popover-open):before {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      :host(.\:popover-open) {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      @media (forced-colors: active) {
        :host {
          outline: solid 1px transparent;
        }

        :host:before {
          display: none;
        }
      }
    </style><slot></slot></template>Additional navigation options</tool-tip>


<anchored-position data-target="action-menu.overlay" id="action-menu-28515277-00a4-43a4-9f1b-2477365d3605-overlay" anchor="action-menu-28515277-00a4-43a4-9f1b-2477365d3605-button" align="start" side="outside-bottom" anchor-offset="normal" popover="auto" data-view-component="true" style="inset: 36px auto auto 0px;">
  <div data-view-component="true" class="Overlay Overlay--size-auto">
    
      <div data-view-component="true" class="Overlay-body Overlay-body--paddingNone">          <action-list data-catalyst="">
  <div data-view-component="true">
    <ul aria-labelledby="action-menu-28515277-00a4-43a4-9f1b-2477365d3605-button" id="action-menu-28515277-00a4-43a4-9f1b-2477365d3605-list" role="menu" data-view-component="true" class="ActionListWrap--inset ActionListWrap">
        <li hidden="" data-menu-item="i0code-tab" data-targets="action-list.items" role="none" data-view-component="true" class="ActionListItem">
    
    
    <a tabindex="-1" id="item-9a353ef9-a85a-427f-9092-883edd857f7a" href="https://github.com/Kiran437228/Module1" role="menuitem" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-code">
    <path d="m11.28 3.22 4.25 4.25a.75.75 0 0 1 0 1.06l-4.25 4.25a.749.749 0 0 1-1.275-.326.749.749 0 0 1 .215-.734L13.94 8l-3.72-3.72a.749.749 0 0 1 .326-1.275.749.749 0 0 1 .734.215Zm-6.56 0a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042L2.06 8l3.72 3.72a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215L.47 8.53a.75.75 0 0 1 0-1.06Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Code
</span>      
</a>
  
</li>
        <li hidden="" data-menu-item="i1pull-requests-tab" data-targets="action-list.items" role="none" data-view-component="true" class="ActionListItem">
    
    
    <a tabindex="-1" id="item-1dab7a31-676d-4977-8768-1a4e186fe936" href="https://github.com/Kiran437228/Module1/pulls" role="menuitem" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-git-pull-request">
    <path d="M1.5 3.25a2.25 2.25 0 1 1 3 2.122v5.256a2.251 2.251 0 1 1-1.5 0V5.372A2.25 2.25 0 0 1 1.5 3.25Zm5.677-.177L9.573.677A.25.25 0 0 1 10 .854V2.5h1A2.5 2.5 0 0 1 13.5 5v5.628a2.251 2.251 0 1 1-1.5 0V5a1 1 0 0 0-1-1h-1v1.646a.25.25 0 0 1-.427.177L7.177 3.427a.25.25 0 0 1 0-.354ZM3.75 2.5a.75.75 0 1 0 0 1.5.75.75 0 0 0 0-1.5Zm0 9.5a.75.75 0 1 0 0 1.5.75.75 0 0 0 0-1.5Zm8.25.75a.75.75 0 1 0 1.5 0 .75.75 0 0 0-1.5 0Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Pull requests
</span>      
</a>
  
</li>
        <li hidden="" data-menu-item="i2actions-tab" data-targets="action-list.items" role="none" data-view-component="true" class="ActionListItem">
    
    
    <a tabindex="-1" id="item-743bfb5f-aad5-4549-bc24-c0f6666d8308" href="https://github.com/Kiran437228/Module1/actions" role="menuitem" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-play">
    <path d="M8 0a8 8 0 1 1 0 16A8 8 0 0 1 8 0ZM1.5 8a6.5 6.5 0 1 0 13 0 6.5 6.5 0 0 0-13 0Zm4.879-2.773 4.264 2.559a.25.25 0 0 1 0 .428l-4.264 2.559A.25.25 0 0 1 6 10.559V5.442a.25.25 0 0 1 .379-.215Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Actions
</span>      
</a>
  
</li>
        <li hidden="" data-menu-item="i3projects-tab" data-targets="action-list.items" role="none" data-view-component="true" class="ActionListItem">
    
    
    <a tabindex="-1" id="item-2731f6cc-e8f1-4650-b35c-3d78c3f40a3e" href="https://github.com/Kiran437228/Module1/projects" role="menuitem" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-table">
    <path d="M0 1.75C0 .784.784 0 1.75 0h12.5C15.216 0 16 .784 16 1.75v12.5A1.75 1.75 0 0 1 14.25 16H1.75A1.75 1.75 0 0 1 0 14.25ZM6.5 6.5v8h7.75a.25.25 0 0 0 .25-.25V6.5Zm8-1.5V1.75a.25.25 0 0 0-.25-.25H6.5V5Zm-13 1.5v7.75c0 .138.112.25.25.25H5v-8ZM5 5V1.5H1.75a.25.25 0 0 0-.25.25V5Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Projects
</span>      
</a>
  
</li>
        <li hidden="" data-menu-item="i4security-tab" data-targets="action-list.items" role="none" data-view-component="true" class="ActionListItem">
    
    
    <a tabindex="-1" id="item-6454c35c-13a7-4273-ab63-10ab23b6992b" href="https://github.com/Kiran437228/Module1/security" role="menuitem" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-shield">
    <path d="M7.467.133a1.748 1.748 0 0 1 1.066 0l5.25 1.68A1.75 1.75 0 0 1 15 3.48V7c0 1.566-.32 3.182-1.303 4.682-.983 1.498-2.585 2.813-5.032 3.855a1.697 1.697 0 0 1-1.33 0c-2.447-1.042-4.049-2.357-5.032-3.855C1.32 10.182 1 8.566 1 7V3.48a1.75 1.75 0 0 1 1.217-1.667Zm.61 1.429a.25.25 0 0 0-.153 0l-5.25 1.68a.25.25 0 0 0-.174.238V7c0 1.358.275 2.666 1.057 3.86.784 1.194 2.121 2.34 4.366 3.297a.196.196 0 0 0 .154 0c2.245-.956 3.582-2.104 4.366-3.298C13.225 9.666 13.5 8.36 13.5 7V3.48a.251.251 0 0 0-.174-.237l-5.25-1.68ZM8.75 4.75v3a.75.75 0 0 1-1.5 0v-3a.75.75 0 0 1 1.5 0ZM9 10.5a1 1 0 1 1-2 0 1 1 0 0 1 2 0Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Security
</span>      
</a>
  
</li>
        <li hidden="" data-menu-item="i5insights-tab" data-targets="action-list.items" role="none" data-view-component="true" class="ActionListItem">
    
    
    <a tabindex="-1" id="item-daac2d8d-5434-4ac3-b6f0-35d3b05ecad8" href="https://github.com/Kiran437228/Module1/pulse" role="menuitem" data-view-component="true" class="ActionListContent ActionListContent--visual16">
        <span class="ActionListItem-visual ActionListItem-visual--leading">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-graph">
    <path d="M1.5 1.75V13.5h13.75a.75.75 0 0 1 0 1.5H.75a.75.75 0 0 1-.75-.75V1.75a.75.75 0 0 1 1.5 0Zm14.28 2.53-5.25 5.25a.75.75 0 0 1-1.06 0L7 7.06 4.28 9.78a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042l3.25-3.25a.75.75 0 0 1 1.06 0L10 7.94l4.72-4.72a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042Z"></path>
</svg>
        </span>
      
        <span data-view-component="true" class="ActionListItem-label">
          Insights
</span>      
</a>
  
</li>
</ul>    
</div></action-list>


</div>
      
</div></anchored-position>  </focus-group>
</action-menu></div>
</nav>
          
        </div>
</header>


      <div hidden="hidden" data-view-component="true" class="js-stale-session-flash stale-session-flash flash flash-warn flash-full">
  
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert">
    <path d="M6.457 1.047c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0 1 14.082 15H1.918a1.75 1.75 0 0 1-1.543-2.575Zm1.763.707a.25.25 0 0 0-.44 0L1.698 13.132a.25.25 0 0 0 .22.368h12.164a.25.25 0 0 0 .22-.368Zm.53 3.996v2.5a.75.75 0 0 1-1.5 0v-2.5a.75.75 0 0 1 1.5 0ZM9 11a1 1 0 1 1-2 0 1 1 0 0 1 2 0Z"></path>
</svg>
        <span class="js-stale-session-flash-signed-in" hidden="">You signed in with another tab or window. <a class="Link--inTextBlock" href="https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md">Reload</a> to refresh your session.</span>
        <span class="js-stale-session-flash-signed-out" hidden="">You signed out in another tab or window. <a class="Link--inTextBlock" href="https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md">Reload</a> to refresh your session.</span>
        <span class="js-stale-session-flash-switched" hidden="">You switched accounts on another tab or window. <a class="Link--inTextBlock" href="https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md">Reload</a> to refresh your session.</span>

    <button id="icon-button-fff5d92c-5ad6-40dc-8a03-0f55eacbe736" aria-labelledby="tooltip-78e2bf3e-171a-4319-945a-80a62cd10fcf" type="button" data-view-component="true" class="Button Button--iconOnly Button--invisible Button--medium flash-close js-flash-close">  <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x Button-visual">
    <path d="M3.72 3.72a.75.75 0 0 1 1.06 0L8 6.94l3.22-3.22a.749.749 0 0 1 1.275.326.749.749 0 0 1-.215.734L9.06 8l3.22 3.22a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215L8 9.06l-3.22 3.22a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042L6.94 8 3.72 4.78a.75.75 0 0 1 0-1.06Z"></path>
</svg>
</button><tool-tip id="tooltip-78e2bf3e-171a-4319-945a-80a62cd10fcf" for="icon-button-fff5d92c-5ad6-40dc-8a03-0f55eacbe736" popover="manual" data-direction="s" data-type="label" data-view-component="true" class="sr-only position-absolute" aria-hidden="true" role="tooltip"><template shadowrootmode="open"><style>
      :host {
        --tooltip-top: var(--tool-tip-position-top, 0);
        --tooltip-left: var(--tool-tip-position-left, 0);
        padding: var(--overlay-paddingBlock-condensed) var(--overlay-padding-condensed) !important;
        font: var(--text-body-shorthand-small);
        color: var(--tooltip-fgColor, var(--fgColor-onEmphasis)) !important;
        text-align: center;
        text-decoration: none;
        text-shadow: none;
        text-transform: none;
        letter-spacing: normal;
        word-wrap: break-word;
        white-space: pre;
        background: var(--tooltip-bgColor, var(--bgColor-emphasis)) !important;
        border-radius: var(--borderRadius-medium);
        border: 0 !important;
        opacity: 0;
        max-width: var(--overlay-width-small);
        word-wrap: break-word;
        white-space: normal;
        width: max-content !important;
        inset: var(--tooltip-top) auto auto var(--tooltip-left) !important;
        overflow: visible !important;
        text-wrap: balance;
      }

      :host(:is(.tooltip-n, .tooltip-nw, .tooltip-ne)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) - var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(:is(.tooltip-s, .tooltip-sw, .tooltip-se)) {
        --tooltip-top: calc(var(--tool-tip-position-top, 0) + var(--overlay-offset, 0.25rem));
        --tooltip-left: var(--tool-tip-position-left);
      }

      :host(.tooltip-w) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) - var(--overlay-offset, 0.25rem));
      }

      :host(.tooltip-e) {
        --tooltip-top: var(--tool-tip-position-top);
        --tooltip-left: calc(var(--tool-tip-position-left, 0) + var(--overlay-offset, 0.25rem));
      }

      :host:after{
        position: absolute;
        display: block;
        right: 0;
        left: 0;
        height: var(--overlay-offset, 0.25rem);
        content: "";
      }

      :host(.tooltip-s):after,
      :host(.tooltip-se):after,
      :host(.tooltip-sw):after {
        bottom: 100%
      }

      :host(.tooltip-n):after,
      :host(.tooltip-ne):after,
      :host(.tooltip-nw):after {
        top: 100%;
      }

      @keyframes tooltip-appear {
        from {
          opacity: 0;
        }
        to {
          opacity: 1;
        }
      }

      :host(:popover-open),
      :host(:popover-open):before {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      :host(.\:popover-open) {
        animation-name: tooltip-appear;
        animation-duration: .1s;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in;
      }

      @media (forced-colors: active) {
        :host {
          outline: solid 1px transparent;
        }

        :host:before {
          display: none;
        }
      }
    </style><slot></slot></template>Dismiss alert</tool-tip>


  
</div>
          
    </div>

  <div id="start-of-content" class="show-on-focus"></div>








    <div id="js-flash-container" class="flash-container" data-turbo-replace="">




  <template class="js-flash-template"></template>
</div>


    
  <notification-shelf-watcher data-base-url="https://github.com/notifications/beta/shelf" data-channel="eyJjIjoibm90aWZpY2F0aW9uLWNoYW5nZWQ6MTgyMzM4MDMzIiwidCI6MTc0NzI0OTI2NX0=--2445a9b5203abc7c23e3192db827c194184a371a572692610fd0ba0eb9727b2a" data-view-component="true" class="js-socket-channel" data-refresh-delay="500" data-catalyst="" data-throttle-delay="5000"></notification-shelf-watcher>
  <div hidden="" data-initial="" data-target="notification-shelf-watcher.placeholder"></div>






  <div class="application-main " data-commit-hovercards-enabled="" data-discussion-hovercards-enabled="" data-issue-and-pr-hovercards-enabled="" data-project-hovercards-enabled="">
        <div itemscope="" itemtype="http://schema.org/SoftwareSourceCode" class="">
    <main id="js-repo-pjax-container">
      
      






    
  <div id="repository-container-header" data-turbo-replace="" hidden=""></div>




<turbo-frame id="repo-content-turbo-frame" target="_top" data-turbo-action="advance" class="">
    <div id="repo-content-pjax-container" class="repository-content ">
      <a href="https://github.dev/" class="d-none js-github-dev-shortcut" data-hotkey=".,Mod+Alt+.">Open in github.dev</a>
  <a href="https://github.dev/" class="d-none js-github-dev-new-tab-shortcut" data-hotkey="Shift+.,Shift+&gt;,&gt;" target="_blank" rel="noopener noreferrer">Open in a new github.dev tab</a>
    <a class="d-none" data-hotkey=",,Mod+Alt+," target="_blank" href="https://github.com/codespaces/new/Kiran437228/Module1/tree/main?resume=1">Open in codespace</a>




    
      
    








<react-app app-name="react-code-view" initial-path="/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md" style="display: block; min-height: calc(100vh - 64px);" data-attempted-ssr="true" data-ssr="true" data-lazy="false" data-alternate="false" data-data-router-enabled="false" data-catalyst="" class="loaded">
  
  <script type="application/json" data-target="react-app.embeddedData">{"payload":{"allShortcutsEnabled":true,"fileTree":{"":{"items":[{"name":"Conditional Statements in Python: Even or Odd Checker.md","path":"Conditional Statements in Python: Even or Odd Checker.md","contentType":"file"},{"name":"Datatypes-Boolean Expression Evaluation.md","path":"Datatypes-Boolean Expression Evaluation.md","contentType":"file"},{"name":"Datatypes-Character Literals.md","path":"Datatypes-Character Literals.md","contentType":"file"},{"name":"Datatypes-Complex Number.md","path":"Datatypes-Complex Number.md","contentType":"file"},{"name":"Datatypes-String Literals.md","path":"Datatypes-String Literals.md","contentType":"file"}],"totalCount":5}},"fileTreeProcessingTime":2.6728009999999998,"foldersToFetch":[],"incompleteFileTree":false,"repo":{"id":974415414,"defaultBranch":"main","name":"Module1","ownerLogin":"Kiran437228","currentUserCanPush":false,"isFork":true,"isEmpty":false,"createdAt":"2025-04-29T00:06:43.000+05:30","ownerAvatar":"https://avatars.githubusercontent.com/u/182343513?v=4","public":true,"private":false,"isOrgOwned":false},"codeLineWrapEnabled":false,"symbolsExpanded":false,"treeExpanded":true,"refInfo":{"name":"main","listCacheKey":"v0:1745865404.772355","canEdit":true,"refType":"branch","currentOid":"cd56a190f392faafdd7928aa78289c2d76b2abb8"},"path":"Conditional Statements in Python: Even or Odd Checker.md","currentUser":{"id":182338033,"login":"dhashvanth21","userEmail":"dhashapro@gmail.com"},"blob":{"rawLines":null,"stylingDirectives":null,"colorizedLines":null,"csv":null,"csvError":null,"dependabotInfo":{"showConfigurationBanner":false,"configFilePath":null,"networkDependabotPath":"/Kiran437228/Module1/network/updates","dismissConfigurationNoticePath":"/settings/dismiss-notice/dependabot_configuration_notice","configurationNoticeDismissed":false},"displayName":"Conditional Statements in Python: Even or Odd Checker.md","displayUrl":"https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python:%20Even%20or%20Odd%20Checker.md?raw=true","headerInfo":{"blobSize":"690 Bytes","deleteTooltip":"Delete the file in your fork of this project","editTooltip":"Edit the file in your fork of this project","ghDesktopPath":"https://desktop.github.com","isGitLfs":false,"onBranch":true,"shortPath":"041d0d3","siteNavLoginPath":"/login?return_to=https%3A%2F%2Fgithub.com%2FKiran437228%2FModule1%2Fblob%2Fmain%2FConditional%2520Statements%2520in%2520Python%253A%2520Even%2520or%2520Odd%2520Checker.md","isCSV":false,"isRichtext":true,"toc":[{"level":1,"text":"Conditional Statements in Python: Even or Odd Checker","anchor":"conditional-statements-in-python-even-or-odd-checker","htmlText":"Conditional Statements in Python: Even or Odd Checker"},{"level":2,"text":"🎯 Aim","anchor":"-aim","htmlText":"🎯 Aim"},{"level":2,"text":"🧠 Algorithm","anchor":"-algorithm","htmlText":"🧠 Algorithm"},{"level":2,"text":"🧾 Program","anchor":"-program","htmlText":"🧾 Program"},{"level":2,"text":"Output","anchor":"output","htmlText":"Output"},{"level":2,"text":"Result","anchor":"result","htmlText":"Result"}],"lineInfo":{"truncatedLoc":"27","truncatedSloc":"22"},"mode":"file"},"image":false,"isCodeownersFile":null,"isPlain":false,"isValidLegacyIssueTemplate":false,"issueTemplate":null,"discussionTemplate":null,"language":"Markdown","languageID":222,"large":false,"planSupportInfo":{"repoIsFork":null,"repoOwnedByCurrentUser":null,"requestFullPath":"/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md","showFreeOrgGatedFeatureMessage":null,"showPlanSupportBanner":null,"upgradeDataAttributes":null,"upgradePath":null},"publishBannersInfo":{"dismissActionNoticePath":"/settings/dismiss-notice/publish_action_from_dockerfile","releasePath":"/Kiran437228/Module1/releases/new?marketplace=true","showPublishActionBanner":false},"rawBlobUrl":"https://github.com/Kiran437228/Module1/raw/refs/heads/main/Conditional%20Statements%20in%20Python:%20Even%20or%20Odd%20Checker.md","renderImageOrRaw":false,"richText":"\u003carticle class=\"markdown-body entry-content container-lg\" itemprop=\"text\"\u003e\u003cdiv class=\"markdown-heading\" dir=\"auto\"\u003e\u003ch1 tabindex=\"-1\" class=\"heading-element\" dir=\"auto\"\u003eConditional Statements in Python: Even or Odd Checker\u003c/h1\u003e\u003ca id=\"user-content-conditional-statements-in-python-even-or-odd-checker\" class=\"anchor\" aria-label=\"Permalink: Conditional Statements in Python: Even or Odd Checker\" href=\"#conditional-statements-in-python-even-or-odd-checker\"\u003e\u003csvg class=\"octicon octicon-link\" viewBox=\"0 0 16 16\" version=\"1.1\" width=\"16\" height=\"16\" aria-hidden=\"true\"\u003e\u003cpath d=\"m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z\"\u003e\u003c/path\u003e\u003c/svg\u003e\u003c/a\u003e\u003c/div\u003e\n\u003cdiv class=\"markdown-heading\" dir=\"auto\"\u003e\u003ch2 tabindex=\"-1\" class=\"heading-element\" dir=\"auto\"\u003e🎯 Aim\u003c/h2\u003e\u003ca id=\"user-content--aim\" class=\"anchor\" aria-label=\"Permalink: 🎯 Aim\" href=\"#-aim\"\u003e\u003csvg class=\"octicon octicon-link\" viewBox=\"0 0 16 16\" version=\"1.1\" width=\"16\" height=\"16\" aria-hidden=\"true\"\u003e\u003cpath d=\"m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z\"\u003e\u003c/path\u003e\u003c/svg\u003e\u003c/a\u003e\u003c/div\u003e\n\u003cp dir=\"auto\"\u003eTo write a Python program to check whether the given number is \u003cstrong\u003eeven\u003c/strong\u003e or \u003cstrong\u003eodd\u003c/strong\u003e using \u003ccode\u003eif...else\u003c/code\u003e statements.\u003c/p\u003e\n\u003cdiv class=\"markdown-heading\" dir=\"auto\"\u003e\u003ch2 tabindex=\"-1\" class=\"heading-element\" dir=\"auto\"\u003e🧠 Algorithm\u003c/h2\u003e\u003ca id=\"user-content--algorithm\" class=\"anchor\" aria-label=\"Permalink: 🧠 Algorithm\" href=\"#-algorithm\"\u003e\u003csvg class=\"octicon octicon-link\" viewBox=\"0 0 16 16\" version=\"1.1\" width=\"16\" height=\"16\" aria-hidden=\"true\"\u003e\u003cpath d=\"m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z\"\u003e\u003c/path\u003e\u003c/svg\u003e\u003c/a\u003e\u003c/div\u003e\n\u003col dir=\"auto\"\u003e\n\u003cli\u003eGet an input from the user.\u003c/li\u003e\n\u003cli\u003eConvert the input to an integer and store it in a variable \u003ccode\u003ea\u003c/code\u003e.\u003c/li\u003e\n\u003cli\u003eUse the modulo operator \u003ccode\u003e%\u003c/code\u003e to check if \u003ccode\u003ea % 2 == 0\u003c/code\u003e.\n\u003cul dir=\"auto\"\u003e\n\u003cli\u003eIf true, print \u003ccode\u003e\"EVEN\"\u003c/code\u003e.\u003c/li\u003e\n\u003cli\u003eElse, print \u003ccode\u003e\"ODD\"\u003c/code\u003e.\u003c/li\u003e\n\u003c/ul\u003e\n\u003c/li\u003e\n\u003cli\u003eEnd the program.\u003c/li\u003e\n\u003c/ol\u003e\n\u003cdiv class=\"markdown-heading\" dir=\"auto\"\u003e\u003ch2 tabindex=\"-1\" class=\"heading-element\" dir=\"auto\"\u003e🧾 Program\u003c/h2\u003e\u003ca id=\"user-content--program\" class=\"anchor\" aria-label=\"Permalink: 🧾 Program\" href=\"#-program\"\u003e\u003csvg class=\"octicon octicon-link\" viewBox=\"0 0 16 16\" version=\"1.1\" width=\"16\" height=\"16\" aria-hidden=\"true\"\u003e\u003cpath d=\"m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z\"\u003e\u003c/path\u003e\u003c/svg\u003e\u003c/a\u003e\u003c/div\u003e\n\u003cdiv class=\"snippet-clipboard-content notranslate position-relative overflow-auto\" data-snippet-clipboard-copy-content=\"a=int(input())\n\nif(a%2==0):\n     print(\u0026quot;EVEN\u0026quot;)\nelse:\n     print(\u0026quot;ODD\u0026quot;)\"\u003e\u003cpre class=\"notranslate\"\u003e\u003ccode\u003ea=int(input())\n\nif(a%2==0):\n     print(\"EVEN\")\nelse:\n     print(\"ODD\")\n\u003c/code\u003e\u003c/pre\u003e\u003c/div\u003e\n\u003cdiv class=\"markdown-heading\" dir=\"auto\"\u003e\u003ch2 tabindex=\"-1\" class=\"heading-element\" dir=\"auto\"\u003eOutput\u003c/h2\u003e\u003ca id=\"user-content-output\" class=\"anchor\" aria-label=\"Permalink: Output\" href=\"#output\"\u003e\u003csvg class=\"octicon octicon-link\" viewBox=\"0 0 16 16\" version=\"1.1\" width=\"16\" height=\"16\" aria-hidden=\"true\"\u003e\u003cpath d=\"m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z\"\u003e\u003c/path\u003e\u003c/svg\u003e\u003c/a\u003e\u003c/div\u003e\n\u003cp dir=\"auto\"\u003e\u003ca target=\"_blank\" rel=\"noopener noreferrer\" href=\"https://private-user-images.githubusercontent.com/206125527/438184680-e0509053-337e-4109-8509-440cd95de43c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDcyNDk1NjQsIm5iZiI6MTc0NzI0OTI2NCwicGF0aCI6Ii8yMDYxMjU1MjcvNDM4MTg0NjgwLWUwNTA5MDUzLTMzN2UtNDEwOS04NTA5LTQ0MGNkOTVkZTQzYy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNTE0JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDUxNFQxOTAxMDRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT00ZjYyNzE3MDdiZjAzZTdlYjJkODJjYTY5M2VlZTg4OTQ2MjVlNmM0ZWFlYmE4NTgzOTQ1MTdlNTYwNjBiYzNiJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.1ftc4a1-ricTnLN22E1yCTr0OHmi1nCt40UC-_kynHE\"\u003e\u003cimg src=\"https://private-user-images.githubusercontent.com/206125527/438184680-e0509053-337e-4109-8509-440cd95de43c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDcyNDk1NjQsIm5iZiI6MTc0NzI0OTI2NCwicGF0aCI6Ii8yMDYxMjU1MjcvNDM4MTg0NjgwLWUwNTA5MDUzLTMzN2UtNDEwOS04NTA5LTQ0MGNkOTVkZTQzYy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNTE0JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDUxNFQxOTAxMDRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT00ZjYyNzE3MDdiZjAzZTdlYjJkODJjYTY5M2VlZTg4OTQ2MjVlNmM0ZWFlYmE4NTgzOTQ1MTdlNTYwNjBiYzNiJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.1ftc4a1-ricTnLN22E1yCTr0OHmi1nCt40UC-_kynHE\" alt=\"image\" style=\"max-width: 100%;\"\u003e\u003c/a\u003e\u003c/p\u003e\n\u003cdiv class=\"markdown-heading\" dir=\"auto\"\u003e\u003ch2 tabindex=\"-1\" class=\"heading-element\" dir=\"auto\"\u003eResult\u003c/h2\u003e\u003ca id=\"user-content-result\" class=\"anchor\" aria-label=\"Permalink: Result\" href=\"#result\"\u003e\u003csvg class=\"octicon octicon-link\" viewBox=\"0 0 16 16\" version=\"1.1\" width=\"16\" height=\"16\" aria-hidden=\"true\"\u003e\u003cpath d=\"m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z\"\u003e\u003c/path\u003e\u003c/svg\u003e\u003c/a\u003e\u003c/div\u003e\n\u003cp dir=\"auto\"\u003eThus, the python program was executed successfully\u003c/p\u003e\n\u003c/article\u003e","renderedFileInfo":null,"shortPath":null,"symbolsEnabled":true,"tabSize":8,"topBannersInfo":{"overridingGlobalFundingFile":false,"globalPreferredFundingPath":null,"showInvalidCitationWarning":false,"citationHelpUrl":"https://docs.github.com/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/about-citation-files","actionsOnboardingTip":null},"truncated":false,"viewable":true,"workflowRedirectUrl":null,"symbols":{"timed_out":false,"not_analyzed":false,"symbols":[{"name":"Conditional Statements in Python: Even or Odd Checker","kind":"section_1","ident_start":2,"ident_end":55,"extent_start":0,"extent_end":690,"fully_qualified_name":"Conditional Statements in Python: Even or Odd Checker","ident_utf16":{"start":{"line_number":0,"utf16_col":2},"end":{"line_number":0,"utf16_col":55}},"extent_utf16":{"start":{"line_number":0,"utf16_col":0},"end":{"line_number":27,"utf16_col":0}}},{"name":"🎯 Aim","kind":"section_2","ident_start":60,"ident_end":68,"extent_start":57,"extent_end":183,"fully_qualified_name":"🎯 Aim","ident_utf16":{"start":{"line_number":2,"utf16_col":3},"end":{"line_number":2,"utf16_col":9}},"extent_utf16":{"start":{"line_number":2,"utf16_col":0},"end":{"line_number":5,"utf16_col":0}}},{"name":"🧠 Algorithm","kind":"section_2","ident_start":186,"ident_end":200,"extent_start":183,"extent_end":433,"fully_qualified_name":"🧠 Algorithm","ident_utf16":{"start":{"line_number":5,"utf16_col":3},"end":{"line_number":5,"utf16_col":15}},"extent_utf16":{"start":{"line_number":5,"utf16_col":0},"end":{"line_number":13,"utf16_col":0}}},{"name":"🧾 Program","kind":"section_2","ident_start":436,"ident_end":448,"extent_start":433,"extent_end":528,"fully_qualified_name":"🧾 Program","ident_utf16":{"start":{"line_number":13,"utf16_col":3},"end":{"line_number":13,"utf16_col":13}},"extent_utf16":{"start":{"line_number":13,"utf16_col":0},"end":{"line_number":22,"utf16_col":0}}},{"name":"Output","kind":"section_2","ident_start":531,"ident_end":537,"extent_start":528,"extent_end":629,"fully_qualified_name":"Output","ident_utf16":{"start":{"line_number":22,"utf16_col":3},"end":{"line_number":22,"utf16_col":9}},"extent_utf16":{"start":{"line_number":22,"utf16_col":0},"end":{"line_number":25,"utf16_col":0}}},{"name":"Result","kind":"section_2","ident_start":632,"ident_end":638,"extent_start":629,"extent_end":690,"fully_qualified_name":"Result","ident_utf16":{"start":{"line_number":25,"utf16_col":3},"end":{"line_number":25,"utf16_col":9}},"extent_utf16":{"start":{"line_number":25,"utf16_col":0},"end":{"line_number":27,"utf16_col":0}}}]}},"copilotInfo":{"documentationUrl":"https://docs.github.com/copilot/overview-of-github-copilot/about-github-copilot-for-individuals","notices":{"codeViewPopover":{"dismissed":false,"dismissPath":"/settings/dismiss-notice/code_view_copilot_popover"}},"userAccess":{"hasSubscriptionEnded":false,"orgHasCFBAccess":false,"userHasCFIAccess":false,"userHasOrgs":false,"userIsOrgAdmin":false,"userIsOrgMember":false,"business":null,"featureRequestInfo":null}},"copilotAccessAllowed":false,"modelsAccessAllowed":false,"modelsRepoIntegrationEnabled":false,"csrf_tokens":{"/Kiran437228/Module1/branches":{"post":"MngNQ6W4smqaXyNv9B99zecV-vrHkUwgd1znN_ydiUBUf5RLzAfxMY9rhNwrPGQEqkq-SXEzpqqSfdN--W9lUg"},"/repos/preferences":{"post":"aIzitDBcPEpary8A2nbIirNmDg4xwCR4-ON2wL3xqvFDvWbI8DWYJyGC5wZ-SHgQCgiVuMnRo6ZEfrKcUeV0vw"}}},"title":"Module1/Conditional Statements in Python: Even or Odd Checker.md at main · Kiran437228/Module1","appPayload":{"helpUrl":"https://docs.github.com","findFileWorkerPath":"/assets-cdn/worker/find-file-worker-263cab1760dd.js","findInFileWorkerPath":"/assets-cdn/worker/find-in-file-worker-881e9a930386.js","githubDevUrl":"https://github.dev/","enabled_features":{"code_nav_ui_events":false,"react_blob_overlay":true,"accessible_code_button":true,"github_models_repo_integration":false}}}</script>
  <div data-target="react-app.reactRoot"><meta data-hydrostats="publish"> <!-- --> <!-- --> <button hidden="" data-testid="header-permalink-button" data-hotkey-scope="read-only-cursor-text-area" data-hotkey="y,Shift+Y"></button><button hidden="" data-hotkey="y,Shift+Y"></button><div><div style="--sticky-pane-height: calc(100vh - (max(104px, 0px))); --spacing: var(--spacing-none);" class="Box-sc-g0xbh4-0 prc-PageLayout-PageLayoutRoot-1zlEO"><div class="prc-PageLayout-PageLayoutWrapper-s2ao4" data-width="full"><div class="prc-PageLayout-PageLayoutContent-jzDMn"><div tabindex="0" class="Box-sc-g0xbh4-0 gISSDQ"><div class="Box-sc-g0xbh4-0 prc-PageLayout-PaneWrapper-nGO0U ReposFileTreePane-module__Pane--wS7IV ReposFileTreePane-module__HidePane--Gj4XZ" style="--offset-header:0px;--spacing-row:var(--spacing-none);--spacing-column:var(--spacing-none)" data-is-hidden="false" data-position="start" data-sticky="true"><div class="Box-sc-g0xbh4-0 prc-PageLayout-HorizontalDivider-CYLp5 prc-PageLayout-PaneHorizontalDivider-4exOb" data-variant="none" data-position="start" style="--spacing-divider:var(--spacing-none);--spacing:var(--spacing-none)"></div><div class="prc-PageLayout-Pane-Vl5LI" data-resizable="true" style="--spacing:var(--spacing-none);--pane-min-width:256px;--pane-max-width:calc(100vw - var(--pane-max-width-diff));--pane-width-size:var(--pane-width-large);--pane-width:320px"><div><div id="repos-file-tree" class="Box-sc-g0xbh4-0 bNhwaa"><div class="Box-sc-g0xbh4-0 hNNCwk"><div class="Box-sc-g0xbh4-0 jfIeyl"><h2 class="Box-sc-g0xbh4-0 XosP prc-Heading-Heading-6CmGO"><span role="tooltip" aria-label="Collapse file tree" id="expand-button-file-tree-button" class="Tooltip__TooltipBase-sc-17tf59c-0 hWlpPn tooltipped-se"><button data-component="IconButton" type="button" data-testid="collapse-file-tree-button" aria-expanded="true" aria-controls="repos-file-tree" data-analytics-opt-out="true" class="prc-Button-ButtonBase-c50BI position-relative ExpandFileTreeButton-module__expandButton--gL4is fgColor-muted prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="medium" data-variant="invisible" aria-describedby=":R356mplab:-loading-announcement" aria-labelledby="expand-button-file-tree-button" data-hotkey="Control+b"><svg aria-hidden="true" focusable="false" class="octicon octicon-sidebar-expand" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align:text-bottom"><path d="m4.177 7.823 2.396-2.396A.25.25 0 0 1 7 5.604v4.792a.25.25 0 0 1-.427.177L4.177 8.177a.25.25 0 0 1 0-.354Z"></path><path d="M0 1.75C0 .784.784 0 1.75 0h12.5C15.216 0 16 .784 16 1.75v12.5A1.75 1.75 0 0 1 14.25 16H1.75A1.75 1.75 0 0 1 0 14.25Zm1.75-.25a.25.25 0 0 0-.25.25v12.5c0 .138.112.25.25.25H9.5v-13Zm12.5 13a.25.25 0 0 0 .25-.25V1.75a.25.25 0 0 0-.25-.25H11v13Z"></path></svg></button></span><button hidden="" data-testid="" data-hotkey-scope="read-only-cursor-text-area" data-hotkey="Control+b"></button></h2><h2 class="Box-sc-g0xbh4-0 kOkWgo prc-Heading-Heading-6CmGO">Files</h2></div><div class="Box-sc-g0xbh4-0 lhbroM"><div class="Box-sc-g0xbh4-0 khzwtX"><button type="button" aria-haspopup="true" aria-expanded="false" tabindex="0" aria-label="main branch" data-testid="anchor-button" class="Box-sc-g0xbh4-0 gMOVLe prc-Button-ButtonBase-c50BI react-repos-tree-pane-ref-selector width-full ref-selector-class" data-loading="false" data-size="medium" data-variant="default" aria-describedby="branch-picker-repos-header-ref-selector-loading-announcement" id="branch-picker-repos-header-ref-selector" data-hotkey="w"><span data-component="buttonContent" class="Box-sc-g0xbh4-0 gUkoLg prc-Button-ButtonContent-HKbr-"><span data-component="text" class="prc-Button-Label-pTQ3x"><div class="Box-sc-g0xbh4-0 bZBlpz"><div class="Box-sc-g0xbh4-0 lhTYNA"><svg aria-hidden="true" focusable="false" class="octicon octicon-git-branch" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align:text-bottom"><path d="M9.5 3.25a2.25 2.25 0 1 1 3 2.122V6A2.5 2.5 0 0 1 10 8.5H6a1 1 0 0 0-1 1v1.128a2.251 2.251 0 1 1-1.5 0V5.372a2.25 2.25 0 1 1 1.5 0v1.836A2.493 2.493 0 0 1 6 7h4a1 1 0 0 0 1-1v-.628A2.25 2.25 0 0 1 9.5 3.25Zm-6 0a.75.75 0 1 0 1.5 0 .75.75 0 0 0-1.5 0Zm8.25-.75a.75.75 0 1 0 0 1.5.75.75 0 0 0 0-1.5ZM4.25 12a.75.75 0 1 0 0 1.5.75.75 0 0 0 0-1.5Z"></path></svg></div><div class="Box-sc-g0xbh4-0 ffLUq ref-selector-button-text-container"><span class="Box-sc-g0xbh4-0 bmcJak prc-Text-Text-0ima0">&nbsp;<!-- -->main</span></div></div></span><span data-component="trailingVisual" class="prc-Button-Visual-2epfX prc-Button-VisualWrap-Db-eB"><svg aria-hidden="true" focusable="false" class="octicon octicon-triangle-down" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align:text-bottom"><path d="m4.427 7.427 3.396 3.396a.25.25 0 0 0 .354 0l3.396-3.396A.25.25 0 0 0 11.396 7H4.604a.25.25 0 0 0-.177.427Z"></path></svg></span></span></button><button hidden="" data-hotkey-scope="read-only-cursor-text-area" data-hotkey="w"></button></div><div class="Box-sc-g0xbh4-0 eTeVqd"><a sx="[object Object]" data-component="IconButton" type="button" aria-label="Add file" class="Box-sc-g0xbh4-0 fhbevO prc-Button-ButtonBase-c50BI prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="medium" data-variant="default" aria-describedby=":R6q6mplab:-loading-announcement :Rq6mplab:" href="https://github.com/Kiran437228/Module1/new/main"><svg aria-hidden="true" focusable="false" class="octicon octicon-plus" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align:text-bottom"><path d="M7.75 2a.75.75 0 0 1 .75.75V7h4.25a.75.75 0 0 1 0 1.5H8.5v4.25a.75.75 0 0 1-1.5 0V8.5H2.75a.75.75 0 0 1 0-1.5H7V2.75A.75.75 0 0 1 7.75 2Z"></path></svg></a><span class="prc-TooltipV2-Tooltip-cYMVY" data-direction="s" aria-label="Add file" role="tooltip" aria-hidden="true" id=":Rq6mplab:" popover="auto">Add file</span><button data-component="IconButton" type="button" aria-label="Search this repository" class="Box-sc-g0xbh4-0 fCjIQM prc-Button-ButtonBase-c50BI prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="medium" data-variant="default" aria-describedby=":R3a6mplab:-loading-announcement" data-hotkey="/"><svg aria-hidden="true" focusable="false" class="octicon octicon-search" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align:text-bottom"><path d="M10.68 11.74a6 6 0 0 1-7.922-8.982 6 6 0 0 1 8.982 7.922l3.04 3.04a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215ZM11.5 7a4.499 4.499 0 1 0-8.997 0A4.499 4.499 0 0 0 11.5 7Z"></path></svg></button><button hidden="" data-testid="" data-hotkey-scope="read-only-cursor-text-area" data-hotkey="/"></button></div></div></div><div class="Box-sc-g0xbh4-0 qkmJR"><span class="Box-sc-g0xbh4-0 vcvyP TextInput-wrapper prc-components-TextInputWrapper-i1ofR prc-components-TextInputBaseWrapper-ueK9q" data-leading-visual="true" data-trailing-visual="true" aria-busy="false"><span class="TextInput-icon" id=":R5amplab:" aria-hidden="true"><svg aria-hidden="true" focusable="false" class="octicon octicon-search" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align:text-bottom"><path d="M10.68 11.74a6 6 0 0 1-7.922-8.982 6 6 0 0 1 8.982 7.922l3.04 3.04a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215ZM11.5 7a4.499 4.499 0 1 0-8.997 0A4.499 4.499 0 0 0 11.5 7Z"></path></svg></span><input type="text" aria-label="Go to file" role="combobox" aria-controls="file-results-list" aria-expanded="false" aria-haspopup="dialog" autocorrect="off" spellcheck="false" placeholder="Go to file" aria-describedby=":R5amplab: :R5amplabH1:" data-component="input" class="prc-components-Input-Ic-y8" value=""><span class="TextInput-icon" id=":R5amplabH1:" aria-hidden="true"><div class="Box-sc-g0xbh4-0 dItACB"><kbd>t</kbd></div></span></span></div><button hidden="" data-testid="" data-hotkey-scope="read-only-cursor-text-area" data-hotkey="t,Shift+T"></button><button hidden="" data-hotkey="t,Shift+T"></button><div class="Box-sc-g0xbh4-0 jbQqON"><div><div class="react-tree-show-tree-items"><div class="Box-sc-g0xbh4-0 cOxzdh" data-testid="repos-file-tree-container"><nav aria-label="File Tree Navigation"><span role="status" aria-live="polite" aria-atomic="true" class="_VisuallyHidden__VisuallyHidden-sc-11jhm7a-0 brGdpi"></span><ul role="tree" aria-label="Files" data-truncate-text="true" class="prc-TreeView-TreeViewRootUlStyles-eZtxW"><li class="PRIVATE_TreeView-item prc-TreeView-TreeViewItem-ShJr0" tabindex="0" id="Conditional Statements in Python: Even or Odd Checker.md-item" role="treeitem" aria-labelledby=":r70:" aria-describedby=":r71:" aria-level="1" aria-selected="false" aria-current="true"><div class="PRIVATE_TreeView-item-container prc-TreeView-TreeViewItemContainer--2Rkn" style="--level: 1;"><div style="grid-area: spacer; display: flex;"><div style="width: 100%; display: flex;"></div></div><div id=":r70:" class="PRIVATE_TreeView-item-content prc-TreeView-TreeViewItemContent-f0r0b"><div class="PRIVATE_VisuallyHidden prc-TreeView-TreeViewVisuallyHidden-4-mPv" aria-hidden="true" id=":r71:"></div><div class="PRIVATE_TreeView-item-visual prc-TreeView-TreeViewItemVisual-dRlGq" aria-hidden="true"><svg aria-hidden="true" focusable="false" class="octicon octicon-file" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M2 1.75C2 .784 2.784 0 3.75 0h6.586c.464 0 .909.184 1.237.513l2.914 2.914c.329.328.513.773.513 1.237v9.586A1.75 1.75 0 0 1 13.25 16h-9.5A1.75 1.75 0 0 1 2 14.25Zm1.75-.25a.25.25 0 0 0-.25.25v12.5c0 .138.112.25.25.25h9.5a.25.25 0 0 0 .25-.25V6h-2.75A1.75 1.75 0 0 1 9 4.25V1.5Zm6.75.062V4.25c0 .138.112.25.25.25h2.688l-.011-.013-2.914-2.914-.013-.011Z"></path></svg></div><span class="PRIVATE_TreeView-item-content-text prc-TreeView-TreeViewItemContentText-smZM-"><span>Conditional Statements in Python: Even or Odd Checker.md</span></span></div></div></li><li class="PRIVATE_TreeView-item prc-TreeView-TreeViewItem-ShJr0" tabindex="-1" id="Datatypes-Boolean Expression Evaluation.md-item" role="treeitem" aria-labelledby=":r73:" aria-describedby=":r74:" aria-level="1" aria-selected="false"><div class="PRIVATE_TreeView-item-container prc-TreeView-TreeViewItemContainer--2Rkn" style="--level: 1; content-visibility: auto; contain-intrinsic-size: auto 2rem;"><div style="grid-area: spacer; display: flex;"><div style="width: 100%; display: flex;"></div></div><div id=":r73:" class="PRIVATE_TreeView-item-content prc-TreeView-TreeViewItemContent-f0r0b"><div class="PRIVATE_VisuallyHidden prc-TreeView-TreeViewVisuallyHidden-4-mPv" aria-hidden="true" id=":r74:"></div><div class="PRIVATE_TreeView-item-visual prc-TreeView-TreeViewItemVisual-dRlGq" aria-hidden="true"><svg aria-hidden="true" focusable="false" class="octicon octicon-file" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M2 1.75C2 .784 2.784 0 3.75 0h6.586c.464 0 .909.184 1.237.513l2.914 2.914c.329.328.513.773.513 1.237v9.586A1.75 1.75 0 0 1 13.25 16h-9.5A1.75 1.75 0 0 1 2 14.25Zm1.75-.25a.25.25 0 0 0-.25.25v12.5c0 .138.112.25.25.25h9.5a.25.25 0 0 0 .25-.25V6h-2.75A1.75 1.75 0 0 1 9 4.25V1.5Zm6.75.062V4.25c0 .138.112.25.25.25h2.688l-.011-.013-2.914-2.914-.013-.011Z"></path></svg></div><span class="PRIVATE_TreeView-item-content-text prc-TreeView-TreeViewItemContentText-smZM-"><span>Datatypes-Boolean Expression Evaluation.md</span></span></div></div></li><li class="PRIVATE_TreeView-item prc-TreeView-TreeViewItem-ShJr0" tabindex="-1" id="Datatypes-Character Literals.md-item" role="treeitem" aria-labelledby=":r76:" aria-describedby=":r77:" aria-level="1" aria-selected="false"><div class="PRIVATE_TreeView-item-container prc-TreeView-TreeViewItemContainer--2Rkn" style="--level: 1; content-visibility: auto; contain-intrinsic-size: auto 2rem;"><div style="grid-area: spacer; display: flex;"><div style="width: 100%; display: flex;"></div></div><div id=":r76:" class="PRIVATE_TreeView-item-content prc-TreeView-TreeViewItemContent-f0r0b"><div class="PRIVATE_VisuallyHidden prc-TreeView-TreeViewVisuallyHidden-4-mPv" aria-hidden="true" id=":r77:"></div><div class="PRIVATE_TreeView-item-visual prc-TreeView-TreeViewItemVisual-dRlGq" aria-hidden="true"><svg aria-hidden="true" focusable="false" class="octicon octicon-file" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M2 1.75C2 .784 2.784 0 3.75 0h6.586c.464 0 .909.184 1.237.513l2.914 2.914c.329.328.513.773.513 1.237v9.586A1.75 1.75 0 0 1 13.25 16h-9.5A1.75 1.75 0 0 1 2 14.25Zm1.75-.25a.25.25 0 0 0-.25.25v12.5c0 .138.112.25.25.25h9.5a.25.25 0 0 0 .25-.25V6h-2.75A1.75 1.75 0 0 1 9 4.25V1.5Zm6.75.062V4.25c0 .138.112.25.25.25h2.688l-.011-.013-2.914-2.914-.013-.011Z"></path></svg></div><span class="PRIVATE_TreeView-item-content-text prc-TreeView-TreeViewItemContentText-smZM-"><span>Datatypes-Character Literals.md</span></span></div></div></li><li class="PRIVATE_TreeView-item prc-TreeView-TreeViewItem-ShJr0" tabindex="-1" id="Datatypes-Complex Number.md-item" role="treeitem" aria-labelledby=":r79:" aria-describedby=":r7a:" aria-level="1" aria-selected="false"><div class="PRIVATE_TreeView-item-container prc-TreeView-TreeViewItemContainer--2Rkn" style="--level: 1; content-visibility: auto; contain-intrinsic-size: auto 2rem;"><div style="grid-area: spacer; display: flex;"><div style="width: 100%; display: flex;"></div></div><div id=":r79:" class="PRIVATE_TreeView-item-content prc-TreeView-TreeViewItemContent-f0r0b"><div class="PRIVATE_VisuallyHidden prc-TreeView-TreeViewVisuallyHidden-4-mPv" aria-hidden="true" id=":r7a:"></div><div class="PRIVATE_TreeView-item-visual prc-TreeView-TreeViewItemVisual-dRlGq" aria-hidden="true"><svg aria-hidden="true" focusable="false" class="octicon octicon-file" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M2 1.75C2 .784 2.784 0 3.75 0h6.586c.464 0 .909.184 1.237.513l2.914 2.914c.329.328.513.773.513 1.237v9.586A1.75 1.75 0 0 1 13.25 16h-9.5A1.75 1.75 0 0 1 2 14.25Zm1.75-.25a.25.25 0 0 0-.25.25v12.5c0 .138.112.25.25.25h9.5a.25.25 0 0 0 .25-.25V6h-2.75A1.75 1.75 0 0 1 9 4.25V1.5Zm6.75.062V4.25c0 .138.112.25.25.25h2.688l-.011-.013-2.914-2.914-.013-.011Z"></path></svg></div><span class="PRIVATE_TreeView-item-content-text prc-TreeView-TreeViewItemContentText-smZM-"><span>Datatypes-Complex Number.md</span></span></div></div></li><li class="PRIVATE_TreeView-item prc-TreeView-TreeViewItem-ShJr0" tabindex="-1" id="Datatypes-String Literals.md-item" role="treeitem" aria-labelledby=":r7c:" aria-describedby=":r7d:" aria-level="1" aria-selected="false"><div class="PRIVATE_TreeView-item-container prc-TreeView-TreeViewItemContainer--2Rkn" style="--level: 1; content-visibility: auto; contain-intrinsic-size: auto 2rem;"><div style="grid-area: spacer; display: flex;"><div style="width: 100%; display: flex;"></div></div><div id=":r7c:" class="PRIVATE_TreeView-item-content prc-TreeView-TreeViewItemContent-f0r0b"><div class="PRIVATE_VisuallyHidden prc-TreeView-TreeViewVisuallyHidden-4-mPv" aria-hidden="true" id=":r7d:"></div><div class="PRIVATE_TreeView-item-visual prc-TreeView-TreeViewItemVisual-dRlGq" aria-hidden="true"><svg aria-hidden="true" focusable="false" class="octicon octicon-file" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M2 1.75C2 .784 2.784 0 3.75 0h6.586c.464 0 .909.184 1.237.513l2.914 2.914c.329.328.513.773.513 1.237v9.586A1.75 1.75 0 0 1 13.25 16h-9.5A1.75 1.75 0 0 1 2 14.25Zm1.75-.25a.25.25 0 0 0-.25.25v12.5c0 .138.112.25.25.25h9.5a.25.25 0 0 0 .25-.25V6h-2.75A1.75 1.75 0 0 1 9 4.25V1.5Zm6.75.062V4.25c0 .138.112.25.25.25h2.688l-.011-.013-2.914-2.914-.013-.011Z"></path></svg></div><span class="PRIVATE_TreeView-item-content-text prc-TreeView-TreeViewItemContentText-smZM-"><span>Datatypes-String Literals.md</span></span></div></div></li></ul></nav></div></div></div></div></div></div></div><div class="Box-sc-g0xbh4-0 prc-PageLayout-VerticalDivider-4A4Qm prc-PageLayout-PaneVerticalDivider-1c9vy" data-variant="line" data-position="start" style="--spacing:var(--spacing-none)"><div role="slider" aria-label="Draggable pane splitter" aria-valuemin="256" aria-valuemax="569" aria-valuenow="320" aria-valuetext="Pane width 320 pixels" tabindex="0" class="Box-sc-g0xbh4-0 bHLmSv"></div></div></div></div><div class="Box-sc-g0xbh4-0 prc-PageLayout-ContentWrapper-b-QRo CodeView-module__SplitPageLayout_Content--qxR1C" data-is-hidden="false"><div></div><div class="prc-PageLayout-Content--F7-I" data-width="full" style="--spacing:var(--spacing-none)"><div data-selector="repos-split-pane-content" tabindex="0" class="Box-sc-g0xbh4-0 leYMvG"><div class="Box-sc-g0xbh4-0 KMPzq"><div class="container CodeViewHeader-module__Box--PofRM"><div class="px-3 pt-3 pb-0" id="StickyHeader"><div class="CodeViewHeader-module__Box_1--KpLzV"><div class="CodeViewHeader-module__Box_2--xzDOt"><div class="CodeViewHeader-module__Box_6--iStzT"><div class="Box-sc-g0xbh4-0 cEytCf"><nav data-testid="breadcrumbs" aria-labelledby="repos-header-breadcrumb--wide-heading" id="repos-header-breadcrumb--wide" class="Box-sc-g0xbh4-0 fzFXnm"><h2 class="sr-only ScreenReaderHeading-module__userSelectNone--vW4Cq prc-Heading-Heading-6CmGO" data-testid="screen-reader-heading" id="repos-header-breadcrumb--wide-heading">Breadcrumbs</h2><ol class="Box-sc-g0xbh4-0 iMnkmv"><li class="Box-sc-g0xbh4-0 ghzDag"><a class="Box-sc-g0xbh4-0 kHuKdh prc-Link-Link-85e08" sx="[object Object]" data-testid="breadcrumbs-repo-link" href="https://github.com/Kiran437228/Module1/tree/main">Module1</a></li></ol></nav><div data-testid="breadcrumbs-filename" class="Box-sc-g0xbh4-0 ghzDag"><span class="Box-sc-g0xbh4-0 hzJBof prc-Text-Text-0ima0" aria-hidden="true">/</span><h1 class="Box-sc-g0xbh4-0 jGhzSQ prc-Heading-Heading-6CmGO" tabindex="-1" id="file-name-id-wide">Conditional Statements in Python: Even or Odd Checker.md</h1></div><button data-component="IconButton" type="button" class="prc-Button-ButtonBase-c50BI ml-2 prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="small" data-variant="invisible" aria-describedby=":R3td9lab:-loading-announcement" aria-labelledby=":Rdd9lab:"><svg aria-hidden="true" focusable="false" class="octicon octicon-copy" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align:text-bottom"><path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path></svg></button><span class="CopyToClipboardButton-module__tooltip--Dq1IB prc-TooltipV2-Tooltip-cYMVY" data-direction="nw" aria-label="Copy path" aria-hidden="true" id=":Rdd9lab:" popover="auto">Copy path</span></div></div><div class="react-code-view-header-element--wide"><div class="CodeViewHeader-module__Box_7--FZfkg"><div class="d-flex gap-2"> <button type="button" data-hotkey="b,Shift+B,Control+/ Control+b" class="Box-sc-g0xbh4-0 fjrFuv prc-Button-ButtonBase-c50BI NavigationMenu-module__Button--SJihq" data-loading="false" data-no-visuals="true" data-size="medium" data-variant="default" aria-describedby=":r8i:-loading-announcement"><span data-component="buttonContent" class="Box-sc-g0xbh4-0 gUkoLg prc-Button-ButtonContent-HKbr-"><span data-component="text" class="prc-Button-Label-pTQ3x">Blame</span></span></button><button hidden="" data-testid="" data-hotkey="b,Shift+B,Control+/ Control+b" data-hotkey-scope="read-only-cursor-text-area"></button><button data-component="IconButton" type="button" aria-label="More file actions" title="More file actions" data-testid="more-file-actions-button-nav-menu-wide" aria-haspopup="true" aria-expanded="false" tabindex="0" class="prc-Button-ButtonBase-c50BI js-blob-dropdown-click NavigationMenu-module__IconButton--NqJ_L prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="medium" data-variant="default" aria-describedby=":r8j:-loading-announcement" id=":r8j:"><svg aria-hidden="true" focusable="false" class="octicon octicon-kebab-horizontal" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M8 9a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3ZM1.5 9a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Zm13 0a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Z"></path></svg></button> </div></div></div><div class="react-code-view-header-element--narrow"><div class="CodeViewHeader-module__Box_7--FZfkg"><div class="d-flex gap-2"> <button type="button" data-hotkey="b,Shift+B,Control+/ Control+b" class="Box-sc-g0xbh4-0 fjrFuv prc-Button-ButtonBase-c50BI NavigationMenu-module__Button--SJihq" data-loading="false" data-no-visuals="true" data-size="medium" data-variant="default" aria-describedby=":r8m:-loading-announcement"><span data-component="buttonContent" class="Box-sc-g0xbh4-0 gUkoLg prc-Button-ButtonContent-HKbr-"><span data-component="text" class="prc-Button-Label-pTQ3x">Blame</span></span></button><button hidden="" data-testid="" data-hotkey="b,Shift+B,Control+/ Control+b" data-hotkey-scope="read-only-cursor-text-area"></button><button data-component="IconButton" type="button" aria-label="More file actions" title="More file actions" data-testid="more-file-actions-button-nav-menu-narrow" aria-haspopup="true" aria-expanded="false" tabindex="0" class="prc-Button-ButtonBase-c50BI js-blob-dropdown-click NavigationMenu-module__IconButton--NqJ_L prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="medium" data-variant="default" aria-describedby=":r8n:-loading-announcement" id=":r8n:"><svg aria-hidden="true" focusable="false" class="octicon octicon-kebab-horizontal" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M8 9a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3ZM1.5 9a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Zm13 0a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Z"></path></svg></button> </div></div></div></div></div></div></div></div><div class="Box-sc-g0xbh4-0 dJxjrT react-code-view-bottom-padding"><!-- --><!-- --> <div class="BlobTopBanners-module__Box--g_bGk"></div>   </div><div class="Box-sc-g0xbh4-0 dJxjrT"><!-- --><!-- --><!-- --><!-- -->   <button hidden="" data-testid="" data-hotkey="r,Shift+R" data-hotkey-scope="read-only-cursor-text-area"></button><button hidden="" data-hotkey="r,Shift+R"></button><div class="d-flex flex-column border rounded-2 mb-3 pl-1"><div class="Box-sc-g0xbh4-0 dzCJzi"><h2 class="sr-only ScreenReaderHeading-module__userSelectNone--vW4Cq prc-Heading-Heading-6CmGO" data-testid="screen-reader-heading">Latest commit</h2><div data-testid="latest-commit" class="Box-sc-g0xbh4-0 ePWWCk"><div class="Box-sc-g0xbh4-0 dpBUfI"><div data-testid="author-avatar" class="Box-sc-g0xbh4-0 hKWjvQ"><a class="prc-Link-Link-85e08" href="https://github.com/Kiran437228" data-testid="avatar-icon-link" data-hovercard-url="/users/Kiran437228/hovercard"><img data-component="Avatar" class="Box-sc-g0xbh4-0 cvdqJW prc-Avatar-Avatar-ZRS-m" alt="Kiran437228" width="20" height="20" src="./Conditional Statements in Python_ Even or Odd Checker_files/182343513" data-testid="github-avatar" aria-label="Kiran437228" style="--avatarSize-regular: 20px;"></a><a class="Box-sc-g0xbh4-0 dkaFxu prc-Link-Link-85e08" data-muted="true" href="https://github.com/Kiran437228/Module1/commits?author=Kiran437228" aria-label="commits by Kiran437228" data-hovercard-url="/users/Kiran437228/hovercard">Kiran437228</a></div><span class=""></span></div><div class="Box-sc-g0xbh4-0 erEOeb d-none d-sm-flex"><div class="Truncate flex-items-center f5"><span class="Truncate-text prc-Text-Text-0ima0" data-testid="latest-commit-html"><a href="https://github.com/Kiran437228/Module1/commit/6cdfb9175f9baeb34691bf5b3197f03830452226" class="Link--secondary" data-pjax="true" data-hovercard-url="/Kiran437228/Module1/commit/6cdfb9175f9baeb34691bf5b3197f03830452226/hovercard">Update Conditional Statements in Python: Even or Odd Checker.md</a></span></div></div><span class="d-flex d-sm-none fgColor-muted f6"><relative-time class="sc-aXZVg" tense="past" datetime="2025-04-28T18:40:14.000Z" title="Apr 29, 2025, 12:10 AM GMT+5:30"><template shadowrootmode="open">2 weeks ago</template>Apr 29, 2025</relative-time></span></div><div class="d-flex flex-shrink-0 gap-2"><div data-testid="latest-commit-details" class="d-none d-sm-flex flex-items-center"><span class="d-flex flex-nowrap fgColor-muted f6"><a class="Link--secondary prc-Link-Link-85e08" aria-label="Commit 6cdfb91" data-hovercard-url="/Kiran437228/Module1/commit/6cdfb9175f9baeb34691bf5b3197f03830452226/hovercard" href="https://github.com/Kiran437228/Module1/commit/6cdfb9175f9baeb34691bf5b3197f03830452226">6cdfb91</a>&nbsp;·&nbsp;<relative-time class="sc-aXZVg" tense="past" datetime="2025-04-28T18:40:14.000Z" title="Apr 29, 2025, 12:10 AM GMT+5:30"><template shadowrootmode="open">2 weeks ago</template>Apr 29, 2025</relative-time></span></div><div class="d-flex gap-2"><h2 class="sr-only ScreenReaderHeading-module__userSelectNone--vW4Cq prc-Heading-Heading-6CmGO" data-testid="screen-reader-heading">History</h2><a href="https://github.com/Kiran437228/Module1/commits/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md" class="prc-Button-ButtonBase-c50BI d-none d-lg-flex LinkButton-module__code-view-link-button--xvCGA flex-items-center fgColor-default" data-loading="false" data-size="small" data-variant="invisible" aria-describedby=":r8q:-loading-announcement"><span data-component="buttonContent" data-align="center" class="prc-Button-ButtonContent-HKbr-"><span data-component="leadingVisual" class="prc-Button-Visual-2epfX prc-Button-VisualWrap-Db-eB"><svg aria-hidden="true" focusable="false" class="octicon octicon-history" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="m.427 1.927 1.215 1.215a8.002 8.002 0 1 1-1.6 5.685.75.75 0 1 1 1.493-.154 6.5 6.5 0 1 0 1.18-4.458l1.358 1.358A.25.25 0 0 1 3.896 6H.25A.25.25 0 0 1 0 5.75V2.104a.25.25 0 0 1 .427-.177ZM7.75 4a.75.75 0 0 1 .75.75v2.992l2.028.812a.75.75 0 0 1-.557 1.392l-2.5-1A.751.751 0 0 1 7 8.25v-3.5A.75.75 0 0 1 7.75 4Z"></path></svg></span><span data-component="text" class="prc-Button-Label-pTQ3x"><span class="fgColor-default">History</span></span></span></a><div class="d-sm-none"><button data-component="IconButton" type="button" aria-label="Open commit details" aria-pressed="false" aria-expanded="false" data-testid="latest-commit-details-toggle" class="Box-sc-g0xbh4-0 hdOVEE prc-Button-ButtonBase-c50BI prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="small" data-variant="invisible" aria-describedby=":ra3:-loading-announcement"><svg aria-hidden="true" focusable="false" class="octicon octicon-ellipsis" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M0 5.75C0 4.784.784 4 1.75 4h12.5c.966 0 1.75.784 1.75 1.75v4.5A1.75 1.75 0 0 1 14.25 12H1.75A1.75 1.75 0 0 1 0 10.25ZM12 7a1 1 0 1 0 0 2 1 1 0 0 0 0-2ZM7 8a1 1 0 1 0 2 0 1 1 0 0 0-2 0ZM4 7a1 1 0 1 0 0 2 1 1 0 0 0 0-2Z"></path></svg></button></div><div class="d-flex d-lg-none"><span role="tooltip" aria-label="History" id="history-icon-button-tooltip" class="Tooltip__TooltipBase-sc-17tf59c-0 hWlpPn tooltipped-n"><a href="https://github.com/Kiran437228/Module1/commits/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md" class="prc-Button-ButtonBase-c50BI LinkButton-module__code-view-link-button--xvCGA flex-items-center fgColor-default" data-loading="false" data-size="small" data-variant="invisible" aria-describedby=":r8s:-loading-announcement history-icon-button-tooltip"><span data-component="buttonContent" data-align="center" class="prc-Button-ButtonContent-HKbr-"><span data-component="leadingVisual" class="prc-Button-Visual-2epfX prc-Button-VisualWrap-Db-eB"><svg aria-hidden="true" focusable="false" class="octicon octicon-history" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="m.427 1.927 1.215 1.215a8.002 8.002 0 1 1-1.6 5.685.75.75 0 1 1 1.493-.154 6.5 6.5 0 1 0 1.18-4.458l1.358 1.358A.25.25 0 0 1 3.896 6H.25A.25.25 0 0 1 0 5.75V2.104a.25.25 0 0 1 .427-.177ZM7.75 4a.75.75 0 0 1 .75.75v2.992l2.028.812a.75.75 0 0 1-.557 1.392l-2.5-1A.751.751 0 0 1 7 8.25v-3.5A.75.75 0 0 1 7.75 4Z"></path></svg></span></span></a></span></div></div></div></div></div><div class="Box-sc-g0xbh4-0 ldRxiI"><div class="Box-sc-g0xbh4-0 fVkfyA container"><div class="Box-sc-g0xbh4-0 gNAmSV react-code-size-details-banner"><div class="react-code-size-details-banner CodeSizeDetails-module__Box--QdxnQ"><div class="text-mono CodeSizeDetails-module__Box_1--_uFDs"><div title="690 Bytes" data-testid="blob-size" class="Truncate__StyledTruncate-sc-23o1d2-0 bgsFir CodeSizeDetails-module__Truncate_1--er0Uk"><span>27 lines (22 loc) · 690 Bytes</span></div></div></div><div class="react-code-size-details-banner"><button type="button" aria-haspopup="true" aria-expanded="false" tabindex="0" class="Box-sc-g0xbh4-0 kXyYCF prc-Button-ButtonBase-c50BI" data-loading="false" data-size="small" data-variant="invisible" aria-describedby=":r8t:-loading-announcement" id=":r8t:" style="--button-color: fg.default;"><span data-component="buttonContent" class="Box-sc-g0xbh4-0 gUkoLg prc-Button-ButtonContent-HKbr-"><span data-component="leadingVisual" class="prc-Button-Visual-2epfX prc-Button-VisualWrap-Db-eB"><svg aria-hidden="true" focusable="false" class="octicon octicon-copilot" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M7.998 15.035c-4.562 0-7.873-2.914-7.998-3.749V9.338c.085-.628.677-1.686 1.588-2.065.013-.07.024-.143.036-.218.029-.183.06-.384.126-.612-.201-.508-.254-1.084-.254-1.656 0-.87.128-1.769.693-2.484.579-.733 1.494-1.124 2.724-1.261 1.206-.134 2.262.034 2.944.765.05.053.096.108.139.165.044-.057.094-.112.143-.165.682-.731 1.738-.899 2.944-.765 1.23.137 2.145.528 2.724 1.261.566.715.693 1.614.693 2.484 0 .572-.053 1.148-.254 1.656.066.228.098.429.126.612.012.076.024.148.037.218.924.385 1.522 1.471 1.591 2.095v1.872c0 .766-3.351 3.795-8.002 3.795Zm0-1.485c2.28 0 4.584-1.11 5.002-1.433V7.862l-.023-.116c-.49.21-1.075.291-1.727.291-1.146 0-2.059-.327-2.71-.991A3.222 3.222 0 0 1 8 6.303a3.24 3.24 0 0 1-.544.743c-.65.664-1.563.991-2.71.991-.652 0-1.236-.081-1.727-.291l-.023.116v4.255c.419.323 2.722 1.433 5.002 1.433ZM6.762 2.83c-.193-.206-.637-.413-1.682-.297-1.019.113-1.479.404-1.713.7-.247.312-.369.789-.369 1.554 0 .793.129 1.171.308 1.371.162.181.519.379 1.442.379.853 0 1.339-.235 1.638-.54.315-.322.527-.827.617-1.553.117-.935-.037-1.395-.241-1.614Zm4.155-.297c-1.044-.116-1.488.091-1.681.297-.204.219-.359.679-.242 1.614.091.726.303 1.231.618 1.553.299.305.784.54 1.638.54.922 0 1.28-.198 1.442-.379.179-.2.308-.578.308-1.371 0-.765-.123-1.242-.37-1.554-.233-.296-.693-.587-1.713-.7Z"></path><path d="M6.25 9.037a.75.75 0 0 1 .75.75v1.501a.75.75 0 0 1-1.5 0V9.787a.75.75 0 0 1 .75-.75Zm4.25.75v1.501a.75.75 0 0 1-1.5 0V9.787a.75.75 0 0 1 1.5 0Z"></path></svg></span><span data-component="text" class="prc-Button-Label-pTQ3x">Code 55% faster with GitHub Copilot</span></span></button></div></div><div class="Box-sc-g0xbh4-0 jdLMhu react-blob-view-header-sticky" id="repos-sticky-header"><div class="BlobViewHeader-module__Box--pvsIA"><div class="react-blob-sticky-header"><div class="Box-sc-g0xbh4-0 hqwSEx"><div class="FileNameStickyHeader-module__Box_5--xBJ2J"><div class="Box-sc-g0xbh4-0 fHind"><nav data-testid="breadcrumbs" aria-labelledby="sticky-breadcrumb-heading" id="sticky-breadcrumb" class="Box-sc-g0xbh4-0 fzFXnm"><h2 class="sr-only ScreenReaderHeading-module__userSelectNone--vW4Cq prc-Heading-Heading-6CmGO" data-testid="screen-reader-heading" id="sticky-breadcrumb-heading">Breadcrumbs</h2><ol class="Box-sc-g0xbh4-0 iMnkmv"><li class="Box-sc-g0xbh4-0 ghzDag"><a class="Box-sc-g0xbh4-0 kHuKdh prc-Link-Link-85e08" sx="[object Object]" data-testid="breadcrumbs-repo-link" href="https://github.com/Kiran437228/Module1/tree/main">Module1</a></li></ol></nav><div data-testid="breadcrumbs-filename" class="Box-sc-g0xbh4-0 ghzDag"><span class="Box-sc-g0xbh4-0 oDtgN prc-Text-Text-0ima0" aria-hidden="true">/</span><h1 class="Box-sc-g0xbh4-0 dnZoUW prc-Heading-Heading-6CmGO" tabindex="-1" id="sticky-file-name-id">Conditional Statements in Python: Even or Odd Checker.md</h1></div></div><button type="button" class="prc-Button-ButtonBase-c50BI FileNameStickyHeader-module__Button--SaiiH FileNameStickyHeader-module__GoToTopButton--9lB4x" data-loading="false" data-size="small" data-variant="invisible" aria-describedby=":r8v:-loading-announcement"><span data-component="buttonContent" data-align="center" class="prc-Button-ButtonContent-HKbr-"><span data-component="leadingVisual" class="prc-Button-Visual-2epfX prc-Button-VisualWrap-Db-eB"><svg aria-hidden="true" focusable="false" class="octicon octicon-arrow-up" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M3.47 7.78a.75.75 0 0 1 0-1.06l4.25-4.25a.75.75 0 0 1 1.06 0l4.25 4.25a.751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018L9 4.81v7.44a.75.75 0 0 1-1.5 0V4.81L4.53 7.78a.75.75 0 0 1-1.06 0Z"></path></svg></span><span data-component="text" class="prc-Button-Label-pTQ3x">Top</span></span></button></div></div></div><div class="Box-sc-g0xbh4-0 gFKFyc BlobViewHeader-module__Box_1--PPihg"><h2 class="sr-only ScreenReaderHeading-module__userSelectNone--vW4Cq prc-Heading-Heading-6CmGO" data-testid="screen-reader-heading">File metadata and controls</h2><div class="BlobViewHeader-module__Box_2--G_jCG"><ul aria-label="File view" class="prc-SegmentedControl-SegmentedControl-e7570 BlobTabButtons-module__SegmentedControl--JMGov" data-size="small"><li class="Box-sc-g0xbh4-0 dXYHoy prc-SegmentedControl-Item-7Aq6h" data-selected="true"><button aria-current="true" class="prc-SegmentedControl-Button-ojWXD" type="button" data-hotkey="Control+/ Control+p"><span class="prc-SegmentedControl-Content-gnQ4n"><div class="Box-sc-g0xbh4-0 prc-SegmentedControl-Text-c5gSh" data-text="Preview">Preview</div></span></button></li><li class="Box-sc-g0xbh4-0 jBWIdY prc-SegmentedControl-Item-7Aq6h"><button aria-current="false" class="prc-SegmentedControl-Button-ojWXD" type="button" data-hotkey="Control+/ Control+c"><span class="prc-SegmentedControl-Content-gnQ4n"><div class="Box-sc-g0xbh4-0 prc-SegmentedControl-Text-c5gSh" data-text="Code">Code</div></span></button></li><li class="Box-sc-g0xbh4-0 jBWIdY prc-SegmentedControl-Item-7Aq6h"><button aria-current="false" class="prc-SegmentedControl-Button-ojWXD" type="button" data-hotkey="b,Shift+B,Control+/ Control+b"><span class="prc-SegmentedControl-Content-gnQ4n"><div class="Box-sc-g0xbh4-0 prc-SegmentedControl-Text-c5gSh" data-text="Blame">Blame</div></span></button></li></ul><button hidden="" data-testid="" data-hotkey="Control+/ Control+c" data-hotkey-scope="read-only-cursor-text-area"></button><button hidden="" data-testid="" data-hotkey="b,Shift+B,Control+/ Control+b" data-hotkey-scope="read-only-cursor-text-area"></button><button hidden="" data-testid="" data-hotkey="Control+/ Control+p" data-hotkey-scope="read-only-cursor-text-area"></button><div class="react-code-size-details-in-header CodeSizeDetails-module__Box--QdxnQ"><div class="text-mono CodeSizeDetails-module__Box_1--_uFDs"><div title="690 Bytes" data-testid="blob-size" class="Truncate__StyledTruncate-sc-23o1d2-0 bgsFir CodeSizeDetails-module__Truncate_1--er0Uk"><span>27 lines (22 loc) · 690 Bytes</span></div></div></div><div class="react-code-size-details-in-header"><button type="button" aria-haspopup="true" aria-expanded="false" tabindex="0" class="Box-sc-g0xbh4-0 kXyYCF prc-Button-ButtonBase-c50BI" data-loading="false" data-size="small" data-variant="invisible" aria-describedby=":r90:-loading-announcement" id=":r90:" style="--button-color: fg.default;"><span data-component="buttonContent" class="Box-sc-g0xbh4-0 gUkoLg prc-Button-ButtonContent-HKbr-"><span data-component="leadingVisual" class="prc-Button-Visual-2epfX prc-Button-VisualWrap-Db-eB"><svg aria-hidden="true" focusable="false" class="octicon octicon-copilot" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M7.998 15.035c-4.562 0-7.873-2.914-7.998-3.749V9.338c.085-.628.677-1.686 1.588-2.065.013-.07.024-.143.036-.218.029-.183.06-.384.126-.612-.201-.508-.254-1.084-.254-1.656 0-.87.128-1.769.693-2.484.579-.733 1.494-1.124 2.724-1.261 1.206-.134 2.262.034 2.944.765.05.053.096.108.139.165.044-.057.094-.112.143-.165.682-.731 1.738-.899 2.944-.765 1.23.137 2.145.528 2.724 1.261.566.715.693 1.614.693 2.484 0 .572-.053 1.148-.254 1.656.066.228.098.429.126.612.012.076.024.148.037.218.924.385 1.522 1.471 1.591 2.095v1.872c0 .766-3.351 3.795-8.002 3.795Zm0-1.485c2.28 0 4.584-1.11 5.002-1.433V7.862l-.023-.116c-.49.21-1.075.291-1.727.291-1.146 0-2.059-.327-2.71-.991A3.222 3.222 0 0 1 8 6.303a3.24 3.24 0 0 1-.544.743c-.65.664-1.563.991-2.71.991-.652 0-1.236-.081-1.727-.291l-.023.116v4.255c.419.323 2.722 1.433 5.002 1.433ZM6.762 2.83c-.193-.206-.637-.413-1.682-.297-1.019.113-1.479.404-1.713.7-.247.312-.369.789-.369 1.554 0 .793.129 1.171.308 1.371.162.181.519.379 1.442.379.853 0 1.339-.235 1.638-.54.315-.322.527-.827.617-1.553.117-.935-.037-1.395-.241-1.614Zm4.155-.297c-1.044-.116-1.488.091-1.681.297-.204.219-.359.679-.242 1.614.091.726.303 1.231.618 1.553.299.305.784.54 1.638.54.922 0 1.28-.198 1.442-.379.179-.2.308-.578.308-1.371 0-.765-.123-1.242-.37-1.554-.233-.296-.693-.587-1.713-.7Z"></path><path d="M6.25 9.037a.75.75 0 0 1 .75.75v1.501a.75.75 0 0 1-1.5 0V9.787a.75.75 0 0 1 .75-.75Zm4.25.75v1.501a.75.75 0 0 1-1.5 0V9.787a.75.75 0 0 1 1.5 0Z"></path></svg></span><span data-component="text" class="prc-Button-Label-pTQ3x">Code 55% faster with GitHub Copilot</span></span></button></div></div><div class="BlobViewHeader-module__Box_3--Kvpex"><button hidden="" data-testid="" data-hotkey="Control+Shift+&gt;" data-hotkey-scope="read-only-cursor-text-area"></button><button hidden="" data-hotkey="Control+Shift+&gt;"></button><button hidden="" data-testid="" data-hotkey="Control+Shift+&lt;" data-hotkey-scope="read-only-cursor-text-area"></button><button hidden="" data-hotkey="Control+Shift+&lt;"></button><div class="react-blob-header-edit-and-raw-actions BlobViewHeader-module__Box_4--vFP89"><div class="Box-sc-g0xbh4-0 prc-ButtonGroup-ButtonGroup-vcMeG"><div><a href="https://github.com/Kiran437228/Module1/raw/refs/heads/main/Conditional%20Statements%20in%20Python:%20Even%20or%20Odd%20Checker.md" data-testid="raw-button" data-hotkey="Control+/ Control+r" class="Box-sc-g0xbh4-0 lefpaC prc-Button-ButtonBase-c50BI BlobViewHeader-module__LinkButton--DMph4" data-loading="false" data-no-visuals="true" data-size="small" data-variant="default" aria-describedby=":r92:-loading-announcement"><span data-component="buttonContent" class="Box-sc-g0xbh4-0 gUkoLg prc-Button-ButtonContent-HKbr-"><span data-component="text" class="prc-Button-Label-pTQ3x">Raw</span></span></a></div><div><button data-component="IconButton" type="button" aria-label="Copy raw content" data-testid="copy-raw-button" data-hotkey="Control+Shift+C" class="prc-Button-ButtonBase-c50BI prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="small" data-variant="default" aria-describedby=":r93:-loading-announcement"><svg aria-hidden="true" focusable="false" class="octicon octicon-copy" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path></svg></button></div><div><span role="tooltip" aria-label="Download raw file" id=":r94:" class="Tooltip__TooltipBase-sc-17tf59c-0 hWlpPn tooltipped-n"><button data-component="IconButton" type="button" aria-label="Download raw content" data-testid="download-raw-button" data-hotkey="Control+Shift+S" class="Box-sc-g0xbh4-0 ivobqY prc-Button-ButtonBase-c50BI prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="small" data-variant="default" aria-describedby=":r95:-loading-announcement"><svg aria-hidden="true" focusable="false" class="octicon octicon-download" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M2.75 14A1.75 1.75 0 0 1 1 12.25v-2.5a.75.75 0 0 1 1.5 0v2.5c0 .138.112.25.25.25h10.5a.25.25 0 0 0 .25-.25v-2.5a.75.75 0 0 1 1.5 0v2.5A1.75 1.75 0 0 1 13.25 14Z"></path><path d="M7.25 7.689V2a.75.75 0 0 1 1.5 0v5.689l1.97-1.969a.749.749 0 1 1 1.06 1.06l-3.25 3.25a.749.749 0 0 1-1.06 0L4.22 6.78a.749.749 0 1 1 1.06-1.06l1.97 1.969Z"></path></svg></button></span></div></div><button hidden="" data-testid="raw-button-shortcut" data-hotkey="Control+/ Control+r" data-hotkey-scope="read-only-cursor-text-area"></button><button hidden="" data-testid="copy-raw-button-shortcut" data-hotkey="Control+Shift+C" data-hotkey-scope="read-only-cursor-text-area"></button><button hidden="" data-testid="download-raw-button-shortcut" data-hotkey="Control+Shift+S" data-hotkey-scope="read-only-cursor-text-area"></button><a class="js-github-dev-shortcut d-none prc-Link-Link-85e08" data-hotkey="., Control+Shift+/" href="https://github.dev/"></a><button hidden="" data-testid="" data-hotkey="., Control+Shift+/" data-hotkey-scope="read-only-cursor-text-area"></button><a class="js-github-dev-new-tab-shortcut d-none prc-Link-Link-85e08" data-hotkey="Shift+.,Shift+&gt;,&gt;" href="https://github.dev/" target="_blank"></a><button hidden="" data-testid="" data-hotkey="Shift+.,Shift+&gt;,&gt;" data-hotkey-scope="read-only-cursor-text-area"></button><div class="Box-sc-g0xbh4-0 prc-ButtonGroup-ButtonGroup-vcMeG"><div><span role="tooltip" aria-label="Edit the file in your fork of this project" id=":r96:" class="Tooltip__TooltipBase-sc-17tf59c-0 hWlpPn tooltipped-nw"><a sx="[object Object]" data-component="IconButton" type="button" aria-label="Edit file" data-hotkey="e,Shift+E" data-testid="edit-button" class="Box-sc-g0xbh4-0 iCOsHh prc-Button-ButtonBase-c50BI BlobViewHeader-module__IconButton_1--MzNlL prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="small" data-variant="default" aria-describedby=":r97:-loading-announcement" href="https://github.com/Kiran437228/Module1/edit/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md"><svg aria-hidden="true" focusable="false" class="octicon octicon-pencil" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M11.013 1.427a1.75 1.75 0 0 1 2.474 0l1.086 1.086a1.75 1.75 0 0 1 0 2.474l-8.61 8.61c-.21.21-.47.364-.756.445l-3.251.93a.75.75 0 0 1-.927-.928l.929-3.25c.081-.286.235-.547.445-.758l8.61-8.61Zm.176 4.823L9.75 4.81l-6.286 6.287a.253.253 0 0 0-.064.108l-.558 1.953 1.953-.558a.253.253 0 0 0 .108-.064Zm1.238-3.763a.25.25 0 0 0-.354 0L10.811 3.75l1.439 1.44 1.263-1.263a.25.25 0 0 0 0-.354Z"></path></svg></a></span></div><div><button data-component="IconButton" type="button" aria-label="More edit options" data-testid="more-edit-button" aria-haspopup="true" aria-expanded="false" tabindex="0" class="prc-Button-ButtonBase-c50BI prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="small" data-variant="default" aria-describedby=":r98:-loading-announcement" id=":r98:"><svg aria-hidden="true" focusable="false" class="octicon octicon-triangle-down" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="m4.427 7.427 3.396 3.396a.25.25 0 0 0 .354 0l3.396-3.396A.25.25 0 0 0 11.396 7H4.604a.25.25 0 0 0-.177.427Z"></path></svg></button></div></div><button hidden="" data-testid="" data-hotkey="e,Shift+E" data-hotkey-scope="read-only-cursor-text-area"></button></div><button data-component="IconButton" type="button" aria-label="Outline" aria-pressed="false" class="Box-sc-g0xbh4-0 yaMnG prc-Button-ButtonBase-c50BI TableOfContents-module__IconButton--RCaNg prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="small" data-variant="invisible" aria-describedby=":ra2:-loading-announcement"><svg aria-hidden="true" focusable="false" class="octicon octicon-list-unordered" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M5.75 2.5h8.5a.75.75 0 0 1 0 1.5h-8.5a.75.75 0 0 1 0-1.5Zm0 5h8.5a.75.75 0 0 1 0 1.5h-8.5a.75.75 0 0 1 0-1.5Zm0 5h8.5a.75.75 0 0 1 0 1.5h-8.5a.75.75 0 0 1 0-1.5ZM2 14a1 1 0 1 1 0-2 1 1 0 0 1 0 2Zm1-6a1 1 0 1 1-2 0 1 1 0 0 1 2 0ZM2 4a1 1 0 1 1 0-2 1 1 0 0 1 0 2Z"></path></svg></button><div class="react-blob-header-edit-and-raw-actions-combined"><button data-component="IconButton" type="button" aria-label="Edit and raw actions" title="More file actions" data-testid="more-file-actions-button" aria-haspopup="true" aria-expanded="false" tabindex="0" class="prc-Button-ButtonBase-c50BI js-blob-dropdown-click BlobViewHeader-module__IconButton--uO1fA prc-Button-IconButton-szpyj" data-loading="false" data-no-visuals="true" data-size="small" data-variant="invisible" aria-describedby=":r9c:-loading-announcement" id=":r9c:"><svg aria-hidden="true" focusable="false" class="octicon octicon-kebab-horizontal" viewBox="0 0 16 16" width="16" height="16" fill="currentColor" display="inline-block" overflow="visible" style="vertical-align: text-bottom;"><path d="M8 9a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3ZM1.5 9a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Zm13 0a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3Z"></path></svg></button></div></div></div></div><div></div></div><div class="Box-sc-g0xbh4-0 hGyMdv"><section aria-labelledby="file-name-id-wide file-name-id-mobile" class="Box-sc-g0xbh4-0 fGqKFv"><div class="Box-sc-g0xbh4-0 eoaCFS js-snippet-clipboard-copy-unpositioned undefined" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto">Conditional Statements in Python: Even or Odd Checker</h1><a id="user-content-conditional-statements-in-python-even-or-odd-checker" class="anchor" aria-label="Permalink: Conditional Statements in Python: Even or Odd Checker" href="https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md#conditional-statements-in-python-even-or-odd-checker"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">🎯 Aim</h2><a id="user-content--aim" class="anchor" aria-label="Permalink: 🎯 Aim" href="https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md#-aim"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">To write a Python program to check whether the given number is <strong>even</strong> or <strong>odd</strong> using <code>if...else</code> statements.</p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">🧠 Algorithm</h2><a id="user-content--algorithm" class="anchor" aria-label="Permalink: 🧠 Algorithm" href="https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md#-algorithm"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="auto">
<li>Get an input from the user.</li>
<li>Convert the input to an integer and store it in a variable <code>a</code>.</li>
<li>Use the modulo operator <code>%</code> to check if <code>a % 2 == 0</code>.
<ul dir="auto">
<li>If true, print <code>"EVEN"</code>.</li>
<li>Else, print <code>"ODD"</code>.</li>
</ul>
</li>
<li>End the program.</li>
</ol>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">🧾 Program</h2><a id="user-content--program" class="anchor" aria-label="Permalink: 🧾 Program" href="https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md#-program"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>a=int(input())

if(a%2==0):
     print("EVEN")
else:
     print("ODD")
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="a=int(input())

if(a%2==0):
     print(&quot;EVEN&quot;)
else:
     print(&quot;ODD&quot;)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Output</h2><a id="user-content-output" class="anchor" aria-label="Permalink: Output" href="https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md#output"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="./Conditional Statements in Python_ Even or Odd Checker_files/438184680-e0509053-337e-4109-8509-440cd95de43c.png"><img src="./Conditional Statements in Python_ Even or Odd Checker_files/438184680-e0509053-337e-4109-8509-440cd95de43c.png" alt="image" style="max-width: 100%;"></a></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Result</h2><a id="user-content-result" class="anchor" aria-label="Permalink: Result" href="https://github.com/Kiran437228/Module1/blob/main/Conditional%20Statements%20in%20Python%3A%20Even%20or%20Odd%20Checker.md#result"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Thus, the python program was executed successfully</p>
</article></div><button hidden="" data-hotkey="Control+a"></button></section></div></div></div>   </div></div></div><div></div></div></div></div></div><div id="find-result-marks-container" class="Box-sc-g0xbh4-0 cCoXib"></div><button hidden="" data-testid="" data-hotkey-scope="read-only-cursor-text-area" data-hotkey="Control+F6,Control+Shift+F6"></button><button hidden="" data-hotkey="Control+F6,Control+Shift+F6"></button></div> <!-- --> <!-- --> <script type="application/json" id="__PRIMER_DATA_:R0:__">{"resolvedServerColorMode":"night"}</script></div>
</react-app>




  </div>

</turbo-frame>

    </main>
  </div>

  </div>

          <footer class="footer pt-8 pb-6 f6 color-fg-muted p-responsive" role="contentinfo" hidden="">
  <h2 class="sr-only">Footer</h2>

  


  <div class="d-flex flex-justify-center flex-items-center flex-column-reverse flex-lg-row flex-wrap flex-lg-nowrap">
    <div class="d-flex flex-items-center flex-shrink-0 mx-2">
      <a aria-label="Homepage" title="GitHub" class="footer-octicon mr-2" href="https://github.com/">
        <svg aria-hidden="true" height="24" viewBox="0 0 24 24" version="1.1" width="24" data-view-component="true" class="octicon octicon-mark-github">
    <path d="M12 1C5.9225 1 1 5.9225 1 12C1 16.8675 4.14875 20.9787 8.52125 22.4362C9.07125 22.5325 9.2775 22.2025 9.2775 21.9137C9.2775 21.6525 9.26375 20.7862 9.26375 19.865C6.5 20.3737 5.785 19.1912 5.565 18.5725C5.44125 18.2562 4.905 17.28 4.4375 17.0187C4.0525 16.8125 3.5025 16.3037 4.42375 16.29C5.29 16.2762 5.90875 17.0875 6.115 17.4175C7.105 19.0812 8.68625 18.6137 9.31875 18.325C9.415 17.61 9.70375 17.1287 10.02 16.8537C7.5725 16.5787 5.015 15.63 5.015 11.4225C5.015 10.2262 5.44125 9.23625 6.1425 8.46625C6.0325 8.19125 5.6475 7.06375 6.2525 5.55125C6.2525 5.55125 7.17375 5.2625 9.2775 6.67875C10.1575 6.43125 11.0925 6.3075 12.0275 6.3075C12.9625 6.3075 13.8975 6.43125 14.7775 6.67875C16.8813 5.24875 17.8025 5.55125 17.8025 5.55125C18.4075 7.06375 18.0225 8.19125 17.9125 8.46625C18.6138 9.23625 19.04 10.2125 19.04 11.4225C19.04 15.6437 16.4688 16.5787 14.0213 16.8537C14.42 17.1975 14.7638 17.8575 14.7638 18.8887C14.7638 20.36 14.75 21.5425 14.75 21.9137C14.75 22.2025 14.9563 22.5462 15.5063 22.4362C19.8513 20.9787 23 16.8537 23 12C23 5.9225 18.0775 1 12 1Z"></path>
</svg>
</a>
      <span>
        © 2025 GitHub,&nbsp;Inc.
      </span>
    </div>

    <nav aria-label="Footer">
      <h3 class="sr-only" id="sr-footer-heading">Footer navigation</h3>

      <ul class="list-style-none d-flex flex-justify-center flex-wrap mb-2 mb-lg-0" aria-labelledby="sr-footer-heading">

          <li class="mx-2">
            <a data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to Terms&quot;,&quot;label&quot;:&quot;text:terms&quot;}" href="https://docs.github.com/site-policy/github-terms/github-terms-of-service" data-view-component="true" class="Link--secondary Link">Terms</a>
          </li>

          <li class="mx-2">
            <a data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to privacy&quot;,&quot;label&quot;:&quot;text:privacy&quot;}" href="https://docs.github.com/site-policy/privacy-policies/github-privacy-statement" data-view-component="true" class="Link--secondary Link">Privacy</a>
          </li>

          <li class="mx-2">
            <a data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to security&quot;,&quot;label&quot;:&quot;text:security&quot;}" href="https://github.com/security" data-view-component="true" class="Link--secondary Link">Security</a>
          </li>

          <li class="mx-2">
            <a data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to status&quot;,&quot;label&quot;:&quot;text:status&quot;}" href="https://www.githubstatus.com/" data-view-component="true" class="Link--secondary Link">Status</a>
          </li>

          <li class="mx-2">
            <a data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to docs&quot;,&quot;label&quot;:&quot;text:docs&quot;}" href="https://docs.github.com/" data-view-component="true" class="Link--secondary Link">Docs</a>
          </li>

          <li class="mx-2">
            <a data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to contact&quot;,&quot;label&quot;:&quot;text:contact&quot;}" href="https://support.github.com/?tags=dotcom-footer" data-view-component="true" class="Link--secondary Link">Contact</a>
          </li>

          <li class="mx-2">
  <cookie-consent-link data-catalyst="">
    <button type="button" class="Link--secondary underline-on-hover border-0 p-0 color-bg-transparent" data-action="click:cookie-consent-link#showConsentManagement" data-analytics-event="{&quot;location&quot;:&quot;footer&quot;,&quot;action&quot;:&quot;cookies&quot;,&quot;context&quot;:&quot;subfooter&quot;,&quot;tag&quot;:&quot;link&quot;,&quot;label&quot;:&quot;cookies_link_subfooter_footer&quot;}">
      Manage cookies
    </button>
  </cookie-consent-link>
</li>

<li class="mx-2">
  <cookie-consent-link data-catalyst="">
    <button type="button" class="Link--secondary underline-on-hover border-0 p-0 color-bg-transparent" data-action="click:cookie-consent-link#showConsentManagement" data-analytics-event="{&quot;location&quot;:&quot;footer&quot;,&quot;action&quot;:&quot;dont_share_info&quot;,&quot;context&quot;:&quot;subfooter&quot;,&quot;tag&quot;:&quot;link&quot;,&quot;label&quot;:&quot;dont_share_info_link_subfooter_footer&quot;}">
      Do not share my personal information
    </button>
  </cookie-consent-link>
</li>

      </ul>
    </nav>
  </div>
</footer>



    <ghcc-consent id="ghcc" class="position-fixed bottom-0 left-0" style="z-index: 999999" data-initial-cookie-consent-allowed="" data-cookie-consent-required="false" data-catalyst=""></ghcc-consent>



  <div id="ajax-error-message" class="ajax-error-message flash flash-error" hidden="">
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert">
    <path d="M6.457 1.047c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0 1 14.082 15H1.918a1.75 1.75 0 0 1-1.543-2.575Zm1.763.707a.25.25 0 0 0-.44 0L1.698 13.132a.25.25 0 0 0 .22.368h12.164a.25.25 0 0 0 .22-.368Zm.53 3.996v2.5a.75.75 0 0 1-1.5 0v-2.5a.75.75 0 0 1 1.5 0ZM9 11a1 1 0 1 1-2 0 1 1 0 0 1 2 0Z"></path>
</svg>
    <button type="button" class="flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path d="M3.72 3.72a.75.75 0 0 1 1.06 0L8 6.94l3.22-3.22a.749.749 0 0 1 1.275.326.749.749 0 0 1-.215.734L9.06 8l3.22 3.22a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215L8 9.06l-3.22 3.22a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042L6.94 8 3.72 4.78a.75.75 0 0 1 0-1.06Z"></path>
</svg>
    </button>
    You can’t perform that action at this time.
  </div>

    <template id="site-details-dialog"></template>

    <div class="Popover js-hovercard-content position-absolute" style="display: none; outline: none;">
  <div class="Popover-message Popover-message--bottom-left Popover-message--large Box color-shadow-large" style="width:360px;"></div>
</div>

    <template id="snippet-clipboard-copy-button"></template>
<template id="snippet-clipboard-copy-button-unpositioned"></template>


    <style>
      .user-mention[href$="/dhashvanth21"] {
        color: var(--color-user-mention-fg);
        background-color: var(--bgColor-attention-muted, var(--color-attention-subtle));
        border-radius: 2px;
        margin-left: -2px;
        margin-right: -2px;
      }
      .user-mention[href$="/dhashvanth21"]:before,
      .user-mention[href$="/dhashvanth21"]:after {
        content: '';
        display: inline-block;
        width: 2px;
      }
    </style>


    </div>

    <div id="js-global-screen-reader-notice" class="sr-only mt-n1" aria-live="polite" aria-atomic="true">Module1/Conditional Statements in Python: Even or Odd Checker.md at main · Kiran437228/Module1</div>
    <div id="js-global-screen-reader-notice-assertive" class="sr-only mt-n1" aria-live="assertive" aria-atomic="true"></div>
  


<div class="sr-only mt-n1" id="screenReaderAnnouncementDiv" role="alert" data-testid="screenReaderAnnouncement" aria-live="assertive"></div><div id="__primerPortalRoot__" style="position: absolute; top: 0px; left: 0px;"></div></body></html>