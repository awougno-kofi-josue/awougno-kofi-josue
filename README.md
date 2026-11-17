cd %TEMP%
git clone https://github.com/awougno-kofi-josue/awougno-kofi-josue.git
cd awougno-kofi-josue
powershell -NoProfile -Command "Get-Clipboard | Set-Content -Encoding UTF8 README.md"
git add README.md
git commit -m "Apply full animated profile README"
git push
cd %USERPROFILE%
rmdir /s /q %TEMP%\awougno-kofi-josue
