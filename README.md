# raskinbot    

category - category  
log - time recode  

## Install

// TODO

## Command

### add log

#### `command` 

```
send [target date(yyyymmdd)] [category id] [time]
```

#### `response` 

```
勤怠を追加しました。  
ログID:[log id]
カテゴリ名:[category name]
対象日:[target date(yyyy-mm-dd)]
時間:[time]h
```

### edit log

#### `command` 

```
edit [log id] [target date(yyyymmdd)] [category id] [time]
```

#### `response`

```
勤怠を編集しました。
ログID:[log id]
カテゴリ名:[category name]
対象日:[target date(yyyy-mm-dd)]
時間:[time]h
```

#### `etc`
time=0でデータ削除

## add category

#### `command` 

```
send-category [category name]
```

#### `response`

```
カテゴリを追加しました。
カテゴリID:[category id]
カテゴリ名:[category name]
時間:[time]
```

#### `etc`

## edit category

#### `command` 

```
edit-category [category id] [category name]
```

#### `response`

```
カテゴリを編集しました。
カテゴリID:[category id]
カテゴリ名:[category name]
時間:[time]
```

#### `etc`

カテゴリは削除できない。

## csv export

#### `command` 

```
export [target start date(yyyymmdd)] [target end date(yyyymmdd)]
```

#### `response`

※csv file
```
log id,category id,category name,username,target date,time,create at,update at
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

