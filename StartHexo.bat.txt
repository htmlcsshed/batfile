@echo off
cd /D %~dp0
SET DP0=%~dp0

rem node.js
SET DP1=%DP0%node-v18.12.1-win-x64
SET NODE_PATH=%DP1%\node.exe
SET NCMD_PATH=%DP1%\npm.cmd

rem git
SET DP2=%DP0%git
SET GIT_PATH=%DP2%\bin\git.exe
SET GCMD_PATH=%DP2%\cmd

rem set path
SET PATH=%PATH%;%DP1%;%DP2%;%NODE_PATH%;%NCMD_PATH%;%GIT_PATH%;%GCMD_PATH%
cmd
