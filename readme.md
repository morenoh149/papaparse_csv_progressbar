# Papaparse Remote csv progressbar example

```
$ python3 -m http.server
```

In a browser open localhost:8000

## Notes

CSV is a much more compact format for transferring information than json.
A row like

`bird,2,blue,0.00023`

might be expanded into a json payload like

```
{
    name: 'bird',
    age: 2,
    color: 'blue',
    heartRate: 0.00023
}
```

in my tests a 10mb csv gets expanded to several 100's of mb in http json requests.
