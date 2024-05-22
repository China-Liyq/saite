[

  {
    "ori":"robot",
    "dest":"devsys",
    "cmd":"uploadAlarm",
    "id":"5252525252",
    "data":{
      "alarms":[{
        "code":"50070",
        "time":"2023-08-21 16:28:00",
        "status":1
      }]

    }
  }
  ,


  {
    "ori":"robot",
    "dest":"devsys",
    "cmd":"uploadBmsInfo",
    "id":"5252525252",
    "data":{
      "bms":"AQAAUQBW9RYA6MsAALgLAAD/////AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAD/////",
      "runData":[0.00,0,0],
      "workData":[0,1,1,1]
    }
  }
,


  {
    "ori":"robot",
    "dest":"devsys",
    "cmd":"uploadBatteryMaintenanceResult",
    "id":"5252525252",
    "data":{
      "taskId":"454545455545",
      "status":1
    }
  }
,
  {
    "ori":"robot",
    "dest":"devsys",
    "cmd":"uploadBatteryMaintenanceResult",
    "id":"5252525252",
    "data":{
      "taskId":"454545455545",
      "status":0,
      "failCode":1
    }
  }
,
  {
    "ori":"robot",
    "dest":"devsys",
    "cmd":"getFileUploadUrl",
    "id":"5252525252",
    "data":{
      "fileList":[
        {
          "type":"downNavigationLog",
          "logType":100,
          "name": "OSFileIO.java",
          "size": "5457645"
        }
      ]
    }
  }
,

  {
    "ori":"robot",
    "dest":"devsys",
    "cmd":"fileUploadProcess",
    "id":"5252525252",
    "data":{
      "name":"OSFileIO.java",
      "process":10,
      "recordId":"1775097074182926336"
    }
  }
,
  {
    "ori":"robot",
    "dest":"devsys",
    "cmd":"fileUploadStatus",
    "id":"5252525252",
    "data":{
      "type":"downLog",
      "uploadList":[
        {
          "uploadId":"",
          "status":1,
          "fileName": "OSFileIO.java",
          "recordId": "1775097074182926336",
          "logType": 100
        }
      ]
    }
  }

,

{
    "ori":"robot",
    "dest":"devsys",
    "cmd":"uploadStatus",
    "id":"5252525252",
    "data":{
        "type":1,
        "steeringAngle":30
    }
}
,

{
    "ori":"robot",
    "dest":"devsys",
    "cmd":"uploadDriverMode",
    "id":"5252525252",
    "data":{
        "type":2,
        "mode":2
    }
}




]