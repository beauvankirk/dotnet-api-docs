all : RemotingConfiguration_IsRemotelyActivatedClientType1_server.exe RemotingConfiguration_IsRemotelyActivatedClientType1_client.exe RemotingConfiguration_IsRemotelyActivatedClientType1_shared.dll

RemotingConfiguration_IsRemotelyActivatedClientType1_shared.dll : RemotingConfiguration_IsRemotelyActivatedClientType1_shared.cs
	csc /debug+ /nologo /t:library RemotingConfiguration_IsRemotelyActivatedClientType1_shared.cs

RemotingConfiguration_IsRemotelyActivatedClientType1_server.exe : RemotingConfiguration_IsRemotelyActivatedClientType1_server.cs RemotingConfiguration_IsRemotelyActivatedClientType1_shared.dll
	csc /debug+ /nologo /r:RemotingConfiguration_IsRemotelyActivatedClientType1_shared.dll RemotingConfiguration_IsRemotelyActivatedClientType1_server.cs

RemotingConfiguration_IsRemotelyActivatedClientType1_client.exe : RemotingConfiguration_IsRemotelyActivatedClientType1_client.cs RemotingConfiguration_IsRemotelyActivatedClientType1_shared.dll
	csc /debug+ /nologo /r:RemotingConfiguration_IsRemotelyActivatedClientType1_shared.dll RemotingConfiguration_IsRemotelyActivatedClientType1_client.cs

