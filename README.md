# Simplified Rime Configuration 

## Introduction

![image-20240320040425989](https://p.ipic.vip/jc2bcy.png)

This repository contains my customized Rime Input Method configuration, focusing primarily on full Pinyin input. It includes various enhancements and features to improve the typing experience.

## Main Features

- **Lua Configuration**: The `rime.lua` file includes various Lua scripts, offering configurable options like trigger keywords and prefixes that can be adjusted directly in the scheme files without altering the Lua files.
- **Character Selection by Word**: This feature allows you to select characters based on words, with shortcuts set in `default.yaml` to avoid conflicts with bracket page-turning. Other Lua configurations are set in the scheme files, as detailed in the comments.
- **Long Word Priority**: By default, this boosts the priority of longer words, placing a 2-word phrase in the 4th position.
- **Date and Time Input**: For full Pinyin, triggers include `rq` (date), `sj` (time), `xq` (week), `dt` (datetime), and `ts` (timestamp). Double Pinyin has its own set of triggers.

## Prefixes and Triggers

- **Unicode**: Starts with an uppercase "U", e.g., `U62fc` for "拼".
- **Symbols**: Initiated with "v" in full Pinyin or uppercase "V" in Double Pinyin.
- **Numerals and Currency**: Begins with an uppercase "R".
- **Lunar Calendar Dates**: Prefixed with an uppercase "N".

## Configuration Flexibility

Rime allows various ways to set configurations, such as direct settings in the scheme file (`xxx.schema.yaml`), scheme patch files (`xxx.custom.yaml`), or global settings in `default.yaml` that can be referenced across schemes. This flexibility enables shared settings like keyboard shortcuts across different schemes without redundancy.

## Customization and Patches

Customization files (`xxx.custom.yaml`) can add or override settings using the `patch` structure. This allows targeted adjustments at different levels of the configuration hierarchy, enabling precise control over the behavior of the input method.

## Lexicon Compilation

When creating lexicons, ensure the proper format and separation of columns for text, code, weight, and other attributes. This ensures efficient and accurate word prediction and selection.

## Mounting Custom Lexicons

Custom lexicons can be specified in the main schema or imported through the `import_tables` directive, allowing a modular approach to lexicon management. This system supports integrating multiple lexicon files for comprehensive and tailored input support.

## Custom Phrases

The `custom_phrase.txt` file can include specific key phrases or shortcuts for personal or frequently used terms, enhancing the efficiency and personalization of the input method.
