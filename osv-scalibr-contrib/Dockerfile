# escape=`
FROM mcr.microsoft.com/windows/servercore:ltsc2022

SHELL ["powershell","-Command"]

# Set workdir to Desktop
WORKDIR "C:/Users/ContainerUser/Desktop"

# Copy all .exe from build context into Desktop inside container
COPY *.exe ./

# Optional: install WinRAR silently (if included in exes)
# RUN Start-Process -FilePath .\winrar-x64-712.exe -ArgumentList '/S' -Wait -NoNewWindow

# Default: open a shell when container starts
CMD ["cmd"]
