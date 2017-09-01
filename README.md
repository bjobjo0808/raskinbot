# raskinbot    

task - 案件毎に作成  
log - 勤怠データ

## Command

### add log

#### `command` 

```
send [target date(yyyymmdd)] [task id] [time]
```

#### `response` 

```
勤怠を追加しました。  
ログID:[log id]
タスク名:[task name]
対象日:[target date(yyyy-mm-dd)]
時間:[time]h
```

### edit log

#### `command` 

```
edit [log id] [target date(yyyymmdd)] [task id] [time]
```

#### `response`

```
勤怠を編集しました。
ログID:[log id]
タスク名:[task name]
対象日:[target date(yyyy-mm-dd)]
時間:[time]h
```

#### `etc`
time=0でデータ削除

## add task

#### `command` 

```
send-task [task name]
```

#### `response`

```
タスクを追加しました。
タスクID:[task id]
タスク名:[task name]
時間:[time]
```

#### `etc`

## edit task

#### `command` 

```
edit-task [task id] [task name]
```

#### `response`

```
タスクを編集しました。
タスクID:[task id]
タスク名:[task name]
時間:[time]
```

#### `etc`

タスクは削除できない。

## csv export

#### `command` 

```
export [target start date(yyyymmdd)] [target end date(yyyymmdd)]
```

#### `response`

※csv file
```
log id,task id,task name,username,target date,time,create at,update at
```

#### `etc`

## help

#### `command` 

```
help
```

#### `response`

※後日記載

#### `etc`

