#Run psexec on remote server

Add to TFSBuild.proj

```<PropertyGroup>
      <!-- call task on remote pc -->
      <StartBuildCompleteJobCommandLine>psexec \\Server -u domain\myTask -accepteula schtasks /Run  </StartBuildCompleteJobCommandLine>
</PropertyGroup>
```