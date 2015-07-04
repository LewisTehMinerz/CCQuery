# CCQuery
jQuery for ComputerCraft

## Methods
|Name|return|Desc|
|---|---|---|
|c.import(table pImport)|nil|Import the methods of pImport into c(down)|
|c.wget(string pUrl|table **wget**, [table pPost], [table pHeader])|string|Start a request to pUrl and return the content|
|c.dloadFile(string pUrl, string pFile)|nil|Download the url and put it in pFile|
|c.execUrl(string pUrl, [table fenv] or [cG])|return value of code|
|c.meta(table pTable, [table pMetatable])|table|return metatable of pTable and if pMetatable set new metatable|
|c.putFile(string filename, mixed content)|nil|Save content into filename. Auto-serialize!|
|c.getFile(string filename)|(string|table)/false|Get content of filename. Auto-unserialize|
|c.addToFile(string filename, string add, [boolean newLine])|boolean|Add *add* to *filename*. If *newLine* then it add "\n" before that|
|c.cloneTable(table pTable, [table into], [function if])|table|Copy *pTable* into the *return* table or into the *into* table. If *if* then only copy if it return true|
|c.api(string apiname, string url)|nil|Load the API *apiname*, if not exists it will downloaded|
|c.checkVersion(string version1, string version2)|number|return 0 if *v1* and *v2* are equal. return *1* if *v1* is newer, return *2* if *v2* is newer `v1 = "1.3443.464.06.4"`|
|c.isset(boolean if, function do)|nil|If *if* == true then exec *do*|
|c.config(string pName)|table (configObject)|Load a config table|
|c.isEmpty(mixed pVal)|boolean|See examples to watch how it works|
|c.isTable(mixed val)|boolean|Self explain|
|c.isBoolean(mixed val)|boolean|Self explain|
|c.isString(mixed val)|boolean|Self explain|
|c.isNumber(mixed val)|boolean|Self explain|
|c.isNil(mixed val)|boolean|Self explain|
|c.isFunction(mixed val)|boolean|Self explain|
|c.isObject(table Table)|boolean|return true when it's a child of cObject|
|c.isA(string Classname, obj Object)|boolean|return true when it is a Object of the class Classname|
|c.isAttr(string Attr)|boolean|Return true when Attr is not defined by down's classmanagment|
|c.serialize(table Table, [string **format**])|string|Serialize the table into a string|
|c.unserialize(string Value, [string **format**]["lua"])|table|Create a table from the string|
|c.sortField(table Table, string Field)|table|Sort the table with Selection Sort. table[i].field must be a number|
|c.newClass(string Name, table class, [table Mainclass]|nil|Creates a new Class from a Table|
|new.*CLASSNAME*(*CLASS ARGS*)|table/class|Create a new Object of a Class|
