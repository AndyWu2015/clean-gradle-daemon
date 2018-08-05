# clean-gradle-daemon
this is a shell for windows to clean all gradle daemon process


copy the following code and save as a bat file and run it. That is all.

<pre><code>
@echo off<br />
echo ------------------------------------------<br />
echo Liferay Kill All Gradle Daemon Process Kit<br />
echo ------------------------------------------<br />
for /f %%i in ('call jps^|find /i "GradleDaemon"') do ( echo %%i && taskkill /f /pid %%i )<br />
<pre><code>
