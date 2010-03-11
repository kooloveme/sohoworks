property Menus:TStrings;

property ScriptClick:string ; 单元名.类名.方法名
property MenuItemClick:TNotifyEvent

如果MenuItemClick实现，则调用MenuItemClick，否则检查ScriptClick属性，存在则调用，当前传递MenuItem.MenuIndex值