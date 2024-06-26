

****

### 上报告警
```json
    {
        "ori":"robot",
        "dest":"devsys",
        "type":"uploadAlarmData",
        "id":"123addf",
        "data":[{
          "faultCode":"60001",
          "faultTime":"2022-02-16 10:00:00",
          "faultReason":1
        }]
    }
```

### 上报当前任务
```json
    {
        "ori":"robot",
        "dest":"devsys",
        "type":"uploadCurrentTaskStatus",
        "id":"123addf",
        "data":{
          "taskCode":"5454545xxx",
          "taskType":1,
          "taskStatus":2,
          "stationList":[
            {
                "sn":1,
                "name":"站点1",
                "arrivalStatus":1
            },
            {
                "sn":2,
                "name":"站点2",
                "arrivalStatus":1
            },
            {
                "sn":3,
                "name":"站点3",
                "arrivalStatus":1
            },
            {
                "sn":4,
                "name":"站点4",
                "arrivalStatus":1
            },
            {
                "sn":5,
                "name":"站点5",
                "arrivalStatus":1
            }
          ]
        }
    }
```

### 站点到达
```json
{
    "ori":"robot",
    "dest":"devsys",
    "type":"uploadArrivedStation",
    "id":"123addf",
    "data":{
      "taskCode":"5454545xxx",
      "taskType":1,
      "taskStatus":2,
      "station":{
        "sn":1,
        "name":"站点1",
        "arrivalStatus":2
      }
    }
}
```


### 上报状态
```json
{
    "ori":"robot",
    "dest":"devsys",
    "type":"uploadStatus",
    "id":"54545645d4s5d4f5df45d6f",
    "data":{
        "type":1,
        "doorPassStatus":2,
        "liftRideStatus":5
    }
}
```

### 触边状态

```json
{
    "ori":"robot",
    "dest":"devsys",
    "type":"uploadStatus",
    "id":"54545645d4s5d4f5df45d6f",
    "data":{
        "type":2,
        "status":1
    }
}
```

//非配送

```json
{
    "ori":"robot",
    "dest":"devsys",
    "type":"uploadCurrentTaskStatus",
    "id":"123addf",
    "data":{
        "taskCode":"5454545xxx",
        "taskType":91,
        "taskStatus":2,
        "stationList":[
            {
            "sn":1,
            "name":"站点1",
            "arrivalStatus":2
            },
            {
            "sn":5,
            "name":"站点5",
            "arrivalStatus":3
            }
        ]
    }
}
```

### 人机应答智能柜日志下载
```json
{
    "data": {
        "status": 1 
    },
    "ori": "robot",
    "dest": "devsys",
    "type": "downloadSmartCabinetLog",
    "id": "b9c2a1bf21f845fea8087170de2d3810",
    "status": 1
}
```

//下载智能柜
```json
{
    "data": {
      "status": 1
    },
    "ori": "robot",
    "dest": "devsys",
    "type": "downloadSmartCabinetLog",
    "id": "f2f206e4eff14349bdf9c6e6ed8b80fb",
    "status": 0
}
```

//文件验证
```json
{
    "data": {
        "smartCabinetSn": "ddd1123",
        "date": "2024-06-16",
        "name": "ddd1123-20240616.zip",
        "size": "1000000"
    },
    "ori": "robot",
    "dest": "devsys",
    "type": "validateSmartCabinetLogSize",
    "id": "b9c2a1bf21f845fea8087170de2d3810",
    "status": 1
}
```

//获取上传地址
```json
{
    "data":{
        "fileList":[
            {
            "type":"downloadSmartCabinetLog",
            "name":"ddd1123-20240616.zip",
            "size":"1000000"
            }
        ]
    },
    "ori":"robot",
    "dest":"devsys",
    "type":"getUploadFileUrl",
    "id":"b9c2a1bf21f845fea808717",
    "status":1
}
```

//人机上报上传进度
```json
{
    "data": {
        "fileName": "ddd1123-20240616.zip",
        "process": 80,
        "recordId": "1803984277331914752"
    },
    "ori": "robot",
    "dest": "devsys",
    "type": "uploadUpProgress",
    "id": "b9c2a1bf21f845fea10",
    "status": 1
}
```

//人机上报上传完成
```json
{
    "data": {
        "type":"downloadSmartCabinetLog",
        "uploadList":[
            {
            "uploadId":"",
            "fileName": "ddd1123-20240616.zip",
            "status": 2,
            "recordId": "1803984277331914752"
            }
        ]
	},
	"ori": "robot",
	"dest": "devsys",
	"type": "uploadUpStatus",
    "id": "b9c2a1bf21f845fea10",
	"status": 1
}
```

****