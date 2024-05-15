
//上报告警
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

//上报当前任务
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


//站点到达
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



//上报状态
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

//触边状态

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


//非配送
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








