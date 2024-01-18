> On Developer command prompt
```
cd C:\Doc\Git Projects\PCF-Controls\ActionButton
```

```
npm install
```

```
msbuild /t:restore
```

```
mkdir ActionButtonSolution
cd ActionButtonSolution
```

```
pac solution init --publisher-name powerapps_samples --publisher-prefix sample
```

```
pac solution add-reference --path ../../ActionButton
```

```
msbuild /t:restore
```

```
msbuild /t:rebuild /restore /p:Configuration=Release
```

```
msbuild
```