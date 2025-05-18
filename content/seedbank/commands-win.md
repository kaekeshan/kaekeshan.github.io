---
title: Windows CLI 
description: Space to note down useful cmd & powershell commads
tags: [seed, dev, pwsh, cmd]
---

<details>
<summary>Command-Line</summary>

#### Files 
<!-- case 1 -->

<details>
<summary>Deleting a non empty directory </summary>  

```bash
rmdir /s /q $DIR_NAME
```
</details>

<!-- case 2 -->

<details>
<summary>Creating a empty file </summary>  

```bash
type NULL > $FILE_NAME
```
</details>

<!-- case 3 -->

<details>
<summary>Removing a File </summary>  

```bash
del $FILE_NAME
```
</details>

#### Variables

<!-- case 1 -->

<details>
<summary> windows-installation\Users\USER-NAME\AppData\local </summary>  

```bash
%localappdata%
```
</details>


</details>

---

<details>
<summary>PowerShell</summary>

#### Paths

<!-- case 1 -->

<details>
<summary> Copy the current directory path </summary>  

```bash
(Get-Location).Path | Set-Clipboard
```
</details>

</details>
