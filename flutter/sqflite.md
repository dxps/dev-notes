## Sqflite - Notes

My reference notes for some [](https://pub.dartlang.org/packages/sqflite)

##### Get first integer

To get just an integer as the result of a query, use something like this:
```dart
Future<int> getItemsCount() async {
//
return Sqflite.firstIntValue(await db.rawQuery('SELECT count(*) FROM $TableName'));
//
}
```
